# Stage 7 — Legal Research, Advice, Drafting and Review Workflows

**Stage:** 7 of the Legal Skills bootstrap (v1.2)  
**Date:** 19 September 2026  
**Branch:** `feat/bootstrap-3`  
**Status:** Complete — accepted input for Stage 8  
**Governing section:** §13 of `2026-09-08-legal-skills-new-project-bootstrap-process.md`  
**Inputs:** Stage 1 (zones, review points); Stage 3 capability model; Stage 4 main log and supporting logs a–g (practice evidence); Stage 5 (authority and temporal model); Stage 6 (artefacts A1–A8)

Method: each workflow family proposed in bootstrap §13 was checked step by step against the professional-practice evidence gathered in Stage 4. Evidence IDs (`A-`…`G-`) point to the Stage 4 supporting logs. Book finding IDs (`AD`, `FF`, `SC`, `-OV-`) point to the Stage 3 logs. No new external research was needed. Workflows are **work loops**, not commands; Stage 14 decides commands.

Step-type key: **D** deterministic or checkable · **G** generative · **J** judgement-heavy · **T** tool-dependent · **H** human decision.

---

## 1. Shared skeleton

Every family uses the same five moves. They exist because the evidence shows the same failures in every stream (Stage 4 §7).

| Move | What happens | Artefact (Stage 6) | Why (evidence) |
| --- | --- | --- | --- |
| S1 Frame | Plain restatement of the question; client and instruction; requested output; zone check; sensitivity; jurisdiction context with as-at date | A1 | Wrong client or scope invalidates all later work (A log M1; B log review brief; F-04); advice boundary depends on territory (F-21 to F-25) |
| S2 Ground | Build or load the domain fact base; separate facts, assumptions, unknowns; ask for missing material facts | A2 | Each stream starts from its own fact base (Stage 4 §2); template-first work is the top failure (C-F1, D-F1) |
| S3 Reason | Issues → elements → propositions with verified authority → application → conclusions in controlled language | A3, A4, A5 | FF2-01 to FF2-13; Stage 5 §6 gates; Stage 4 §4 |
| S4 Act | Requirements, drafts, redlines, consistency findings; smallest sufficient change | A6, A7 | AD3-16 to AD3-18; Stage 4 N8, N22 |
| S5 Hand over | Human review points; escalation package where triggered; delivery with as-at date, limits and sources searched | A8; A1 status | Stage 1 §7; Stage 4 N18, N19; F log memo layout |

Two sub-loops are called from several families.

### 1.1 Authority verification sub-loop

```text
candidate authority (from search, database, user, or model suggestion)
→ resolve identity and locator                                   D/T   V1
→ read the pinpoint in raw text where the point is material      T     V2   (extract-only is recorded as weaker)
→ state the proposition; test support at that level of generality J     V3
→ currency: provision-level status, banner, transitional rules,
  guidance currency state                                         D/T   V4
→ cases: appellate history and later treatment, method declared   T     V5   ("none" blocks confident wording)
→ jurisdiction and forum fit; source class and standing           D/J   V6
→ gate (Stage 5 §6) → record → reuse only after V4/V5 refresh
```

Failure → repair: a failed V1 or V3 removes the authority and re-opens only the conclusions that used it. Evidence: F-04, F-05, F-08 (misgrounded citations pass an existence check), F-33 (no free official citator), C-19, C-20, and the six observed summariser errors (Stage 4 §1).

### 1.2 Escalation sub-loop

```text
trigger fires (zone B/C; doctrinally loaded term; regulated perimeter; similar-mark assessment;
  mandatory representation; conflicting high-level authority; unresolved jurisdiction;
  departure from clear wording; request to exploit a gap; knowing non-compliance)
→ stop analysis at the trigger; keep Zone A preparatory work      D
→ choose the specialism                                          J
→ build A8: precise question, decision needed, all facts including adverse ones,
  authority table with verification states, contrary view, limits of work done   G/D
→ human sends it (sensitivity routing first)                     H
→ record the outcome: addressee, date, assumptions, question answered            D
```

