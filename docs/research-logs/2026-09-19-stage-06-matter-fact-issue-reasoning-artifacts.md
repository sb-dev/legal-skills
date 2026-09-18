# Stage 6 — Matter, Fact, Issue and Legal-Reasoning Artefacts

**Stage:** 6 of the Legal Skills bootstrap (v1.2)  
**Date:** 19 September 2026  
**Branch:** `feat/bootstrap-3`  
**Status:** Complete — accepted input for Stage 7  
**Governing section:** §12 of `2026-09-08-legal-skills-new-project-bootstrap-process.md`  
**Inputs:** Stage 1 (§3.2 owned outcomes, §7 review points, §8 quality); Stage 3 (C1–C21); Stage 4 (§4 controlled language, §6 N1–N27, §7 failure taxonomy, §9 model); Stage 5 (jurisdiction context, authority record, proposition record, verification, temporal contract)

This is a design stage. No new external research was needed. Every design choice below cites the evidence that justifies it. The family project contract leaves artefacts domain-owned (`02-production-skills-project-contract.md` §2 item 9), so no family schema constrains this stage.

---

## 1. Design constraints

| # | Constraint | Source |
| --- | --- | --- |
| K1 | Artefacts live in the **consuming project**, not in Legal Skills. Legal Skills defines their shape and rules only. | Stage 1 §3.4; family spec 04 §2 |
| K2 | **Cheapest adequate representation.** Each artefact has a minimal form. A fuller form is used only when the uncertainty justifies it. | Bootstrap §4 |
| K3 | **Plain files.** Markdown with a small field block. Identifiers are local to the matter. No database, no graph store, no universal ontology. | Bootstrap §12, §19 |
| K4 | **Relationships are ID references in one direction plus a derived reverse view.** An auditor can walk the chain by reading files. | Bootstrap §12 exit |
| K5 | **Separate what must fail separately:** fact, assumption, issue, authority, proposition, application, conclusion, requirement, document state. | Stage 1 §8; Stage 5 R3 |
| K6 | **Every record is dated**, and records that depend on law carry an as-at date. | Stage 5 §7 |
| K7 | **States are explicit.** "Verified" and "approved" are recorded events with a date and an actor. They are never inferred. | Stage 1 §7; Stage 4 N19 |
| K8 | **Repair the smallest responsible unit** and re-open only dependents. | Bootstrap §4; AD3-16 to AD3-18; Stage 5 §7.1(6) |
| K9 | **Nothing confidential by default in shared fixtures.** Sensitivity is a field on the matter, consumed by Stage 10 routing. | Bootstrap §4, §16 |

---

## 2. Artefact set

Eight artefacts, as the bootstrap requires. The authority record and proposition record were defined in Stage 5 and are reused unchanged.

```text
A1 matter brief
A2 fact / assumption record            (includes the domain fact base)
A3 legal issue
A4 legal proposition + authority       (Stage 5 §4, §5, §6)
A5 legal conclusion / risk item
A6 legal requirement / project constraint
A7 legal document / clause state
A8 escalation package
```

Identifier convention (local to a matter): `M-` matter, `F-` fact, `AS-` assumption, `U-` unknown, `I-` issue, `AU-` authority, `P-` proposition, `C-` conclusion, `R-` requirement, `D-` document, `CL-` clause, `E-` escalation. Example: `M-001/F-012`.

### A1 — Matter brief

Purpose: fix the question before work starts. It is the cheapest artefact and it is always produced.

