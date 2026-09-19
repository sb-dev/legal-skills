# Stage 11 — Legal AI Skills, Databases, Registries and Tools

**Stage:** 11 of the Legal Skills bootstrap (v1.2)  
**Date:** 19 September 2026  
**Branch:** `feat/bootstrap-3`  
**Status:** Complete — accepted input for Stage 12  
**Governing section:** §17 of `2026-09-08-legal-skills-new-project-bootstrap-process.md`  
**Inputs:** Stage 5 (authority record, verification tests V1–V6, source profiles, gaps); Stage 7 (tool-dependent steps); Stage 10 (sensitivity classes, routes, most-exposed-tool rule)

Supporting records:

| Log | Categories | Evidence rows |
| --- | --- | --- |
| `2026-09-19-stage-11a-skills-providers-evals.md` (`J-`) | Legal Agent Skills; legal MCP servers and connectors; legal AI providers; evaluation frameworks and datasets | 41 inspected |
| `2026-09-19-stage-11b-legal-data-sources.md` (`K-`) | Legislation, case law and citators, regulators, trade mark / design / patent registries, company registries, licence reference data | 53 rows, about 75 URLs and endpoints |
| `2026-09-19-stage-11c-legal-tooling.md` (`L-`) | Redlining; document parsing and clause extraction; citation verification; licence scanners and SBOM; privacy and data mapping; policy tooling; secret and personal-data detection | 57 rows, about 70 repositories and pages; two local tests on public or synthetic input |

All sixteen capability categories named in bootstrap §17 are covered. **Every fact below is valid only as of 19 September 2026.** Repository activity, licences and access terms change.

---

## 1. Method and limits

1. Three research agents worked under one written brief. They were told to read raw text, use the GitHub API, or make live keyless calls, because the fetch tool had produced invented and reversed content in Stage 4. None used a model-written fetch summary.
2. Nothing was signed up for. No API key was used. No confidential data was sent anywhere.
3. A usage limit interrupted all three agents; they resumed with context intact.
4. Main-session checks (19 September 2026):

| Claim | Check | Result |
| --- | --- | --- |
| `anthropics/claude-for-legal` exists; Apache-2.0; about 9.5k stars | GitHub API | Confirmed: created 21 April 2026; pushed 21 August 2026; 9,477 stars; practice-area folders at top level |
| Open Justice Licence needs a separate licence for computational analysis | Raw text of the licence page | Confirmed: "additional permission (a separate licence) for computational analysis of Find Case Law judgments (including indexing by search engines)". The linked page that defines the term was **not** read by the main session. |
| `legislation/legislation-mcp-ts` exists under a verified National Archives organisation | GitHub API | Confirmed: organisation "Legislation at The National Archives", verified; created 27 February 2026; pushed 28 August 2026; 6 stars. **GitHub reports the licence as `NOASSERTION`**; stream L read it as Open Government Licence from the repository text. Treat the licence as "stated OGL, not machine-detected". |
| `JSv4/Python-Redlines` exists; MIT | GitHub API | Confirmed: MIT; pushed 6 September 2026; 129 stars |

5. Not done: commercial products were assessed at headline level only and several vendor rows rest on search summaries (marked † in log a). LibreOffice and pandoc were not installed, so those routes were read about, not run. Python-Redlines was not run. `ukcite.py` in the Lawvable citation skill was not read.

---

## 2. The most important finding: a near-equivalent exists

`anthropics/claude-for-legal` (J-01 to J-08): Apache-2.0; about 151 `SKILL.md` files across twelve practice-area plugins; roughly twenty MCP connectors; a builder hub with a skill quality checklist.

What stream J found on reading it:

| Aspect | Finding |
| --- | --- |
| Audience | Lawyers. Legal Skills also serves founders, engineers and designers (Stage 1 §5). |
| Default law | United States. Research connectors are US-only or paid. Its own `CONNECTORS.md` lists EUR-Lex and legislation.gov.uk connectors as wanted. |
| National forks found | China, Turkey, Finland, Spain, Germany. **None for England and Wales.** |
| Not present | A record of whether each stated point of law was separately verified; as-at dating of stated law; provision-level currency; confidentiality routing; product-to-law consistency and change impact; a jurisdiction-dependent advice boundary. |
| Worth reusing (licence permits) | Source-attribution tags; a "no silent supplement" rule (do not fill gaps from model memory without saying so); freshness fields in skill front matter; the `skills-qa` checklist and trust gates. |

Classification: **ADAPT**. Consequence for later stages: Legal Skills must not rebuild practice-area coverage that already exists under a permissive licence. Its distinct ground, as evidenced so far, is the verification, currency, jurisdiction, confidentiality and product-consistency layer, proven first for England and Wales / UK. **Stage 13 must test this positioning**; it is not decided here.

Other near-equivalents:

| Project | Finding | Classification |
| --- | --- | --- |
| Lawvable `uk-citation-verification` (J-14), MIT | Graded verdicts against Find Case Law and legislation.gov.uk; coverage table; handles the Open Justice Licence; refuses to claim support or later treatment. Maps to V1 and V2. | **USE after a code read**; otherwise ADAPT |
| Lawvable `proposition-audit` (J-15) | Claim typing and salience ranking | ADAPT the typing; **not** its percentage scoring (Stage 9) |
| Lawvable registry / awesome list (J-13) | The list is CC BY-NC-ND; individual skills carry their own licences | REFERENCE; never copy the list |
| `davendra/uk-legal-skills` (J-16) | Nearest UK pack. Functional Source Licence with a bar on competing use. | REFERENCE only — code reuse is unsafe |
| Most-starred community legal pack (J-18) | No licence; no verification; false precision | **REJECT** — the pattern to avoid |
| `vercel-labs/skills` CLI and skills.sh (J-11, J-12) | The project's stated distribution channel | USE |
| `anthropics/skills` docx / pdf (J-10; L-09) | The docx skill does tracked changes, but its licence forbids copying, derivatives and redistribution | USE when the host agent provides it; never copy or adapt |

---

## 3. Accepted classifications

Full assessment fields (coverage, currency, citation behaviour, access, confidentiality, cost, composability, maintenance, limits) are in the supporting logs. This section records the decision and the condition attached to it.

### 3.1 Legislation

| Capability | Decision | Condition or limit |
| --- | --- | --- |
| legislation.gov.uk API (K-01 to K-07) | **USE** | Provision-level and point-in-time URIs; CLML and Akoma Ntoso XML; machine-readable unapplied effects; typed effects feed with an "applied" flag. Open Government Licence. A User-Agent is mandatory. Two official pages give different rate limits → use the lower. Maps one-to-one onto Stage 5 §4.3. |
| legislation.gov.uk MCP server (L-28) | **USE as a pilot** | Official organisation; exposes status, extent, unapplied effects, point-in-time text. Young, no release, licence not machine-detected. Must degrade to plain HTTP. |
| EUR-Lex HTML, ELI, CELLAR REST (K-19, K-20, K-22) | **USE** | Returned the full GDPR (807 KB) with article anchors. **Closes Stage 5 gap G8.** |
| CELLAR SPARQL (K-21) | **USE through vetted query templates** | In-force flag is machine-readable. **Trap:** entry into force and date of application return as two values of one property; a naive reader collapses them (Stage 5 §9). |
| `cyanheads/eur-lex-mcp-server` (J-25) | USE candidate — test first | Apache-2.0; pushed 16 September 2026; consolidation flags |
| EUR-Lex data dump | **REJECT** | No registry mirror (non-goal) |
| GovInfo, eCFR, Congress.gov (K-23 to K-26) | REFERENCE; USE when a US fixture needs them | GovInfo has an official MCP server in preview |

### 3.2 Case law and citators