Evidence: A-01, A-02, A-05 (SRA escalation ladder and records); A log M6 (instruction quality; Post Office review; FTC bar on relying on management assertions); G log M6; D-14, D-15, D-24, D-28 (perimeter); E-22, E-23 (trade mark opinion).

---

## 2. Legal advice workflow

### 2.1 Validation of the proposed sequence

| Proposed step (bootstrap §13) | Result | Evidence and change |
| --- | --- | --- |
| intake | **Kept, extended** | Add client and instruction identification, plain restatement, zone check, sensitivity (A log M1, M2; MVG-OV-09 adapted). |
| facts / assumptions | **Kept, extended** | Add the unknowns list and a request for missing material facts. The student source only reasons conditionally (FF2-10); practice asks (Stage 3 §6). |
| jurisdiction | **Kept** | Resolve per issue; record unresolved fields (Stage 5 §3). |
| issue spotting | **Kept, extended** | Party / event grid; element decomposition; completeness sweeps; flag out-of-scope issues without analysing them (FF2-03 to FF2-06 qualified). |
| research | **Kept, reordered** | Secondary overview first, then re-frame issues, then primary sources per sub-issue (FF2-07; F log §3.5). Keep a research log with nil results (Stage 4 N7). |
| authority verification | **Kept, made a named sub-loop** | §1.1. Three tests, not one (F-04, F-08). |
| application | **Kept** | Name the facts that satisfy each element; one cycle per sub-issue (FF2-02, FF2-09). Text → context → purpose → aids (F-14). |
| options / risks | **Changed** | Four separate statements; fixed ladder; non-numeric exits; no composite score (Stage 4 §4). |
| recommendation | **Kept, qualified** | The user decides. An unlawful option is named as unlawful (MVG-OV-07 qualified; A-01 to A-05). |
| review / escalation | **Kept** | §1.2. |
| valid-as-of delivery | **Kept, extended** | Answer-first layout: answer, facts / assumptions / unknowns, as-at date, sources searched, limits, next steps (F-34, F-35; FF2-01 merged). |
| — | **Added** | Counter-position search before concluding (FF2-11; SC1-18). Conclusion-change log after delivery (Stage 4 N20). |

### 2.2 Accepted loop

```text
frame (A1)                                                        G/J
→ ground: facts, assumptions, unknowns; ask for material gaps (A2) G/H
→ resolve jurisdiction per issue                                  J
→ spot issues; decompose into elements; flag out-of-scope (A3)    G/J
   ↺ cheap stop: deliver an ISSUE LIST if that resolves the uncertainty
→ plan research per element; overview first; log sources searched T
→ find candidate authorities → verification sub-loop (A4)         T/D/J
   ↺ cheap stop: deliver an AUTHORITY TABLE
→ search for the counter-position                                 T/J
→ apply: element by element, naming facts (A5)                    J
→ state requirement / outcome likelihood / exposure separately    J
→ options and recommendation; name unlawful options               J
→ check triggers → escalation sub-loop if any                     D/H
→ human review points (Stage 1 §7)                                H
→ deliver answer-first, with as-at date and limits                G
→ later: refresh V4/V5; change conclusions only on new fact,
  new authority or identified error                               D
```

Commitment points: scope accepted; material facts confirmed; reliance on a contestable reading; risk acceptance. All are human decisions.

Iteration loops: research ↔ issue framing (FF2-07); unknowns answered → re-apply; adverse authority found → revise band or escalate.

---

## 3. Drafting workflow

### 3.1 Validation

