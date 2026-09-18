# Stage 5 — Jurisdiction, Authority and Temporal-Validity Model

**Stage:** 5 of the Legal Skills bootstrap (v1.2)  
**Date:** 19 September 2026  
**Branch:** `feat/bootstrap-3`  
**Status:** Complete — accepted input for Stage 6  
**Governing section:** §11 of `2026-09-08-legal-skills-new-project-bootstrap-process.md`  
**Inputs:** Stage 1 (§4 zones, §6.3 jurisdiction strategy); Stage 3 (C3–C8); Stage 4 main log (§3.2, §5, §6 N4–N7, N25–N27, §9) and supporting logs c, d, e, f

This log defines the **smallest useful** jurisdiction context, authority record and temporal-validity contract. It is a model, not a schema file, a database or a jurisdiction engine. Field names are provisional until Stage 6 fixes the artefacts.

---

## 1. Evidence used

Most evidence was gathered in Stage 4. Stage 5 added targeted checks of official sources.

### 1.1 Stage 4 evidence relied on (by ID)

| Topic | Evidence |
| --- | --- |
| legislation.gov.uk status apparatus: status line, changes banner, prospective marking, changes table, lag | F-01, F-02, F-16, F-17, F-19, F-29, F-30, F-37; C-19, C-20 |
| Provision-level and staged commencement; transitional provisions; amended instruments | C-17, C-19, C-20 (Data (Use and Access) Act 2025); D log (DMCC Act 2024) |
| Official case law; neutral citations; versions; no free official citator | F-03, F-20, F-33 |
| Forum-dependent citability | F-13, F-36 |
| EU: Official Journal is authentic; consolidated texts "have no legal effect"; application dates can be amended | F-11, F-12; C-22, C-23 |
| Assimilated law and the post-2023 court position | F-15 to F-18 |
| Regulator guidance with status banners and update dates | C-05 to C-16; D log (CMA37, PERG) |
| Registry evidence and representation rules | E log (TMA 1994 ss 5, 82, 84; UK IPO manual; USPTO rule) |
| Three-test citation verification; misgrounded citations | F-04, F-05, F-08, F-38 |
| Advice boundary is jurisdiction-dependent | F-21 to F-25 |

### 1.2 Stage 5 checks (retrieved 19 September 2026; fetch-tool extracts unless stated)

| ID | Source | Result |
| --- | --- | --- |
| S5-01 | legislation.gov.uk developer page, URI scheme — https://www.legislation.gov.uk/developer/uris | Provision-level URIs (`/{type}/{year}/{number}/section/{n}`); `/enacted` or `/made` for the original text; a date in the URI (`/YYYY-MM-DD`) gives the text as it stood on that date; dates before 1 February 1991 redirect to the base date; data formats via `data.ext`. |
| S5-02 | Find Case Law, "About this service" — https://caselaw.nationalarchives.gov.uk/about-this-service | Covers England and Wales courts and tribunals plus UK-wide Supreme Court and Privy Council; mostly from the early 2000s; not complete (many decisions are never transcribed); gives no legal advice. The page says nothing about later treatment. |
| S5-03 | EUR-Lex help, CELEX numbers — https://eur-lex.europa.eu/content/help/eurlex-content/celex-number.html | CELEX = sector + year + type + number. Sector 3 = legal acts. Sector 0 = consolidated texts, written as the act number plus the consolidation date (example given: `02009L0156-20161018`). |
| S5-04 | GOV.UK, "Search for a trade mark" — https://www.gov.uk/search-for-trademark | Search by number, owner, keyword / phrase / image. Purpose stated: check whether a similar mark exists; find the owner. No date shown. No guidance on how to assess similarity. |
| S5-05 | Companies House developer overview — https://developer.company-information.service.gov.uk/overview | REST API over public company data. The overview page says nothing about cost, keys or accuracy of filed data. **Not enough to profile the register**; bounded in §8. |
| S5-06 | EUTMR (Reg (EU) 2017/1001) on EUR-Lex | **Failed again:** the fetch cut off at Article 53, before Articles 119–120. |
| S5-07 | Web search on EUTMR Art 119(2) (results include the EUIPO representation FAQ and an article-level mirror) | Search-level only: persons with no domicile, principal place of business or real establishment in the EEA must be represented in all proceedings **other than filing an application**. **Not inspected at a primary source.** Gap G1 stays open, narrowed. |
| S5-08 | USPTO rule page (URL from memory) | 404. Stream E had already inspected the USPTO rule at source (E log). No new evidence. |