| Capability | Decision | Condition or limit |
| --- | --- | --- |
| Find Case Law (K-08 to K-13); `ds-caselaw-utils.neutral_url` + HTTP GET (L-T1) | **USE narrowly — subject to an owner decision (§5)** | Single judgment, by citation, for the user's own matter; no bulk, no storage, no index, no vector store; attribution. Existence check works: 200 for a real judgment, 404 for an invented one. `/data.xml` gives raw XML. |
| BAILII (K-14) | **REJECT for agent access** | Terms and robots.txt forbid programmatic use. Human link target only. |
| Third-party UK case-law MCP servers (J-26 and hosted bundles) | **REJECT** | Non-commercial licence; or a hosted intermediary that adds a disclosure hop |
| ICLR case information (K-50) | REFERENCE | The one free editorial later-treatment check a **human** can do; small monthly allowance; not callable by an agent |
| Westlaw UK, Lexis+ UK, vLex Justis (K-52, K-53) | REFERENCE | **No UK citator, free or commercial, offers a public API.** Confirms Stage 4. V5 stays `qualified (no citator)` unless the user has access and reports the result. |
| CourtListener REST, citation lookup, official MCP (K-15 to K-17; J-22 to J-24) | USE for US matters only | Token needed; the user sets it up |
| eyecite (L-20; local test) | USE for US text only | **Returned nothing for UK neutral citations, law-report citations or an ECLI** |
| CJEU through EUR-Lex / CELLAR | USE | |
| UK or EU citation extractor | **None maintained.** Blackstone dead since 2021; LexNLP dead and AGPL. | A small neutral-citation pattern set is a justified native gap → Stage 13. The National Archives enrichment code is the best pattern source (L-25). |

### 3.3 Regulators

| Capability | Decision | Condition or limit |
| --- | --- | --- |
| GOV.UK Content API and Search API (K-27 to K-29) | **USE** | Gives `public_updated_at`, `change_history[]`, `withdrawn_notice` for CMA, IPO, Companies House guidance. Fills Stage 5 `currency_state` directly. |
| ICO website (K-32) | USE by direct fetch of named pages | Quote the update and "under review" block verbatim; no crawling |
| FCA Handbook API (K-30, K-31) | REFERENCE now | Behind sign-in; free; OGL. **The Instruments, not the consolidated Handbook, are the definitive text** → add to Stage 5 do-not-collapse list |
| SRA Standards (K-33) | REFERENCE | Bot wall; record `inspection_mode` |

### 3.4 Registries

| Capability | Decision | Condition or limit |
| --- | --- | --- |
| UK IPO trade mark search (K-39) | REFERENCE — human-performed lookup | **No trade mark API or bulk data.** An API is "in development", no date. The skill records what the user saw (`query_used`, `retrieved_at`). |
| EUIPO API portal (K-34) | REFERENCE now | REST APIs exist; production access needs approval; user-held credentials only |
| TMview / DesignView (K-36) | REFERENCE | Finding aid |
| WIPO Global Brand Database (K-35) | **REJECT for agent access** | Terms forbid automated queries; captcha wall |
| USPTO TSDR and Open Data Portal (K-37) | REFERENCE; USE only with the user's own key | Keys require identity verification |
| Third-party trade mark MCP servers | REFERENCE, uninspected | Do not orchestrate |
| Companies House API (K-40, K-41) | USE with a user-supplied key | Free; 600 requests per 5 minutes. Accuracy policy read at source → **closes Stage 5 gap G3**. No-key fallback: the public web service for single look-ups. |
| GLEIF LEI API (K-43) | **USE** | Keyless; CC0 |
| OpenCorporates; EU BRIS; EPO OPS | REFERENCE | |

Consequence: the Stage 7 trade mark knockout screen is **mostly human-performed** in the UK and at WIPO today. The skill structures the search, records dated evidence and triages. It does not query those registers itself.

### 3.5 Redlining and document comparison