| Field | Required | Notes |
| --- | --- | --- |
| `matter_id`, `title`, `opened_on` | Yes | |
| `question_presented` | Yes | In plain words. Euphemistic briefs are restated plainly (MVG-OV-09, adapted). |
| `client_and_instruction` | Yes | Which entity the work is for; who instructs; with what authority (Stage 4 N2). For a solo founder this is one line. |
| `requested_output` | Yes | Advice note / issue list / authority table / draft / review / consistency check / change-impact check / escalation package. |
| `jurisdiction_context` | Yes | The Stage 5 §3 record, including `analysis_as_at` and `resolution_status`. |
| `scope_in` / `scope_out` | Yes | Out-of-scope issues that are noticed are **flagged, not analysed** (Stage 3 §6, FF2-06 qualified). |
| `zone_check` | Yes | Stage 1 §4 zone per requested activity, with the reason. |
| `sensitivity` | Yes | `public` / `confidential` / `personal data` / `possibly privileged` / `unknown`. Feeds Stage 10. |
| `fact_base_type` | Yes | Which domain fact base the matter needs: data-flow inventory / user journey / provenance chain / component list / deal terms / none (Stage 4 N1). |
| `review_points` | Yes | Which Stage 1 §7 decisions apply, and who decides. |
| `research_log` | Grows | Sources searched, queries, nil results, blocked sources, tools used and their inspection mode (Stage 4 N7, N12). |
| `status` | Yes | `scoped` → `in analysis` → `delivered (as-at date)` → `stale` → `refreshed` / `closed`. |

### A2 — Fact / assumption record

Purpose: keep what is known apart from what is assumed and what is missing.

Three record kinds share one table.

| Field | Fact `F-` | Assumption `AS-` | Unknown `U-` |
| --- | --- | --- | --- |
| `statement` | One fact | One assumed fact | The missing fact, as a question |
| `source` | Who or what supplied it: user statement / document / code or config / observed behaviour / register entry / third party | Why it is reasonable | Who could answer |
| `source_date` and `recorded_on` | Yes | Yes | Yes |
| `confidence_in_source` | `confirmed` / `stated, unverified` / `contested` | — | — |
| `materiality` | Result of the counterfactual test: would a different value change an issue or conclusion? (FF1-22, FF2-22) | Same | Same |
| `used_by` | Issue and conclusion IDs (derived view) | Same | Same |
| `status` | `current` / `superseded by F-…` | `open` / `confirmed → becomes F-…` / `falsified` | `open` / `answered → F-…` |

Rules:

1. **An assumption believed or suspected to be untrue is not allowed** (Stage 4, FF2-13 extended; G-F7).
2. A **label is not a fact**. "We are a processor" is a claim; the fact is what the party actually does (Stage 4 N2; C-F2).
3. A user's claimed status ("I am a solicitor") is a fact about the user. It is never support for a legal proposition (Stage 4 N20).
4. **Empirical premises** used in reasoning ("users read the summary") are recorded as assumptions with a source or as unknowns (SC2-23).
5. **Domain fact base.** When `fact_base_type` is set, facts are held as rows of that base, for example one row per processing activity or per component. Each row is a fact record with the extra columns the domain needs. Missing cells are `U-` records. The row set is the single source for every derived document (Stage 4 N1, N3).

### A3 — Legal issue

Purpose: a question of law raised by specific facts.

| Field | Required | Notes |
| --- | --- | --- |
| `issue_id`, `question` | Yes | One question. |
| `raised_by` | Yes | Fact, assumption or unknown IDs. An issue with no fact link is a template artefact and is rejected. |
| `why_spotted` | Yes | The reason in one or two lines; optionally the sweep that found it (party / event grid; five-category sweep; conduct / fairness prompt). |
| `legal_area` and `regime` | Yes | Regimes are tagged separately when several apply to one interface (Stage 4 M7 in log c). |
| `elements` | When analysed | Sub-issues, each needing its own rule–application–conclusion cycle (FF2-02, FF2-04). |
| `jurisdiction_override` | When different from the matter | |
| `zone` | Yes | A / B / C for this issue. |
| `disposition` | Yes | `analyse` / `flag only (out of scope)` / `escalate` / `parked (needs U-…)`. |
| `priority` | Optional | By materiality to the requested output, not by a risk score. |

### A4 — Legal proposition + authority