Main-session primary checks already recorded in Stage 4 §1: DMCC Act 2024 Part 4 ch 2 marked "Prospective"; TMA 1994 ss 82 and 84 with no known outstanding effects.

---

## 2. Design rules (from the evidence)

| # | Rule | Why |
| --- | --- | --- |
| R1 | The unit of authority is the **provision or the passage**, not the instrument or the case. | Status differs inside one Act and inside one section (FF1-04; C-19). |
| R2 | Every record carries **three dates at least**: source date, retrieved-at, and the as-at date the proposition is asserted for. | Official revised text lags (F-01); banners change. |
| R3 | **Four things are never merged:** the authority, the proposition drawn from it, the interpretation applied, and the verification status. | SC1-11 to SC1-13; misgrounded citations (F-08). |
| R4 | Status is **typed**, never a boolean. | FF1-06; N5. |
| R5 | Source class and standing are **relative to a forum**. | SC1-16; F-13; F-36. |
| R6 | Jurisdiction is **resolved per matter and per issue**. It is never a pack, a directory or a default. | Bootstrap §21.2; Stage 1 §6.3. |
| R7 | "Unresolved" and "not checked" are **valid values**. They block confident wording; they do not block the work. | N7; §4 of the Stage 4 log. |
| R8 | A model-written extract is **not** an inspection of the source for a material proposition. | N12 (observed six times in Stage 4, and again at S5-06). |
| R9 | The record stores **pointers and short pinpoints**, not copies of law. | Non-goals: no legislation mirror, no case-law database. |
| R10 | Reference data (court hierarchy, source profiles) is **dated configuration**, not knowledge. | FF1-24; F-15 to F-18. |

---

## 3. Jurisdiction context

### 3.1 Record

One per matter. Issue-level overrides are allowed, because one product can raise issues under different laws.

| Field | Required | Values / notes |
| --- | --- | --- |
| `matter_territories` | Yes | Where the conduct, product or document operates. List. |
| `governing_law` | When a document is in scope | Stated choice, or `none stated`, or `unresolved`. Drives the label lock (Stage 4 N11). |
| `forum` | When material | Court, tribunal, regulator or registry that would decide. Drives source standing (R5). |
| `regulators` | When material | Body + power (guidance only / enforcement / fining). |
| `actor_locations` | Yes | Entity, place of establishment, and role decided from facts (controller / processor; provider / deployer; trader). |
| `user_locations` | When consumers, data subjects or end users matter | Markets actually offered into, not only intended. |
| `asset_right_territories` | For IP, licensing, registry work | Per right. Rights are territorial. |
| `choice_of_law_terms` | When present | Pointer to the clause. |
| `material_dates` | Yes | Event date(s), launch date, contract date, filing or priority date. At least one. |
| `analysis_as_at` | Yes | The date the analysis is valid for. Defaults to the retrieval date. May be a past event date or a planned launch date. |
| `cross_border_questions` | When any | Open list: for example "UK-only lawful basis used for EU users". |
| `advice_boundary_note` | Yes | Result of the zone check for this territory (Stage 1 §4), including the individualisation test outside England and Wales (Stage 4 N26). |
| `resolution_status` | Yes, per field group | `resolved` / `assumed (stated)` / `unresolved` / `out of proving scope`. |

### 3.2 Rules

1. **Do not collapse:** `matter_territories` ≠ `governing_law` ≠ `forum`. A contract under English law can be enforced by a regulator of another state against conduct in a third.
2. **`unresolved` is reported, not hidden.** An output with an unresolved jurisdiction field must say which conclusions depend on it.
3. **Proving scope (Stage 1 §6.3):** England and Wales / UK first; EU instruments second; US only where a fixture needs it. Other territories: the method still runs; every proposition is marked `out of proving scope` and the matter is a Zone B candidate.
4. **No universal conflict-of-laws engine.** Conflict questions are recorded in `cross_border_questions` and escalated when material.
5. **One regime's rule is never carried into another without its own authority record.** (Stage 4 T3; example: UK GDPR Art 6(1)(ea) is UK-only.)