| Capability | Decision | Condition or limit |
| --- | --- | --- |
| Python-Redlines with the Docxodus engine (L-01, L-02) | **USE** | The only open, local tool found that writes a real Word tracked-changes file from two .docx files. MIT. One effective maintainer; v1.0.0 (6 September 2026) changed the comparison algorithm → **pin the version**. Not run in this stage. **Never use its hosted demo for real documents.** |
| pandoc `--track-changes` (L-08) | **USE, with a hard rule** | pandoc's default when reading .docx is `accept`, which **silently drops a counterparty's deletions and comments**. Always `--track-changes=all`. |
| `houfu/redlines` (L-04); git `--word-diff` (L-11) | USE | Text and Markdown change lists; change detection for Stage 8 |
| LibreOffice headless compare (L-10) | REJECT for now | No command-line compare flag found; unproven |
| Draftable, Litera and similar | REFERENCE | What firms already have |

### 3.6 Parsing and clause extraction

| Capability | Decision | Condition or limit |
| --- | --- | --- |
| Docling (L-12) | **USE** | Default local parser for PDFs and scans |
| pdfplumber / pypdf (L-14, L-15) | USE | Born-digital PDFs; page pinpoints |
| marker (L-17) | **REJECT as default** | Model weights free only under a funding or revenue cap |
| LexNLP; Blackstone (L-18, L-19) | REJECT as dependencies | Unmaintained; LexNLP is AGPL |
| CUAD 41-category taxonomy and dataset (L-21; J-33) | **ADAPT** | CC BY 4.0. Review-checklist seed and public fixture material |
| Unstructured; Tika | REFERENCE | One parser is enough |

### 3.7 Licence scanning and SBOM

| Capability | Decision | Condition or limit |
| --- | --- | --- |
| ScanCode Toolkit (L-30) | **USE** | File-level licence evidence. Output is a finding aid (Stage 5 §4.2). |
| Syft (L-36) | **USE** | Dependency inventory; SPDX and CycloneDX output |
| REUSE tool (L-35) | USE | This repository's own hygiene; outbound-licensing check |
| SPDX licence list data; OSI API (K-45, K-46; L-41) | **USE** | Pin the list version |
| deps.dev; ClearlyDefined (K-47, K-48) | USE / REFERENCE as finding aids only | They **disagree** on a well-known package's licence (`CC0-1.0 AND MIT` vs `MIT`). Disagreement is itself a finding. |
| pip-licenses (maintained fork) | USE as a first pass | |
| Trivy (L-38) | REFERENCE | **Telemetry on by default.** Do not adopt its severity labels as legal risk. |
| ORT; FOSSology; FOSSA; Snyk | REFERENCE | Too heavy to be a skill step, or commercial |
| askalono | REJECT | Archived |

### 3.8 Privacy and data mapping

| Capability | Decision | Condition or limit |
| --- | --- | --- |
| ICO ROPA and DPIA templates (L-45 to L-47) | **ADAPT** | OGL v3.0. Take the column set as the data-flow inventory shape and the step structure for DPIA screening. Attribute the ICO; link to the live page. **Not checked** whether the templates reflect the Data (Use and Access) Act 2025. |
| Data inventory from code (approach) | ADAPT as a skill step | No tool dependency |
| Ethyca Fides (L-42) | **REJECT** | Archived (date from a search snippet only); a platform is out of scope |
| Fideslang taxonomy; Privado | REFERENCE | |
| OneTrust, TrustArc, DataGrail | REFERENCE | |

### 3.9 Policy and compliance tooling

Open Policy Agent, NIST OSCAL, compliance-as-code projects: **REFERENCE only.** The project guardrail against a universal policy-as-code engine stands.

### 3.10 Secret and personal-data detection (Stage 10 routing)