Defined in Stage 5 (§4 authority record; §5 proposition record; §6 verification V1–V6 and gates). Stage 6 adds only the link rules:

1. A proposition belongs to one issue element. One authority may support many propositions.
2. Authority records are **shared within a matter** and may be reused across matters only after V4 and V5 are re-run (Stage 5 §7.1).
3. The minimal form is an **authority table**: one row per authority with citation, source class, pinpoint, proposition supported, as-at date and V1–V6. This is the "authority table before polished advice" of bootstrap §4.

### A5 — Legal conclusion / risk item

Purpose: the application of propositions to facts, and what follows.

| Field | Required | Notes |
| --- | --- | --- |
| `conclusion_id`, `issue_ref`, `element_ref` | Yes | One per element; roll-ups at issue and matter level (FF2-13). |
| `application` | Yes | Names the specific facts that satisfy or fail each requirement of the rule. "On the facts, satisfied" is rejected (FF2-09). |
| `propositions_used`, `facts_used`, `assumptions_used` | Yes | IDs. |
| `counter_position` | When one exists | With authority. Not invented where none exists (FF2-11). |
| **`requirement_statement`** | Yes | What the law requires on these facts. If clear, it is stated as a requirement with no likelihood term (Stage 4 §4 items 1–2). |
| **`outcome_likelihood`** | When uncertain | A band from the fixed ladder with its range and its stated basis; or `cannot be banded`; or `unclear pending …` (Stage 4 §4 items 3–5). |
| **`exposure`** | When relevant | Consequences if wrong, in kind, not as a score. Two tracks where they differ: private-law effect and public enforcement (Stage 4, D log M8). |
| **`enforcement_likelihood`** | Only on request | Labelled "not a statement of law". Never used to soften the requirement (Stage 4 §4 item 1). |
| `confidence_in_analysis` | Yes | `high` / `moderate` / `low` over source base, verification status and stability of the law. Separate from likelihood. |
| `contingencies` | When any | Each typed `assumption (fact)` or `qualification (law)`. |
| `risk_cause_tag` | Optional | `not known` / `misunderstood` / `law unclear` / `known and not followed` — selects the control. The last value is a recorded human decision and an escalation item, not a rated risk (Stage 4 §3.3, WG-OV-01 adapted). |
| `options` and `recommendation` | When advice is the output | Lawful alternatives. An unlawful option is named as unlawful and is not listed as a neutral choice (MVG-OV-07 qualified). |
| `as_at`, `status` | Yes | `draft` → `verified (all gates met)` → `delivered` → `stale` / `superseded`. |
| `change_log` | Grows | Every change of conclusion states its cause: `new fact` / `new authority` / `identified reasoning error`. Bare disagreement is not a cause (Stage 4 N20). |

No composite score exists on this artefact or on the matter (Stage 4 §4 item 7).

### A6 — Legal requirement / project constraint

Purpose: what the consuming project must do, may not do, or must be able to show.

| Field | Required | Notes |
| --- | --- | --- |
| `requirement_id`, `statement` | Yes | Testable. One obligation per record. |
| `kind` | Yes | `must` / `must not` / `must be able to evidence` / `should (guidance-based)` / `decision needed`. |
| `derived_from` | Yes | Conclusion ID, or for direct extraction: provision (authority ID + pinpoint), source class, as-at date, interpretation note, open-ambiguity flag (Stage 4 N8). |
| `regime` and `jurisdiction` | Yes | So that a UK-only rule is not applied to EU users (Stage 4 T3). |
| `applies_to` | Yes | Fact-base rows, product surface, document or process. |
| `owner_domain` | Yes | Engineering / design / content / operations / commercial / legal document. This is the handoff (Stage 1 §9). |
| `implemented_by` | When known | Pointer supplied by the consuming project: control, code, configuration, process, clause. |
| `acceptance_evidence` | When known | **Dated evidence that the control operates**, not only that it exists (Stage 4, WG-OV-07 adapted). `none yet` is a valid value and is a finding. |
| `voluntary` | Flag | True for public promises, codes and policies the project has adopted (Stage 4 N24). |
| `watch` | Optional | The source whose change would re-open this requirement, with its as-at date (Stage 4, WG-OV-09 adapted). |
| `link_created_on`, `status` | Yes | `proposed` → `accepted by project` → `implemented` → `evidenced` → `re-open (trigger …)`. |