---

## 4. Authority record

### 4.1 Core fields (every authority)

| Field | Required | Values / notes |
| --- | --- | --- |
| `authority_id` | Yes | Local identifier within the matter. |
| `identity` | Yes | Official title + provision or paragraph pinpoint. |
| `citation` | Yes | Official identifier: year-and-chapter or SI number; neutral citation; CELEX or ELI; register number; SPDX expression. |
| `locator` | Yes | Stable URI where one exists (S5-01, S5-03). |
| `source_class` | Yes | See §4.2. |
| `jurisdiction` | Yes | Territory and, for UK legislation, extent. |
| `issuing_body` | Yes | Legislature, court and level, regulator, registry, licence steward. |
| `standing` | Yes, **per forum** | `mandatory` / `optional` / `not permissible` / `research only, not citable` (Stage 4 §3.2, SC1-16). `unknown` allowed. |
| `source_date` | Yes | Enactment, making, judgment, publication or last-updated date. `not shown` is a valid value and is itself a finding (Stage 4 N27). |
| `retrieved_at` | Yes | Date, and time when registers are involved. |
| `version_read` | Yes | Which text was actually read: see §4.3–§4.6. |
| `inspection_mode` | Yes | `raw text read` / `model-written extract` / `search result only` / `secondary report of the source`. (R8) |
| `verification` | Yes | See §6. |
| `notes_on_limits` | When any | Banner text, blocked pages, translation, mirror. |

### 4.2 Source classes

Merged from Stage 3 (C6) and Stage 4 (N4, FF1-09 extension).

| Class | Examples | Default role |
| --- | --- | --- |
| `primary-legislation` | Act; EU regulation or directive (Official Journal) | Can support a proposition of law |
| `secondary-legislation` | Statutory instrument; commencement regulations | Same; often holds the dates (FF1-01) |
| `case-law` | Judgment with neutral citation | Same; subject to §4.4 |
| `treaty` | | Same; check domestic effect |
| `statutory-code-or-guidance` | Guidance a body must issue or a court must consider | Strong practical weight; say what the statute makes of it |
| `regulator-guidance` | ICO, CMA, FCA perimeter guidance | Soft law: see §4.5 |
| `court-practice-direction` | Citation practice directions | Governs citability in that forum |
| `official-register-entry` | Trade mark, company, design register entry | A **dated fact**, not a legal conclusion |
| `registry-guidance` | UK IPO manual | Practice of the office; not law |
| `licence-text` | Versioned licence text | The operative text for licence obligations |
| `steward-interpretation` | Licence steward FAQ | Persuasive only |
| `government-proposal` | Consultation; report; bill not enacted | **Never** supports a statement of current law (Stage 4 N25) |
| `professional-commentary` | Practitioner text; law-firm note; journal | Finding aid and context |
| `finding-aid` | Headnote; digest; explanatory note; licence summary; scanner output; register hit list; **consolidated EU text**; **any model-written summary** | Never the sole support for a proposition |

### 4.3 Legislation extension

| Field | Values / notes |
| --- | --- |
| `provision` | Section, subsection, regulation, article, schedule paragraph (R1). |
| `text_version` | `as enacted` / `latest revised` / `point-in-time (date)` / `authentic OJ text` / `consolidated (documentation only)`. |
| `in_force_state` | `in force` / `partly in force` / `enacted, prospective` / `announced, not enacted` / `repealed` / `expired` / `unknown`. |
| `commencement` | Mode (on assent; fixed date; period after assent; by regulations) + instrument + date, per provision. For the EU: entry into force **and** application date, and whether the application date has itself been amended. |
| `effects` | Typed list using the official vocabulary (amended, substituted, inserted, repealed, applied, disapplied, modified, excluded, saved, …) each with `applied_to_text: yes / not yet`. |
| `changes_banner` | Verbatim short text of any "changes not yet applied" or "prospective" notice + the page's "up to date to" date. |
| `transitional_saving` | Which version governs events before and after commencement. `none found` / `not checked`. |
| `amending_or_amended` | If this provision only edits another instrument, the record points to the **amended** instrument, which gets its own record. |
| `extent` | Territorial extent; devolved matter flag. |
| `provenance` | `domestic` / `assimilated` / `implements international obligation` / `rights-sensitive`. |