| Capability | Decision | Condition or limit |
| --- | --- | --- |
| Gitleaks (L-51) | **USE now** | Local, MIT, no network. Feature-frozen; its author moved to a successor with optional HTTP validation → re-evaluate later, validation off. |
| TruffleHog (L-53); detect-secrets (L-54) | **REJECT as the default**; detect-secrets as second opinion with `--no-verify` | They **verify found secrets over the network by default**, which breaks Stage 10 class 7 |
| Presidio (L-55) | USE as an optional local helper for redaction | A second check after human-directed redaction; **never the gate**. MIT; UK recognisers; now under a different organisation. |
| scrubadub | REJECT | Unmaintained |

### 3.11 Legal AI providers and connectors

All **REFERENCE**: Thomson Reuters CoCounsel / Westlaw AI; Lexis+ AI / Protégé; Harvey; vLex Vincent; Juro; Ironclad; Definely; Spellbook; Luminance; LegalOn. Rows marked † in log a were not inspected at the vendor's own pages. Robin AI: **REJECT** — not a going concern. Lesson recorded: never hard-wire a vendor. Independent evaluations cover US law only and vendors opt in; several large vendors were absent from or withdrew from the one independent multi-vendor report found (J-30, J-31).

### 3.12 Evaluation frameworks and datasets

| Capability | Decision | Use in Stage 18 |
| --- | --- | --- |
| Stanford "Hallucination-Free?" method (J-29) | **ADAPT** | Correctness × groundedness split = V1–V3 in evaluation form |
| Vals AI legal reports (J-30, J-31) | ADAPT the rubric shape | Atomic checks per reference answer; "unable to answer" as a recorded outcome |
| LegalBench-RAG (J-34) | ADAPT the method | Character-span scoring for pinpoint accuracy |
| CUAD, MAUD, ACORD (J-33) | ADAPT / REFERENCE | CC BY 4.0 public contracts as fixture inputs |
| ContractNLI | ADAPT with caution | Hypothesis + evidence-span format; **licence unresolved** |
| LexGLUE (UNFAIR-ToS, LEDGAR) | REFERENCE | Clause labels could seed consumer-terms fixtures |
| LegalBench | REFERENCE | A model benchmark; licences vary per task |
| JudgmentBench; LexRubric (J-37, J-38) | REFERENCE | Rubric-only scoring of open-ended legal work is weak → include paired comparisons; validate any model judge against human scoring |
| `skill-creator` evaluation tooling | USE | Harness layer; the legal content of fixtures is ours |

**Gap in the landscape:** no benchmark found measures currency of law, jurisdiction fit, later treatment, product consistency, escalation behaviour, confidentiality behaviour, or any England-and-Wales or EU practice task. Stage 18 must write those fixtures.

---

## 4. Access and licence traps

| Trap | Evidence | Consequence |
| --- | --- | --- |
| Open Justice Licence excludes "computational analysis", defined by the National Archives to include AI and large language models, vector databases, bulk programmatic search and building AI services. One-at-a-time download is free. | K-08 to K-13; L log; main-session check | Owner decision (§5). No storage, index or bulk in any case. |
| BAILII forbids programmatic use | K-14 | No agent access |
| WIPO Global Brand Database forbids automated queries | K-35 | No agent access |
| USPTO keys need identity verification; EUIPO production access needs approval | K-34, K-37 | User-held credentials only |
| Lawvable list is CC BY-NC-ND; one UK skills pack bars competing use; one UK case-law MCP server is non-commercial; the most-starred pack has no licence | J-13, J-16, J-18, J-26 | Check each item's own licence; never copy the list |
| Anthropic docx skill forbids copying, derivatives and redistribution | L-09 | Use it when present; never adapt it |
| marker weights are revenue-capped; LexNLP is AGPL; TruffleHog is AGPL | L-17, L-18, L-53 | Rejected as defaults |
| Secret scanners and one SBOM scanner contact the network by default | L-38, L-53, L-54 | Conflicts with Stage 10; choose local tools or disable |
| FCA: Instruments are definitive, not the consolidated Handbook | K-30, K-31 | Source-standing rule |
| Hosted demo sites for local tools | L-01 | Never for real documents |