| Proposed step | Result | Evidence and change |
| --- | --- | --- |
| purpose / parties / audience | **Kept, extended** | Audience `business` or `consumer` selects the quality standard. Governing law is fixed here because it changes what words do (B-04, B-08 to B-10). |
| project facts | **Kept, strengthened** | No drafting without the fact base. Every factual statement in the draft maps to a fact row (C-05, C-07; D-01; Stage 4 N1). |
| rights / obligations | **Kept** | Expressed as requirements (A6) before clauses. |
| authority / policy constraints | **Kept, extended** | Mandatory content lists (for example pre-contract information), statutory controls on exclusions (B-01 to B-03; D log M3), house playbook, locked standards. |
| clause plan | **Kept** | The cheap representation. Each planned clause gets a function category and its sources (AD1-12, AD1-26). |
| draft | **Kept** | Category-correct language; named actor; defined-term discipline; vagueness only where chosen (AD1, AD2 findings). Locked terms untouched (Stage 4 N11). |
| clause review | **Kept** | Uncertain-meaning checks; usage checks **keyed to governing law** (Stage 4 §9, C15 condition). |
| cross-document consistency | **Kept, extended** | Includes every layer of a consumer document: summary, FAQ, journey copy, marketing (D-01; Stage 4 N3). |
| product consistency | **Kept** | Document ↔ fact base, both directions. |
| redline / revise | **Kept** | Smallest change; tracked; reasons in comments (B-39, vendor-level evidence only). |
| approval | **Kept** | Human. Approved text is then preserved. |
| — | **Added** | Consumer branch (§3.3). Execution and variation formalities as a gate (B-12; B log M3). Obligations register as an output (B-15; Stage 4 N22). |

### 3.2 Accepted loop

```text
frame: purpose, parties, audience, governing law, origin of paper (A1, A7)   J/H
→ ground: fact base rows this document must reflect (A2)                     G/H
→ requirements: what the document must and must not say or do (A6)           J
→ constraints: mandatory content, statutory controls, playbook, locked forms D/J
→ clause plan: function + sources per clause                                 G
   ↺ cheap stop: agree the CLAUSE PLAN before prose
→ draft                                                                      G
→ clause review (meaning, categories, defined terms, governing-law checks)   D/J
→ consistency: within document → across documents and layers → against facts D
→ revise by smallest change                                                  G
→ triggers? → escalation sub-loop                                            D/H
→ human approval → state = approved; text preserved                          H
→ outputs: document, clause inventory with source_refs, obligations register D
```

### 3.3 Consumer-facing branch (UK evidence)

Runs in addition to §3.2 when `audience = consumer`. Adams's rules are a clarity layer only here (Stage 4 §3.1).

```text
real user journey as the fact base (sign-up, renewal, cancellation, checkout)   H/T
→ substantive fairness review: what each term DOES (imbalance, legitimate reason,
  proportionality, exit right for trader-side discretion)                       J
→ transparency: can the average consumer understand the practical and economic
  consequences? explain reasons; layer summaries                                J/G
→ pre-contract information list for the sales channel                           D
→ prominence map: onerous, unusual and price terms → where in the journey        D/J
→ choice-architecture check of the flow (defaults, drip pricing, cancellation friction)  J
→ consistency across all layers and against the flow                            D
→ two-track consequences: private-law effect and public enforcement             J
```

Evidence: D-01 (CMA37, 22 July 2026), D-03, D-05 to D-07, D-11, D-34 to D-36. Currency note: the subscription-contract regime is enacted but prospective (Stage 5 §10.1); the branch reports it under the temporal rule and does not apply it as current law. This branch is a candidate specialisation for Stage 15. The split from Adams's rules is core.

---

## 4. Review / redlining workflow

### 4.1 Validation