### 4.4 Case-law extension

| Field | Values / notes |
| --- | --- |
| `court_level` | From dated reference data (§7.2). |
| `version_read` | `handed-down transcript` / `official report` / `other report` / `press summary (finding aid)`. |
| `best_report_available` | If known. |
| `appellate_history` | `none found` / `affirmed` / `reversed` / `varied` / `appeal pending` / `not checked`. |
| `later_treatment` | `applied` / `followed` / `approved` / `distinguished` / `doubted` / `not followed` / `overruled` / `none found` / `not checked`. |
| `later_treatment_method` | `commercial citator` / `free-text search of official sources` / `none`. **`none` blocks confident wording on a material point.** |
| `citability` | Forum-specific restriction, if any. |
| `pinpoint` | Paragraph number(s) actually read. |
| `holding_or_dicta` | `holding` / `possibly dicta` / `unclear`, with the level of generality chosen and the court's own words as anchor (SC1-12). |

### 4.5 Guidance extension (soft law)

| Field | Values / notes |
| --- | --- |
| `legal_status` | `statutory guidance` / `regulator guidance` / `voluntary code` / `non-binding by its own terms`. |
| `applied_by` | Who applies it and with what power (court only; regulator with fining power). |
| `reliance_effect` | `safe harbour` / `"have regard"` / `none stated`. |
| `practical_weight` | `defines the operative test in practice` / `persuasive` / `background`. |
| `currency_state` | `current` / `under review (banner quoted)` / `updated on (date)` / `consultation draft` / `superseded` / `withdrawn`. |

### 4.6 Register and licence extensions

| Field | Values / notes |
| --- | --- |
| Register: `office`, `register_number`, `status`, `owner`, `classes_and_specification`, `filing_or_priority_date`, `query_used`, `retrieved_at` (date and time) | A register entry proves what the register showed at that moment. It proves nothing about conflict, validity or clearance (Stage 4 N15). |
| Licence: `spdx_expression`, `version`, `only_or_later`, `source_of_identification` (file header / manifest / scanner / vendor statement), `text_read` | Default is a frozen version (Stage 4, AD3-14 adapted). |

---

## 5. Proposition record

The link between an authority and the analysis. Kept separate from the authority (R3).

| Field | Required | Values / notes |
| --- | --- | --- |
| `proposition_id` | Yes | |
| `statement` | Yes | One proposition of law, in the analyst's own words. |
| `authority_refs` | Yes | One or more `authority_id` + pinpoint. |
| `support_type` | Yes | `text states it` / `holding` / `inference from text` / `guidance states it` / `commentary only`. |
| `quotation` | When used | Short; marked `text-verified` or `as reported`. |
| `jurisdiction` and `as_at` | Yes | The proposition is asserted only for this territory and this date. |
| `interpretation_note` | When the text is vague or open-textured | Which kind of indeterminacy; where the meaning was taken from; alternative readings (Stage 4, SC2-10 adapted). |
| `contrary_authority_refs` | When any | With the balance stated (C9). |
| `dependent_on_facts` | When any | Links to fact or assumption records (Stage 6). |
| `verification` | Yes | §6. |
| `stability` | Yes | `settled` / `moving (pending reform, guidance under review, appeal pending)` / `unknown`. Feeds "confidence in the analysis" (Stage 4 §4 item 6). |

A proposition with `support_type = commentary only` or whose only authority is a `finding-aid` **cannot** be delivered as a statement of law.

---

## 6. Verification status

Three independent tests (Stage 4 N6), then currency, then treatment. Each is recorded separately so that each can fail separately (Stage 18).

