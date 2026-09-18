# Stage 8 — Project-to-Law Traceability and Change Impact

**Stage:** 8 of the Legal Skills bootstrap (v1.2)  
**Date:** 19 September 2026  
**Branch:** `feat/bootstrap-3`  
**Status:** Complete — accepted input for Stage 9  
**Governing section:** §14 of `2026-09-08-legal-skills-new-project-bootstrap-process.md`  
**Inputs:** Stage 4 (§3.3 WG-OV-07 adapted; §6 N1, N3, N8–N10, N24; logs a, c, d, e, g); Stage 5 (temporal contract); Stage 6 (artefacts, upstream references, repair rules); Stage 7 (change-impact re-entry); family spec `04-cross-domain-orchestration-and-integration.md` §4, §8, §9

This is a design stage. It turns the Stage 6 relationships into two usable walks: forward (behaviour to evidence) and reverse (change to bounded re-review).

---

## 1. Evidence base

| Point | Evidence | Standing |
| --- | --- | --- |
| No examined book covers traceability or change impact | Stage 3 §7 item 5 | — |
| Trace links from law to requirement must be dated; cross-references must be closed; exceptions and definitions must be carried | C-30, C-31 (requirements-engineering literature) | Supported finding (method) |
| Non-lawyers classify legal ambiguity inconsistently (Fleiss' kappa 0.0446 in one study) | C-32 | Supported finding → ambiguity is annotated and escalated, not resolved silently |
| Model-generated legal requirements: mostly correct, low coverage (16 of 61 expert requirements in one study), citations right 50–68% of the time | C-33, C-35 | Supported finding → omission and wrong citation are the measured risks |
| Regulators require documents and assessments to follow the product: records "reflect the current situation"; DPIA repeated on substantial change; people told of new uses before processing starts | C-05, C-07, C-08; A log M4 | Supported finding (UK) |
| Review gate tied to "new or modified" product behaviour | A log M2 (incl. a regulator order and one company's public description) | Practical heuristic; public evidence thin |
| Obligations also move when law, guidance or third parties move | C-19, C-23 (dates amended weeks before they applied); six ICO pages under review; C log M6 | Supported finding |
| Evidence must show that a control **operates**, with a date | Stage 4 §3.3; G log (DOJ "paper programme" test; ISO 37301 clauses read in preview) | Supported finding |
| Voluntary commitments are obligations too | G log M1 | Supported finding |
| Consumer documents must agree with the real user journey and with every summary layer | D-01; D log M4, F1, F5 | Supported finding (UK) |
| Licence obligations depend on the distribution model and the exact licence version | E log M6, M7 | Supported finding |
| Register evidence is a dated fact that goes stale | E log M2, F7 | Supported finding |
| Horizon scanning needs an owner and triggers; Legal Skills should define the re-review, not run the watch | Stage 4 §3.3 WG-OV-09 adapted | Context-dependent method |

Surfaces **not researched** in Stage 4: age / child protections; user-generated-content moderation and enforcement. The method below applies to them, but their trigger lists are provisional (§9 G1).

---

## 2. Forward trace

### 2.1 Chain

```text
project behaviour            F- (fact-base row)                      what the product or business really does
→ legal issue                I-                                      question of law raised by that behaviour
→ authority / proposition    AU-, P-  (Stage 5)                      provision-level, as-at dated, verified
→ conclusion                 C-                                      requirement statement; uncertainty kept separate
→ legal requirement          R-                                      testable; regime- and jurisdiction-tagged
→ implementation             control / code / config / process / clause (CL-)   pointer owned by the consuming project
→ acceptance evidence        dated proof that the control operates
```

Risk is a branch condition on this chain (it decides depth, DPIA, escalation). It is not the root (Stage 4 §3.3).

A shorter chain is allowed for direct extraction from a provision, where no contested analysis is needed:

```text
provision (AU- + pinpoint, source class, as-at) → obligation → F- row → R- → implementation → evidence
```

### 2.2 Link rules

| # | Rule | Reason |
| --- | --- | --- |
| L1 | Every link is stored **upstream** on the dependent record and carries `link_created_on`. | Stage 6 K4; C-30 |
| L2 | A requirement names the **provision**, not the instrument, with source class and as-at date. | Stage 5 R1, R2 |
| L3 | **Cross-reference closure:** if the provision refers to another provision, definition or schedule, that target gets its own authority record or an explicit "not followed — reason". | C-30, C-31; C-F10 |
| L4 | **Exceptions and conditions travel with the rule.** A requirement derived from a rule with an exception records the exception and the facts that decide it. | C-31 |
| L5 | **Definitions dictionary per matter:** defined statutory terms used in requirements point to their definition. | C-31; C-F11 |
| L6 | **Ambiguity is annotated, not resolved silently.** The requirement carries an open-ambiguity flag, the readings, and who must decide. Material ambiguity is an escalation trigger. | C-32; C-F13 |
| L7 | **Regime and jurisdiction tags** on every requirement. A UK-only rule never reaches EU users by default. | C-F7; Stage 4 T3 |
| L8 | A requirement whose only support is guidance is `kind: should (guidance-based)` and carries the guidance currency state. | Stage 5 §4.5 |
| L9 | Voluntary commitments enter as requirements with `voluntary: true` and a pointer to the public statement. | G log M1 |
| L10 | `acceptance_evidence: none yet` is valid and is reported as a finding. A document that exists is not evidence that a control operates. | Stage 4 §3.3 |
| L11 | Legal Skills records **pointers** to implementation and evidence. The consuming project owns the things pointed to. | Stage 1 §3.4 |

### 2.3 Coverage check

Correctness and coverage are separate quality dimensions (Stage 4 N9).

| Check | Question | Output |
| --- | --- | --- |
| Statement-level coverage | For each provision in scope, has every obligation-bearing statement produced a requirement or an explicit "not applicable — reason"? | Coverage table: provision statement → R- or reason |
| Fact-base coverage | Does every fact-base row that raises an issue reach a requirement or an explicit "no requirement — reason"? | Row table |
| Document coverage | Does every requirement owned by a legal document reach a clause, and does every factual clause reach a fact? | Two-direction table (§4) |
| Citation check | Every generated citation passes V1–V3 (Stage 5). | Verification states |

A coverage table with gaps is a valid deliverable. Silence about what was not covered is not.

---

## 3. Reverse trace: change impact

### 3.1 Change notice

The minimal input. It can come from a person, a commit, a release note, a regulator page, or a Pactwright intent.

| Field | Notes |
| --- | --- |
| `change_id`, `noticed_on`, `effective_on` | `effective_on` may be in the future (planned change). |
| `direction` | `product` / `law or guidance` / `third party` / `legal document` |
| `what_changed` | Plain statement, with a pointer (diff, page, register entry, notice). |
| `source_of_notice` and its reliability | User statement / repository / official page / third-party notice. |
| `sensitivity` | For routing (Stage 10). |

### 3.2 Procedure

```text
change notice
→ classify direction; restate plainly                                     D
→ locate the changed record(s):
     product      → new or superseded F- rows
     law/guidance → AU- records (re-run V4, V5); requirements whose `watch` names the source
     third party  → F- rows about that party; register or licence AU- records
     document     → CL- records changed outside the workflow (for example edited after approval)
→ is any material field different? (counterfactual test)                  J
     no  → record "no legal impact — reason"; stop                        ← valid outcome
     yes → continue
→ dependency walk (Stage 6 §4): collect the records that name the changed record upstream
→ re-review set = exactly those records; everything else is preserved      D
→ re-run only the steps those records need (Stage 7 loops):
     issue still raised? proposition still supported? application still true?
     requirement still right? clause still accurate? evidence still valid?
→ new issues? run issue spotting on the CHANGED facts only                 J
→ triggers? → escalation sub-loop
→ impact report; re-opened records go to `draft` with the trigger; old versions kept
→ human decisions: accept new requirements; approve changed clauses;
  for new uses of personal data: tell people BEFORE the change goes live   H
```

Stop conditions: the walk ends where a record does not name a changed record upstream. The walk never crosses matters. It never triggers regeneration of a whole document.

### 3.3 Impact report (output)

| Section | Content |
| --- | --- |
| Change | The notice, restated |
| Changed records | With before and after |
| Re-review set | Records re-opened, with the link that pulled each one in |
| Preserved | Count and statement that approved, unaffected work was not touched |
| Findings | New or changed issues, conclusions, requirements, clause findings |
| Timing | What must happen before the change takes effect (for example notice to users; new assessment; re-screen before filing) |
| Decisions needed | By whom |
| Limits | What could not be checked; as-at date |

### 3.4 Trigger catalogue

Legal Skills defines triggers and the bounded re-review. It does not run monitoring (Stage 4, WG-OV-09 adapted). Each requirement can name a `watch` source; the consuming project or its tooling decides how to watch it.

| Direction | Typical triggers | Evidence |
| --- | --- | --- |
| Product | New data category, purpose, recipient, processor, region or retention; new or changed sign-up, renewal, cancellation or pricing flow; new automated decision or AI feature; change to what an assistant says or does; new dependency or licence change; new distribution model (for example SaaS → shipped binary); new market; new brand or product name; new asset source | C-05, C-07, C-08; D-01; E log M6; A log M2 |
| Law or guidance | Commencement of a prospective provision; amendment; transitional period ending; application date moved; guidance reissued, marked under review, or withdrawn; new decision treating a relied-on case; reform proposal becoming law | C-19, C-20, C-23; D log F8; F log §3.5; E log M10 |
| Third party | Processor or sub-processor change; provider terms change; upstream licence change or relicensing; new conflicting trade mark filing; register status change; platform terms change | C-05; E-08; E log F7 |
| Legal document | Approved text edited outside the workflow; summary or FAQ layer edited alone; translation added | A log F13; D log F5 |

---

## 4. Consistency surfaces

The bootstrap names eight surfaces. Each is a pairing of a fact base with the documents and claims that must agree with it. The check always runs in **both directions**.

| Surface | Fact base | Must agree with | Direction 1: document → fact | Direction 2: fact → document | Evidence |
| --- | --- | --- | --- | --- | --- |
| Privacy / data | Data-flow inventory; configuration | Notice, ROPA, DPIA, LIA, processor terms, in-product disclosures | Every statement maps to an inventory row | Every row needing disclosure appears | C-05, C-07; Stage 4 N3 |
| Consumer terms / commercial flows | Real user journey; pricing and billing configuration | Terms, pre-contract information, summaries, FAQs, marketing | Every right, fee, renewal and cancellation statement matches the flow | Every fee, default and friction in the flow is disclosed with the right prominence | D-01; D log M4, M5 |
| Disclosures / UI | Actual interface copy and behaviour | Legal terms and notices | Interface copy does not contradict the terms | Required disclosures appear where the decision is made | D log M5, M6 |
| Licence obligations / dependencies / assets | Component list with versions; asset provenance records; distribution model | Notices file, attribution, licence statements, asset credits | Every notice matches a component and its licence text | Every component and asset with an obligation is covered | E log M1, M6, M7 |
| Trade mark claims / registry evidence | Dated register entries; actual use of ® and ™; ownership records | Brand statements, footers, marketing | Every registration claim matches a current register entry in that territory | Every mark in use has a recorded status | E log M2, F7 |
| AI disclosures / actual AI use | What the system does; where generated or automated output reaches users | AI disclosures, automated-decision information, terms | Disclosure matches behaviour, per regime | Every AI interaction or automated decision that needs disclosure has one | C-18, C-24; D log M9 |
| Age / child protections | Actual age gates, defaults and data use for young users | Terms, notices, policy statements | **Provisional — not researched in Stage 4** | Same | §9 G1 |
| UGC moderation / enforcement | Actual moderation capability, tooling and response times | UGC terms, community rules, takedown statements | Terms promise only what the project can do | Enforcement actions taken have a basis in the terms | **Provisional — not researched in Stage 4**; §9 G1 |

Finding types: `document says X, product does Y` · `product does Z, not disclosed` · `layers disagree` · `claim rests on stale evidence` · `promise exceeds capability` · `UK-only rule applied to other users`.

---

## 5. Pactwright interface (optional)

Pactwright's lifecycle, as described in its own README on 19 September 2026: intent → decision → contract → brief → evidence, recorded as nodes and edges. Legal Skills works without Pactwright (family principle "standalone first"). When Pactwright is present:

| Pactwright step | Legal Skills supplies | Legal Skills does not do |
| --- | --- | --- |
| Intent | A change notice can be derived from the intent (§3.1) | Record or interpret intents |
| Proposing and approving a contract | Legal requirements and constraints (A6) relevant to the change; open decisions; escalation needs; timing constraints (for example notice before go-live) | Draft or approve the Pactwright contract; choose among alternatives |
| Brief | Requirement IDs and owner domains that the brief should cover | Write the brief |
| Review | Consistency findings for the delivered change (§4); clause findings | Record review results in the project graph |
| Evidence | Which acceptance evidence each legal requirement needs; verification inputs (authority records with as-at dates) | Define evidence semantics; create evidence nodes |
| Lifecycle gates | A statement of open legal items: unresolved requirements, pending human decisions, escalations | Operate or define gates |

Pactwright owns lifecycle, contracts, evidence semantics and the project graph. Legal Skills owns legal-production semantics. No Legal Skills artefact is a Pactwright node type. A future `integrations/pactwright.yml` may declare compatibility and capability bindings only (family spec 04 §9); Stage 26 decides.

---

## 6. Handoffs to other Production Skills

Recorded as **hypotheses**. They are not promoted to family contracts (family spec 04 §4, §7; Stage 21 and Stage 27 decide).

| Producing → consuming | Minimum information | Authority over changes | Integration check |
| --- | --- | --- | --- |
| Legal Skills → Software Engineering | Requirement (A6): statement, kind, regime, applies-to, acceptance evidence needed | Legal Skills changes the requirement; engineering owns the implementation | Evidence that the control operates |
| Software Engineering → Legal Skills | Fact-base rows: data flows, configuration, dependency manifest, change notices | Engineering owns the facts | Legal Skills reports rows it could not use |
| Legal Skills → UI/UX | Disclosure and prominence requirements; wording constraints; placement in the journey | UI/UX owns the design | Interface copy checked against terms (§4) |
| UI/UX → Legal Skills | Actual journey and interface copy | UI/UX | — |
| Legal Skills → Video / Narrative / Music / Game Development | Licence, provenance, likeness and brand constraints per asset | Creative domain owns the asset | Provenance record complete |
| Creative domains → Legal Skills | Asset provenance records; reference sources; licences relied on | Creative domain | — |
| Deep Research → Legal Skills | General evidence with provenance | Deep Research | Legal Skills re-verifies anything used as legal authority (Stage 5 gates) |

---

## 7. Guardrails

| Not built | Reason |
| --- | --- |
| A monitoring or regulatory-change service | Non-goal; triggers and `watch` pointers only |
| A persistent cross-project requirement store | Matters live in consuming projects |
| A universal compliance ontology or control library | Bootstrap §19; a reusable requirement library is left to consuming projects (A log M3) |
| Automatic regeneration of documents on change | Violates smallest-responsible-unit repair |
| Automatic acceptance of "no impact" | "No legal impact" needs a stated reason and stays a human-reviewable outcome |
| Compliance certification | Stage 1 non-goal; only an audit certifies (Stage 4, WG-OV-11) |

---

## 8. Worked example (synthetic)

The legal content is illustrative and is not a statement of law. It continues Stage 6 §7.

**Forward.** `F-007` (analytics to Processor X, 26 months) → `I-003` → `P-006` (`AU-005`, `AU-004`) → `C-008` → `R-009` (notice equals configured retention) → `CL-014` and a configuration control → acceptance evidence: dated export of the retention setting.

**Product change.** Notice: "From 1 November, crash reports also go to Processor Y in another region."

```text
direction: product; effective_on 2026-11-01
→ new rows F-020 (crash data → Processor Y), F-021 (region)      U-005: what data is in a crash report?
→ material? yes (new recipient, possible transfer)
→ walk: nothing upstream names F-020 yet → issue spotting on the CHANGED facts only:
     I-010 recipient disclosure; I-011 transfer; I-012 processor terms
→ re-review set: CL-009 (recipients clause), the processor list, the transfer assessment
→ preserved: CL-014 and 31 other approved clauses; AU-004, AU-005, P-006
→ timing: people are told about the new use BEFORE 1 November
→ decisions: accept R-015 (disclose Processor Y), R-016 (transfer assessment before go-live)
```

**Law or guidance change.** The guidance page behind `AU-004` changes from "under review" to "updated on (date)".

```text
direction: law or guidance
→ AU-004 re-runs V4; the text relied on is compared
→ unchanged in substance → P-006 stays; C-008 confidence_in_analysis may rise; no clause re-opened
→ changed in substance  → P-006 re-opened → C-008 → R-009 → CL-014 only
```

**No-impact outcome.** Notice: "We renamed an internal analytics table." Counterfactual test: no material field differs. Record "no legal impact — internal naming only"; stop.

---

## 9. Bounded gaps

| # | Gap | Bound |
| --- | --- | --- |
| G1 | Age / child protections and UGC moderation were not researched in Stage 4 | Their rows in §4 are provisional. Stage 15 (catalogue), Stage 16 and Stage 17 must research them before any example or pack relies on them. |
| G2 | Public evidence on real product-counsel review gates is thin | The "new or modified" gate is a practical heuristic |
| G3 | No measured accuracy for change-impact walks | Stage 18 builds fixtures |
| G4 | Extraction accuracy figures come from single studies on specific regulations | Used only to justify separate coverage and citation checks |

---

## 10. Exit verification

| Requirement (bootstrap §14) | Where | Met |
| --- | --- | --- |
| Forward direction: behaviour → issue → authority / proposition → requirement / risk → implementation / process / document → acceptance evidence | §2 | Yes |
| Reverse direction: change → changed facts → affected issues / requirements → affected implementation → affected documents → targeted re-review | §3 | Yes |
| The eight consistency surfaces addressed | §4 | Yes — six evidenced; two provisional with a bounded gap |
| Pactwright boundary respected | §5 | Yes |
| **Exit: legal analysis can drive production changes, and later product changes can trigger bounded legal re-review** | §2 (requirements with owner domains and acceptance evidence); §3.2 stop conditions; §8 | Yes |
| Over-engineering guardrails | §7 | Yes |