| Proposed step | Result | Evidence and change |
| --- | --- | --- |
| review brief | **Kept, specified** | Side; whose paper; value and risk class; governing law; playbook; authority limits; business objective (B-16, B-39, B-40). No professional-body template was found. |
| authoritative document / version | **Kept** | Compare against the last version sent; a non-authoritative copy is a recorded limit (B-39; AD3-17). |
| clause / obligation map | **Kept** | Clause inventory with function categories; obligations view (AD1-12; B-15). |
| omissions / conflicts / ambiguity | **Kept, typed** | Six sources of uncertain meaning (AD2-01) plus omission against the requirement set and the playbook. |
| verify legal assertions | **Kept** | Verification sub-loop for any legal statement inside the document or in the other side's comments. |
| compare with product behaviour | **Kept** | Fact base ↔ clauses. |
| smallest sufficient changes | **Kept, extended** | Triage rule: raise only mismatch with the deal and real confusion risk (AD1-03); two readings matter only if each is reasonable (AD2-25); stop when change costs more than it gains (AD3-18). New mode: **do not edit — locked standard** (B-41). **Governing-law label lock** before any style edit (B-04, B-08 to B-10). |
| preserve unaffected approved text | **Kept** | Stage 6 A7 `approved` and `change_mode`. |
| re-evaluate | **Kept** | Re-run only the checks the changes can affect. |
| — | **Added** | Pre-amendment gates for signed documents: variation clause, consideration or deed, authority, third-party and guarantor consent, related documents (B-12; C(RTP)A s 2). Tracked-change honesty: every change visible (B-14). Playbook fallback / walk-away with escalation threshold (B-40). Notice and claims mechanics in the obligations view (B log M9). |

### 4.2 Accepted loop

```text
review brief (A1) + authoritative version (A7)                     H/D
→ label lock for the governing law; identify locked standards      D
→ clause inventory: function, source_refs, approved flags          G/D
   ↺ cheap stop: deliver the CLAUSE INVENTORY + issue list
→ findings: mismatch with deal or facts; uncertain meaning (typed);
  omissions vs requirements / playbook; statutory controls; formalities  D/J
→ triage: material and reasonable readings only                    J
→ verify any legal assertion relied on → verification sub-loop     T/D
→ propose smallest change per finding, with reason and rule        G
→ position vs playbook: preferred / fallback / walk-away → threshold breach → escalate   D/H
→ tracked redline + clean copy + comment per substantive change    D
→ re-evaluate changed clauses and their cross-references only      D
→ human approval; obligations register updated                     H/D
```

Limits recorded: drafting checks are verified for England and Wales only. Under other governing laws the loop still runs, the label lock is `unknown`, and doctrinally loaded terms escalate (Stage 4 G2).

---

## 5. Trade mark / brand workflow

### 5.1 Validation

| Proposed step | Result | Evidence and change |
| --- | --- | --- |
| candidate mark | **Kept, extended** | Record the exact sign, variants, and intended use. Several candidates are screened together to "narrow down" (E-23). |
| territory | **Kept** | Per right. Rights are territorial (E-09, E-20, E-21). Each office has its own representation rule (Stage 4 §5; Stage 5 G1). |
| goods / services | **Kept, strengthened** | The specification is an irreversible commitment: goods and services cannot be added after filing (E log M5). Draft from actual and planned use. |
| classification | **Kept** | Nice classes, plus **adjacent** classes for searching (E-06, E-10). |
| identical / similar search | **Changed: split in two** | Knockout screen on free registers (identical and near-identical) is automatable. A full availability search (similar marks, unregistered rights, company names, domains, marketplace use) usually needs paid databases and is outside what the tool can complete (E-20, E-22). |
| result triage | **Kept** | Separate identical from similar hits; name the dimensions screened; every similar hit is "candidate — legal assessment required" (Stage 4 §3.2). |
| similarity / conflict analysis | **Moved to Zone B** | The legal test is similarity **plus** likelihood of confusion (E-01). It is a legal evaluation, not a string match. The tool prepares; a qualified person assesses. Exception the tool may state: identical mark for identical goods on the register is a knockout (E-01 s 5(1)). |
| risk / options | **Kept, constrained** | Output never says "clear" or "available". It says what was searched, when, and what that cannot show (E log F1, F4, F7). Options: drop, modify, narrow the specification, obtain a full search and opinion. |
| professional escalation / filing handoff | **Kept, corrected** | UK: self-filing is lawful; acting as filing agent is excluded by project policy, not by statute (Stage 4 §5). USPTO: a foreign-domiciled applicant must use a US-licensed attorney. EUIPO: representation needed for non-EEA parties in proceedings other than filing — search-level evidence only. |
| — | **Added** | Dated register evidence with query and time (Stage 5 §4.6). Passing examination is not proof of no conflict (E-12). Change monitoring: new filings; opposition window (E-08). |