| Test | Pass means | Values |
| --- | --- | --- |
| V1 Existence | The authority exists at the citation and locator | `pass` / `fail` / `not checked` |
| V2 Text | The pinpointed words are in the version read; any quotation matches | `pass (raw text)` / `pass (extract only)` / `fail` / `not checked` |
| V3 Support | The text supports the proposition as stated, at the stated level of generality | `pass` / `partial` / `fail` / `not checked` |
| V4 Currency | §4.3 or §4.5 fields completed for the as-at date | `pass` / `qualified (banner / under review)` / `fail` / `not checked` |
| V5 Treatment | §4.4 appellate history and later treatment recorded with method | `pass` / `qualified (no citator)` / `not applicable` / `not checked` |
| V6 Jurisdiction fit | Authority's territory, extent and forum match the jurisdiction context | `pass` / `fail` / `unresolved` |

Derived gates (categorical, tied to the action — Stage 4, SC2-24 adapted):

| Gate | Minimum |
| --- | --- |
| **May inform research** | V1 pass |
| **May support a stated proposition** | V1–V3 pass, V2 on raw text for any quotation, V6 pass |
| **May support confident wording on a material point** | The above + V4 pass or qualified-and-disclosed + V5 pass, or qualified-and-disclosed |
| **Must be disclosed as a limit** | Any `not checked`, `extract only`, `qualified`, `unresolved` |
| **Blocks delivery as law** | V1 or V3 fail; only finding-aid support; `government-proposal` used for current law |

`pass (extract only)` exists because this project's own tools produce model-written extracts. It is honest, and it is weaker.

---

## 7. Temporal-validity contract

### 7.1 Dates that must stay distinct

```text
made / enacted / judgment / publication date      (source_date)
commencement / application / effective date        (commencement; per provision)
amendment / repeal / later-treatment date          (effects; later_treatment)
source "up to date to" date                        (changes_banner)
retrieved_at                                       (when we looked)
analysis_as_at                                     (the date the conclusion is valid for)
material_dates                                     (when the facts happened or will happen)
```

Rules:

1. `analysis_as_at` is stated on every deliverable. It never silently means "today".
2. If a `material_date` is **before** `analysis_as_at`, the question is "which version governed that event?" Use point-in-time text where the source offers it (S5-01) and check transitional provisions.
3. If a `material_date` is **after** `analysis_as_at` (a planned launch), prospective provisions and announced changes are reported as `enacted, prospective` or `announced, not enacted`, with the latest official statement of timing and its date. They are never reported as law in force. They are never ignored.
4. Every trace link and every record carries its creation date (Stage 4 N8, C-30).
5. **Staleness is a state, not an error.** A record older than the matter's refresh rule, or whose `stability` is `moving`, is re-verified before reuse. The refresh rule is set per matter; the model does not fix a number.
6. A refresh re-runs V4 and V5 only, unless they fail. Dependent propositions are re-opened only if the authority changed (smallest responsible unit).

### 7.2 Dated reference data

Kept as small configuration tables, each with `verified_on`, `source`, and a `prospective_changes` column (Stage 4, FF1-24 adapted):

- court hierarchy and who binds whom, per jurisdiction;
- status of assimilated EU law and the courts' power to depart from it;
- source profiles (§8);
- per-office representation rules for registries;
- the advice-boundary test per territory.

Stage 5 does **not** populate these tables beyond §8. They are built when a workflow or fixture needs them, from sources inspected at that time. The 2011 content in the Stage 3 logs must not be used.

---

## 8. Source profiles (proving jurisdictions)

What each source can and cannot tell the model. Verified on 18–19 September 2026 unless stated.