Accepted chain (Stage 4 §3.3):

```text
provision (as-at, source class) → obligation → product fact (fact-base row)
→ requirement → control / implementation → operating evidence
```

Risk is a branch condition on this chain, not its root.

### A7 — Legal document / clause state

Purpose: know what each document says, where each statement comes from, and what state it is in.

Document level:

| Field | Notes |
| --- | --- |
| `document_id`, `title`, `type`, `audience` | Audience `business` or `consumer` selects the review standard (Stage 4 §3.1). |
| `governing_law` | Drives the label lock (Stage 4 N11). `none stated` and `unresolved` are valid. |
| `authoritative_version` | File, version, date, and how it was obtained. Review of a non-authoritative copy is a recorded limit. |
| `origin` | Own paper / other side's paper / market or community standard (`locked: yes`) (Stage 4 N11, B-M7). |
| `layers` | For consumer documents: full terms, summary, FAQ, journey copy, marketing. Each is a view that must agree with the others (Stage 4 N3). |
| `state` | `draft` → `reviewed` → `approved (by, on)` → `published / signed (on)` → `under change` → `superseded`. |

Clause level (the minimal form is a **clause inventory**):

| Field | Notes |
| --- | --- |
| `clause_id`, `location`, `function` | Function uses the category taxonomy: obligation, discretion, prohibition, condition, policy, declaration, performance (AD1-12), or for notices: statement of fact about processing, right, contact, and so on. |
| `source_refs` | Requirement IDs and fact IDs that this clause implements or states. A factual statement with no fact link is a finding. |
| `locked_terms` | Doctrinally loaded words that must not be restyled under the governing law. |
| `findings` | Each with type (uncertain-meaning class; consistency; fairness; transparency; prominence; formalities), competing readings where relevant, proposed repair, and the rule relied on (AD3-17). |
| `approved` | `yes (by, on)` / `no`. **Approved text is preserved** unless a finding or a change trigger names it. |
| `change_mode` | `leave` / `smallest change` / `replace clause` / `do not edit — locked standard` (AD3-18; Stage 4 §3.1). |

Derived view: an **obligations register** (who, what, when, trigger, notice, consequence) is generated from clause records. It is a view, not a ninth artefact (Stage 4 N22).

### A8 — Escalation package

Purpose: make specialist review efficient and honest.

| Field | Required | Notes |
| --- | --- | --- |
| `escalation_id`, `trigger` | Yes | Which rule fired: Zone B or C; conflicting high-level authority; unresolved jurisdiction; departure from clear wording; doctrinally loaded term; regulated perimeter; similar-mark assessment; mandatory representation; request to exploit a gap; knowing non-compliance. |
| `specialist_type` | Yes | The right specialism for the question (Stage 4 N18). |
| `question_for_specialist` | Yes | Precise. Not framed to obtain a preferred answer. |
| `decision_required` and `by_when` | Yes | |
| `facts`, `assumptions`, `unknowns` | Yes | **Including adverse facts and documents.** Nothing is withheld to improve the answer (Stage 4 N18; MVG-OV-06). |
| `jurisdiction_context` | Yes | |
| `authorities` and `analysis_so_far` | Yes | Authority table with verification states; the contrary view. |
| `options` | Yes | |
| `limits_of_work_done` | Yes | What was not checked; tools and inspection modes used. |
| `sensitivity_and_routing` | Yes | From A1; privilege note where relevant (Stage 4 N21). |
| `outcome` | Later | What the specialist said, to whom it was addressed, its date, its assumptions and the question it answered — so that "counsel cleared it" can be verified later (Stage 4, G log M6). |