### 5.2 Accepted loop

```text
frame: candidate sign(s), territories, intended use, timing (A1)             H
→ ground: goods / services actually offered and planned (A2)                  H
→ draft specification and classes; note adjacent classes                     G/J
→ knockout screen per register: identical / near-identical                    T/D
   record each hit as a dated register entry (A4 register extension)
   ↺ cheap stop: candidate killed by an identical mark for identical goods
→ triage: identical | similar (candidate — legal assessment required) | none found
→ state what the screen cannot show (unregistered rights, recent filings,
  reputation marks, use, similarity as a legal evaluation)                    D
→ options (drop / modify / narrow / proceed to full search and opinion)       J
→ escalation sub-loop: trade mark attorney; mandatory representation per office   D/H
→ hand over: screen report + specification draft + dated evidence             G
→ later: re-screen before filing; watch new filings                           T
```

Step types show why this loop is mostly Zone B: the judgement-heavy steps are exactly the ones the evidence reserves for qualified people.

---

## 6. Privacy / data workflow

### 6.1 Validation

| Proposed step | Result | Evidence and change |
| --- | --- | --- |
| data-flow inventory | **Kept, confirmed as the root** | Per processing activity: data categories, subjects, purpose, basis, recipients, processors, transfers, retention, systems (C-06, C-07, C-37). All outputs derive from it. |
| roles / actors | **Kept, strengthened** | Decided from what the party does, per activity; a contract label that conflicts with the facts is a finding (C-11, C-29). For AI features: provider or deployer (C-24). |
| purposes / data categories | **Kept** | |
| legal basis / conditions | **Kept, qualified** | Chosen before processing and recorded; necessity test and three-part legitimate-interests test come from regulator guidance with a currency state; one lawful basis is UK-only (C-02, C-09, C-10, C-19, C-20). |
| sharing / transfers | **Kept** | Transfer assessment is a distinct artefact (C-12, C-21). |
| retention | **Kept** | Stated period or criteria; must match configuration (C-05). |
| rights / controls | **Kept, extended** | Includes automated-decision safeguards in force since 5 February 2026 and complaints handling from 19 June 2026 (C-18, C-19). |
| risk / DPIA questions | **Kept** | DPIA triggers and review on change; regulator method page is under review (C-08, C-13). |
| requirements | **Kept** | Use the extraction method: statement-level coverage, cross-reference closure, exceptions, definitions, ambiguity annotation with escalation (C-30 to C-32). |
| privacy artefacts | **Kept** | Notice, ROPA, DPIA, LIA, processor terms and in-product disclosures are **views of one fact base** (Stage 4 N3). |
| implementation consistency | **Kept** | Every notice statement maps to an inventory row; every row needing disclosure appears. |
| — | **Added** | Regime tagging where several regimes meet on one interface (UK transparency, UK automated decisions, EU AI Act Art 50) (C-05, C-18, C-24). Provision-level currency with transitional rules (C-19, C-20). Guidance currency state in every output (six ICO pages under review). Change triggers from product, law / guidance and third parties; tell people about new uses before processing starts (C-05, C-08). |

### 6.2 Accepted loop