| Source | Gives | Does not give | Evidence |
| --- | --- | --- | --- |
| legislation.gov.uk (UK) | Provision-level URIs; as-enacted, revised and point-in-time text; status line; changes banner; prospective marking; typed effects table; extent | Guaranteed currency: revised text can lag; effects may be "not yet applied"; changes data lags by weeks | S5-01; F-01, F-02, F-37; C-20 |
| Find Case Law (E&W + UKSC / JCPC) | Official judgments from about the early 2000s; neutral citations | Completeness; later treatment; law reports | S5-02; F-03 |
| BAILII | Free judgments | Returned 403 to fetch tools in Stage 4 | B log; F-20 |
| Commercial citators | Appellate history; later treatment | Free access. **No free official UK citator was found.** | F-33 |
| ICO, CMA, FCA sites | Guidance with update dates and "under review" banners; PERG | Binding law; PERG "does not bind the courts" | C-05 to C-16; D log |
| EUR-Lex (EU) | Official Journal text (authentic); CELEX and ELI identifiers; consolidated texts labelled by date | Legal effect for consolidated texts. Long acts were truncated by the fetch tool twice. | S5-03, S5-06; F-11, F-12 |
| UK IPO search and manual | Register entries; examination practice | Any assessment of similarity or clearance | S5-04; E log |
| EUIPO | — | Pages blocked in Stage 4 and Stage 5. Representation rule known at search level only. | S5-07; E log |
| USPTO | Register; representation rule for foreign-domiciled applicants | — | E log |
| WIPO (Madrid Monitor, Global Brand Database) | **Not inspected** | — | Gap |
| Companies House | Public company data by API | Accuracy of filed data, cost and key rules **not established** from the page read | S5-05 |
| Licensed legal databases | — | **No access in this bootstrap.** Any workflow that needs them must say so. | — |

---

## 9. Do-not-collapse rules (acceptance checks for later stages)

```text
jurisdiction        ≠ governing law ≠ forum
authority           ≠ proposition   ≠ interpretation ≠ verification status
enacted             ≠ in force      ≠ applied to this event
publication date    ≠ effective date ≠ retrieved-at ≠ analysis as-at
revised text        ≠ current law automatically   (read the banner)
consolidated EU text≠ authentic text
regulator guidance  ≠ legislation   (and ≠ "only guidance")
government proposal ≠ law
register entry      ≠ legal clearance ≠ ownership proof
licence summary     ≠ licence text;  scanner output ≠ licence finding
model-written extract ≠ the source
no negative treatment found ≠ good law   (say which method was used)
existence of a case ≠ support for the proposition
```

---

## 10. Worked records (exit test)

Each ties a material proposition to verified authority and a defined jurisdiction and time context. Values are real and come from this bootstrap's own checks.

### 10.1 Prospective legislation

| Field | Value |
| --- | --- |
| Proposition | The subscription-contract regime in Part 4, Chapter 2 of the Digital Markets, Competition and Consumers Act 2024 is enacted but not in force. |
| Jurisdiction / as-at | UK / 19 September 2026 |
| Authority | 2024 c. 13, Part 4 ch 2 — `primary-legislation` — https://www.legislation.gov.uk/ukpga/2024/13/part/4/chapter/2 |
| `in_force_state` | `enacted, prospective` |
| `changes_banner` | Page reports provisions that are prospective, and one outstanding insertion by a 2026 Act not yet applied |
| Timing statement | Government statement of 2 April 2026 anticipates spring 2027 (stream D; `government-proposal` class for timing only) |
| Verification | V1 pass · V2 pass (extract only) · V3 pass · V4 pass · V5 n/a · V6 pass |
| Use | For a launch planned after the as-at date: report under rule 7.1(3). Do not state these duties as current. |

### 10.2 Provision with a clean status

| Field | Value |
| --- | --- |
| Proposition | An unregistered person who, in business, describes themselves as a "registered trade mark attorney" commits a summary offence. |
| Jurisdiction / as-at | UK / 19 September 2026 |
| Authority | Trade Marks Act 1994 s 84 — https://www.legislation.gov.uk/ukpga/1994/26/section/84 |
| `in_force_state` / banner | `in force`; "no known outstanding effects" |
| Verification | V1 pass · V2 pass (extract only) · V3 pass · V4 pass · V6 pass |
| Use | Supports Stage 1 Zone C "use of protected titles". Read with s 82 (agents) — see Stage 4 §5 correction. |

### 10.3 Guidance under review

| Field | Value |
| --- | --- |
| Proposition | The ICO's published method for privacy information (right to be informed) is the practical test for notice content, and the page is flagged as under review because of the Data (Use and Access) Act. |
| Jurisdiction / as-at | UK / 18 September 2026 |
| Authority | ICO right-to-be-informed guidance — `regulator-guidance` (stream C, C-05) |
| Guidance fields | `legal_status`: regulator guidance · `applied_by`: ICO with enforcement powers · `practical_weight`: defines the operative test in practice · `currency_state`: under review (banner quoted in log c) |
| Verification | V1 pass · V2 pass (extract only) · V3 pass · V4 **qualified** · V6 pass |
| Use | May be relied on with the limit disclosed. `stability = moving`: re-verify before reuse. |