---

## 5. Decision for the repository owner

**Question:** may a Legal Skills workflow fetch a single Find Case Law judgment, at the user's request, for that user's own matter, and have the model read it?

- The licence text allows downloading judgments one at a time as needed.
- It requires a separate (free, use-specific) licence for "computational analysis", which the National Archives defines to include using AI or large language models.
- The text does not settle whether an agent reading one judgment for one user is "computational analysis".

This is a licence interpretation with consequences for the project and its users. It is the owner's decision, not the tool's. **Stage 12 brings it forward with options.** Until it is decided, the conservative handling applies: the skill gives the user the citation and the official URL, asks the user to open it, and works from what the user supplies or confirms.

---

## 6. Gaps closed and opened

| Earlier gap | State |
| --- | --- |
| Stage 5 G3 Companies House profile | **Closed** (K-40, K-41) |
| Stage 5 G8 raw-text route for long EU acts | **Closed** (K-19 to K-22) |
| Stage 5 G4 / Stage 4: no free UK citator | **Confirmed**; no API at all, free or paid |
| Stage 5 G1 EUIPO representation rules | Still open (not in scope here) |
| Stage 5 G2 WIPO | Closed as "REJECT for agent access" |

New gaps:

| # | Gap | Bound |
| --- | --- | --- |
| N1 | Find Case Law licence interpretation | §5; Stage 12 |
| N2 | No maintained UK or EU citation extractor | Candidate native gap → Stage 13 |
| N3 | Python-Redlines, the legislation MCP server, the EUR-Lex MCP server and the Lawvable citation skill were not run or code-read | Pilot and review before any dependency → Stage 12, Stage 24 |
| N4 | Commercial providers not inspected at source | REFERENCE only |
| N5 | ICO templates not checked against the 2025 Act | Attribute and link to the live page |
| N6 | ContractNLI and per-task LegalBench licences unresolved | Do not redistribute |
| N7 | Licence of `legislation-mcp-ts` not machine-detected | Read the licence file before depending on it |

---

## 7. What the landscape means for the project

1. **Orchestrate, do not rebuild:** legislation retrieval and status (legislation.gov.uk, CELLAR), guidance currency (GOV.UK Content API), entity identity (GLEIF, Companies House), licence identification (SPDX, ScanCode, Syft), parsing (Docling), redlining (Python-Redlines, pandoc with the tracked-changes rule), secret stripping (Gitleaks).
2. **Human-performed with structured recording:** UK and WIPO trade mark searches; later treatment of cases; anything behind a login the user holds.
3. **Reuse conventions from the near-equivalent:** attribution tags, no silent supplement, freshness fields, quality checklist.
4. **Genuinely missing in the landscape**, and therefore candidate native work for Stage 13: the verification record and gates (Stage 5); provision-level currency handling; jurisdiction-dependent boundary; confidentiality routing; product-to-law consistency and change impact; controlled uncertainty language; a UK neutral-citation pattern set; England-and-Wales and EU evaluation fixtures.
5. **Never hard-wire a vendor or a young tool.** Every USE above must degrade to a plain, disclosed manual step.

---

## 8. Exit verification

| Requirement (bootstrap §17) | Where | Met |
| --- | --- | --- |
| All sixteen capability categories researched | §2, §3.1–§3.12; logs a–c | Yes |
| Each evaluated for jurisdiction coverage, authority coverage, currency, citation behaviour, confidentiality controls, cost, composability, maintenance | Supporting logs §3 (assessment fields per row) | Yes; commercial products at headline level only |
| Each classified USE / ADAPT / REFERENCE / REJECT | §2, §3 | Yes |
| Research before native infrastructure | §7 | Yes |
| **Exit: the project knows what it should orchestrate rather than rebuild** | §7 items 1–4 | Yes |