```text
frame (A1): fact_base_type = data-flow inventory; territories of users        H
→ build or load inventory; missing cells become unknowns (A2)                 G/H
   ↺ cheap stop: deliver the INVENTORY with gaps marked
→ role analysis per activity                                                  J
→ regime and jurisdiction tagging per activity                                D/J
→ purposes, categories, lawful basis (recorded before processing)             J
→ sharing, transfers, retention, rights and controls                          J/D
→ DPIA screening; high-risk → DPIA questions → possible escalation            J/H
→ authorities and guidance → verification sub-loop (status banners, as-at)    T/D
→ requirements (A6) by the extraction method; ambiguity → annotate / escalate J
→ derive or review artefacts as views of the inventory (A7)                   G
→ consistency: notice ↔ inventory ↔ configuration ↔ processor terms           D
→ human review points; delivery with guidance currency state                  H/G
→ re-entry on change: product | law or guidance | third party                 D
```

---

## 7. Other families confirmed by the evidence

Bootstrap §13 says "at least". Stage 4 showed three more loops that reuse the skeleton. They are recorded so that later stages do not reinvent them. None adds a new artefact.

| Family | Shape | Boundary | Evidence |
| --- | --- | --- | --- |
| Licence and provenance review (open source, content, data) | component or asset list → licence identification (full SPDX expression, version, source of identification) → distribution model → obligations from the **licence text** → notices → compatibility → findings. Tool output is a finding aid. | Copyleft in a distributed or network-served product and incompatibility → escalate | E-37, E-38, E-43 to E-46; E log M6–M8 |
| Financial-perimeter spotting | what the feature does for the user → PERG sequence as a spot list (regulated activity? specified investment? by way of business? exclusion? promotion?) → **no conclusion** → specialist package | Always Zone B: breach of the general prohibition is criminal; PERG tells readers to take advice if in doubt | D-12 to D-16, D-19 to D-21, D-24, D-28, D-29 |
| Change-impact re-entry | trigger → changed record → dependency walk (Stage 6 §4) → bounded re-review | Defined in Stage 8 | A log M2, M4; C log M6; G-log WG-OV-09 |

Due-diligence review (B log §3.2) was **not** promoted to a core workflow: it is deal-specific and its evidence is practitioner-level. Stage 13 and Stage 15 decide.

---

## 8. Cross-family observations

| # | Observation | Consequence |
| --- | --- | --- |
| O1 | The judgement-heavy steps are where escalation triggers cluster (similarity, perimeter, fairness at the margin, departure from clear words). | Step types are a usable map of where human review belongs. |
| O2 | Every family has a **cheap stop** that may fully answer the need: issue list, authority table, clause plan, clause inventory, inventory with gaps, killed candidate. | Supports "cheapest adequate representation". Stage 14 should let each stop be a complete deliverable. |
| O3 | Verification and consistency steps are mostly deterministic or tool-dependent. | They are the natural targets for independent evaluation (Stage 18). |
| O4 | Tool dependence is real in research (citators), trade marks (paid searches) and licences (scanners). | Stage 11 and Stage 12 must say what can be done without those tools and how the limit is disclosed. |
| O5 | None of the loops generates a document before the fact base exists. | This is what separates these loops from a list of document generators. |
| O6 | Evidence for redline mechanics and for how product counsel work is vendor-level or thin (Stage 4 G9). | Those steps stay provisional. |

---

## 9. Exit verification

| Requirement (bootstrap §13) | Where | Met |
| --- | --- | --- |
| Legal advice workflow validated | §2 | Yes — 11 proposed steps checked; 2 changed; 2 added |
| Drafting workflow validated | §3 | Yes — plus a consumer branch required by the evidence |
| Review / redlining workflow validated | §4 | Yes — label lock, locked standards and amendment gates added |
| Trade mark / brand workflow validated | §5 | Yes — search split in two; similarity analysis moved to Zone B; filing handoff corrected |
| Privacy / data workflow validated | §6 | Yes — inventory confirmed as root; regime tagging, currency and change triggers added |
| Validation rests on evidence, not on the proposal | Evidence IDs in every validation table | Yes |
| Commitment points, iteration loops, failure and repair, handoffs identified | §1.1, §1.2, accepted loops, §8 | Yes |
| **Exit: credible legal work loops rather than a list of document generators** | §8 O5; every loop starts from a frame and a fact base and ends in human review | Yes |