### 10.4 EU act whose application dates moved

| Field | Value |
| --- | --- |
| Proposition | Obligations for stand-alone (Annex III) high-risk AI systems under Regulation (EU) 2024/1689 apply from 2 December 2027, following amendment by Regulation (EU) 2026/1744. |
| Jurisdiction / as-at | EU / 19 September 2026 |
| Authorities | Reg (EU) 2024/1689 and Reg (EU) 2026/1744 — Official Journal texts (authentic). Consolidated text, if used, is a `finding-aid`. |
| `commencement` | Entry into force and application date recorded separately; `application date amended: yes (OJ 24 July 2026; in force 27 July 2026)` |
| Verification | V1 pass · V2 pass (extract only; stream C) · V3 pass · V4 pass · V6 pass. Main session: search-level confirmation only. |
| Use | Any advice written before 24 July 2026 that gives 2 August 2026 for these duties is stale (Stage 4, C-F8). Article-level wording must be re-read at source before durable quotation. |

### 10.5 What a failing record looks like

A case cited from a model's memory with no locator: V1 `not checked` → may not inform even research output as authority. A real judgment whose holding was taken from a fetch-tool summary: V2 `pass (extract only)`, V3 **not yet trustworthy** — Stage 4 recorded a summary that reversed the holding (B-F8). The record must be upgraded to raw text before it supports a proposition on a material point.

---

## 11. Bounded gaps

| # | Gap | Bound |
| --- | --- | --- |
| G1 | EUIPO representation (EUTMR Arts 119–120) not inspected at a primary source; known at search level: representation is required for non-EEA parties in proceedings other than filing | EU trade mark filing and proceedings stay Zone B |
| G2 | WIPO sources not inspected | Not used until inspected |
| G3 | Companies House profile incomplete | Register entries are dated facts only; no accuracy claim |
| G4 | No access to commercial citators | `later_treatment_method` must say so; V5 is `qualified` |
| G5 | Hierarchy of law report series: Practice Direction inspected (F-13); detail not rebuilt | Build the reference table when a fixture needs it |
| G6 | Court-hierarchy and assimilated-law tables not populated | §7.2: build on demand from sources inspected then |
| G7 | US and EU member-state source profiles not built | Out of first proving scope; propositions marked accordingly |
| G8 | Fetch tools truncate long EU acts and return model-written extracts | `inspection_mode` records it; Stage 11 must find a raw-text route |

---

## 12. Exit verification

| Requirement (bootstrap §11) | Where | Met |
| --- | --- | --- |
| Smallest useful jurisdiction context | §3 | Yes — 13 fields, most conditional |
| All candidate jurisdiction fields considered | §3.1 covers matter territory, governing law, forum / regulator, actor location, user location, establishment / offering, data-subject location (under `user_locations`), asset / right territory, choice-of-law terms, material dates, cross-border questions | Yes |
| Authority record with the candidate fields | §4: identity, URL / citation / registry reference, type, jurisdiction, issuing body, binding / persuasive / guidance status, publication / judgment date, effective / commencement date, amendment / repeal status, appeal / later treatment, retrieved-at, valid-as-of, proposition supported (§5), pinpoint, verification status (§6) | Yes |
| Temporal-validity contract | §7 | Yes |
| Official sources researched: legislation, case law, regulators, UK IPO / EUIPO / WIPO / USPTO, EUR-Lex, corporate registries, licensed databases | §8, with honest gaps for EUIPO, WIPO, Companies House and licensed databases (§11) | Yes, with bounded gaps |
| Do-not-collapse list respected and extended | §9 | Yes |
| No universal jurisdiction engine, registry mirror or legal database | R6, R9, §3.2(4), §7.2 | Yes |
| **Exit: a material proposition can be tied to verified authority and a defined jurisdiction / time context** | §10 — four worked records from real checks, and one failing pattern | Yes |