---

## 3. Relationships

```text
M (matter brief)
 ├─ F / AS / U  (facts, assumptions, unknowns; domain fact-base rows)
 │     └─ raise → I (issue) → elements
 │                    └─ P (proposition) ── supported by ─→ AU (authority)
 │                    └─ C (conclusion)  ── uses ─→ P, F, AS
 │                           ├─ → R (requirement) ── applies to ─→ F rows / surfaces
 │                           │        ├─ implemented by → control / code / process / CL
 │                           │        └─ evidenced by   → acceptance evidence (dated)
 │                           └─ → E (escalation package)
 └─ D (document) → CL (clauses) ── source_refs ─→ R, F
```

Stored direction: each record points **upstream** to what it depends on (`raised_by`, `authority_refs`, `propositions_used`, `derived_from`, `source_refs`). Downstream views (`used_by`) are derived by reading the files. This keeps writes small and makes the dependency walk for repair simple. It is not a knowledge graph: there is no cross-matter linking, no inference and no shared ontology.

---

## 4. Repair and change rules

| Event | Smallest responsible unit | What is re-opened | What is preserved |
| --- | --- | --- | --- |
| A fact is corrected or superseded | The `F-` record | Issues it raised; conclusions and requirements that list it; clauses whose `source_refs` include it | Everything else, including verified authorities |
| An assumption is falsified | The `AS-` record | Same walk as a fact | Same |
| An authority fails V1 or V3 | The `AU-` / `P-` record | Conclusions that used the proposition | Other propositions; facts; unaffected clauses |
| An authority becomes stale or changes (V4, V5) | The `AU-` record | Propositions resting on it; then only conclusions whose proposition actually changed | Same |
| A clause has a defect | The `CL-` record | That clause; cross-references to it; its row in the obligations view | Approved clauses not named by a finding |
| The product changes | New or superseded `F-` rows | The fact walk above. This is the change-impact walk of Stage 8. | Same |
| The law or guidance changes | The `AU-` record and any `watch` that names it | Requirements with that `watch`; the authority walk | Same |
| A third party changes (processor, licence, register) | The relevant `F-` row | The fact walk | Same |
| A conclusion is challenged with no new fact, authority or error | None | Nothing. The challenge is noted in `change_log` as not a cause. | The conclusion |

A re-opened record goes to `draft` and carries the trigger. Its old version is kept.

---

## 5. Cheapest adequate form per requested output

| Requested output | Minimum artefacts | Not needed |
| --- | --- | --- |
| One bounded legal question | A1; the few A2 facts; one A3; A4 authority table; one A5 | A6, A7, A8 unless triggered |
| Issue list | A1; A2; A3 only | A4, A5 |
| Authority table | A1; A3; A4 | A5 prose |
| Review of one document | A1; A2 facts the document depends on; A7 clause inventory with findings | Full redraft |
| Drafting | A1; A2 fact base; A6 requirements; A7 | — |
| Product-consistency check | A2 fact base; A7 `source_refs`; findings | New research unless a finding needs it |
| Change-impact check | The changed records and the dependency walk | Everything not reached by the walk |
| Escalation | A8 built from what already exists | New analysis beyond the trigger |

---

## 6. What is deliberately not an artefact

| Not built | Reason |
| --- | --- |
| A central or cross-project matter store | Non-goal; consuming projects own matters (Stage 1 §3.4) |
| A universal legal knowledge graph or ontology | Bootstrap §12, §19: deferred unless implementation evidence proves the need |
| A numeric risk register or matter-level score | Stage 4 §4 |
| A jurisdiction table tree | Stage 5 R6, §7.2: dated reference data on demand |
| Copies of legislation or judgments | Stage 5 R9 |
| A separate research-log, change-log or obligations artefact | Held as sections or derived views (A1, A5, A7) to keep the set at eight |
| Domain templates (privacy notice, terms, DPIA) | Stage 7 and Stage 15 decide workflows and packs; artefacts stay domain-neutral, with a typed fact base as the only domain hook |

---

## 7. Audit walk (exit test)

**Synthetic example.** It shows that a reader can go from a project fact to authority to conclusion to action, and back. The legal content is illustrative and is not a statement of law.

```text
M-001  Question: does the app's privacy notice match what the app does with analytics data?
       Jurisdiction: UK; analysis_as_at 2026-09-19; fact_base_type: data-flow inventory

F-007  (inventory row) Analytics events are sent to Processor X and kept for 26 months.
       source: config file + processor dashboard, seen 2026-09-18; confirmed
F-011  Notice v3 (published 2026-02-01) says analytics data is kept for 12 months.
       source: authoritative published version
U-002  Is any analytics data sent outside the UK?   (who could answer: engineering)

I-003  Is the retention statement in the notice accurate and complete?
       raised_by F-007, F-011; regime: UK GDPR transparency; zone A

AU-004 [regulator guidance on privacy information] — currency_state: under review
       (banner quoted); retrieved 2026-09-18; V1 pass, V2 extract only, V3 pass, V4 qualified
AU-005 [the statutory transparency provision] — in force; banner state recorded
P-006  Privacy information must state the retention period or the criteria used to set it.
       authority_refs AU-005 (text), AU-004 (guidance); as_at 2026-09-19

C-008  application: F-011 states 12 months; F-007 shows 26 months; the notice is inaccurate.
       requirement_statement: the notice must state the real period or criteria.  (clear → no likelihood term)
       confidence_in_analysis: moderate (guidance under review; extract-only reading)
       contingency: none.  change_log: —

R-009  must: notice retention statement equals the configured retention for analytics.
       derived_from C-008; applies_to F-007 row; owner_domain: legal document + engineering
       acceptance_evidence: none yet  → finding
R-010  decision needed: keep 26 months and change the notice, or reduce retention to 12 months.
       (the user decides; both options lawful on the stated facts)

D-001/CL-014  retention clause; source_refs R-009, F-007; approved: yes (2026-02-01)
       finding: consistency; change_mode: smallest change; all other clauses: leave
```

Forward walk: `F-007 → I-003 → P-006 (AU-005, AU-004) → C-008 → R-009 → CL-014 → acceptance evidence`.  
Backward walk from the clause: `CL-014 → R-009 → C-008 → P-006 → AU-005` and `→ F-007`.  
Change test: if engineering later sets retention to 12 months, `F-007` is superseded; the walk re-opens `C-008`, `R-009`, `CL-014` only. `AU-004`, `AU-005`, `P-006` and every other clause are preserved. If the guidance page changes, `AU-004` re-runs V4; `P-006` is re-opened only if the text relied on changed.

---

## 8. Exit verification

| Requirement (bootstrap §12) | Where | Met |
| --- | --- | --- |
| Minimal durable artefacts for all eight named items | §2 A1–A8 | Yes |
| Relationship chain fact → issue → proposition → authority → analysis → conclusion / risk → requirement → implementation / document → acceptance evidence | §3; §2 A6 chain | Yes |
| No universal legal knowledge graph | §1 K3–K4; §3 last paragraph; §6 | Yes |
| **Exit: legal work can be audited from project fact to authority to conclusion to action** | §7 forward, backward and change walks | Yes |
| Consistency with accepted stages | Stage 5 records reused unchanged (A4); Stage 4 controlled language built into A5; Stage 4 missing capabilities N1–N3, N7, N8, N11, N18–N22, N24 placed in fields | Yes |
| Over-engineering check | Eight artefacts only; three items held as views; most fields conditional; minimal forms defined (§5) | Yes |
