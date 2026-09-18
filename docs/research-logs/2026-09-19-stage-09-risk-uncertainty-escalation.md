# Stage 9 — Risk, Uncertainty, Escalation and Human Review

**Stage:** 9 of the Legal Skills bootstrap (v1.2)  
**Date:** 19 September 2026  
**Branch:** `feat/bootstrap-3`  
**Status:** Complete — accepted input for Stage 10  
**Governing section:** §15 of `2026-09-08-legal-skills-new-project-bootstrap-process.md`  
**Inputs:** Stage 1 (§4 zones, §7 review points); Stage 3 (C10, C18, C20, C21; MVG-OV and WG-OV findings); Stage 4 (§3.3, §4 controlled-language position, §6 N17–N20, logs a and g); Stage 5 (verification gates, stability); Stage 6 (A5, A8); Stage 7 (§1.2 escalation sub-loop)

Stage 4 §4 handed this stage a position "to test". This log tests it against the evidence, fixes the vocabulary, and defines the triggers and review points.

---

## 1. Evidence

### 1.1 From Stage 4 (IDs point to supporting logs a and g)

| Point | Evidence | Standing |
| --- | --- | --- |
| Bare probability words are read very differently by writer and reader ("serious possibility" read as anything from about 20% to about 80%) | G-10 | Supported finding |
| Words shown with ranges work better than words alone | G-15 | Supported finding |
| Lawyers' predictions of their own case outcomes are overconfident, and experience does not fix it | G-17 (secondary report of the study; primary not inspected; figure appears as 43% and 44%) | Supported in direction; figure unverified |
| UK intelligence practice uses seven verbal bands with published ranges, and separates analytical confidence from probability | G-13, G-14; S9-02 below | Supported finding |
| England and Wales civil legal aid uses statutory numeric bands **and two non-numeric exits** | G-21; S9-01 below | Supported finding |
| US tax-opinion practice keeps the chance of audit out of the merits assessment | G-19 | Supported finding (US practice) |
| The Attorney General's legal-risk guidance (reissued 8 September 2026) uses fixed percentage bands with fixed wording; keeps merits, likelihood of challenge and impact apart; sets a floor ("no tenable argument" = unlawful); says to consider what a court would decide even if the point is unlikely to be tested | A-16, A-17 | Supported finding (government practice); not transferable as a whole to product work |
| An unanchored red rating meant "55% to one lawyer and 90% to another" | A log (2015 government predecessor guidance) | Supported finding |
| Treating law as "legal risk" can turn a boundary into a price; the interpretive question drifts under pressure | MVG-OV-03, MVG-OV-04; A-09, A-10 (authors' own reports); A-01 to A-05 (SRA in-house guidance) | Supported finding (failure mode) |
| SRA in-house guidance: client is the organisation; independence; escalation ladder; records; advice not followed is not by itself reportable; accepting a degree of legal risk can be proper; purposive loophole exploitation is a concern | A-01 to A-05 | Supported finding (E&W solicitors) |
| Opinions used as risk transfer; controls as theatre | MVG-OV-06; A log M6; G log (DOJ test; failure-to-prevent-fraud guidance) | Supported finding |
| Language models abandon correct answers under mere user doubt; worse over turns and with apparent user authority; most stance change is nevertheless toward a correct user correction; answers can flip with no change of input | G-28 to G-34, G-37 | Supported finding (general domain); **no legal-task study found** |
| One shared definition of "legal risk" does not exist: the IBA / McCormick definition excludes wilful or reckless behaviour; the four-cause wording is unverified | G log §4 WG-OV-01 | Disputed claim |

### 1.2 Stage 9 checks at primary sources (19 September 2026; fetch-tool extracts)

| ID | Source | Result |
| --- | --- | --- |
| S9-01 | Civil Legal Aid (Merits Criteria) Regulations 2013, SI 2013/104, reg 5 — https://www.legislation.gov.uk/uksi/2013/104/regulation/5 | Latest revised version. Outstanding changes listed affect reg 11 only. Categories: very good (80% or more); good (60% to less than 80%); moderate (50% to less than 60%); **borderline** (not unclear, but disputed law, fact or expert evidence prevents classing it as 50% or more, or as marginal or poor); marginal (45% to less than 50%); poor (less than 45%); **unclear** (identifiable investigations could allow a reliable estimate). |
| S9-02 | Professional Head of Intelligence Assessment, *Explaining uncertainty in UK intelligence assessment*, 24 March 2025 — gov.uk | Probability Yardstick: remote chance >0–≈5%; highly unlikely ≈10–≈20%; unlikely ≈25–≈35%; realistic possibility ≈40–<50%; likely or probable ≈55–≈75%; highly likely ≈80–≈90%; almost certain ≈95–<100%. Probability is "the likelihood that a statement is true"; analytical confidence is "the soundness and stability of the foundations" of the assessment. |

The gaps between the yardstick bands are visible in the ranges. The stated reason for them ("to avoid a false impression of accuracy") comes from G-14.

---

## 2. Result of the test

| Stage 4 §4 item | Test result | Change |
| --- | --- | --- |
| 1 Four separate statements | **Confirmed.** Two independent professional practices separate merits from enforcement (tax opinions; Attorney General's guidance). The separation answers MVG-OV-03 without banning numbers. | None |
| 2 A clear requirement is stated as a requirement | **Confirmed.** Attorney General's floor and SRA guidance both treat "unlawful" as a statement, not a rating. | Label set fixed in §4.1 |
| 3 Fixed verbal ladder with ranges | **Confirmed**, with a concrete default: the seven-band UK yardstick (S9-02). | §4.2 |
| 4 No tool-generated point percentages | **Confirmed** (G-10, G-14, G-17; model instability G-34). | None |
| 5 Two non-numeric exits | **Confirmed at primary source** (S9-01 "borderline", "unclear"). | Names fixed in §4.2 |
| 6 Confidence in the analysis is separate | **Confirmed at primary source** (S9-02). | Criteria tied to Stage 5 verification states (§4.4) |
| 7 No composite score, no single colour | **Confirmed.** Unanchored ratings are a documented failure. | None |
| 8 Conjunctive claims | **Kept as a rule of reasoning** (SC2-24; FF2-13). No empirical evidence sought. | Marked practical heuristic |

Bootstrap default "no single numeric legal-risk score" is **upheld**. Numbers are allowed only as published ranges attached to fixed words, for one statement type (§4.2).

---

## 3. Dimensions kept visible

The bootstrap lists ten candidate dimensions. All are kept. None is summed. Each has a home in a Stage 5 or Stage 6 field, and a small fixed vocabulary.

| Dimension | Home | Vocabulary | Evidence |
| --- | --- | --- | --- |
| Authority clarity | A5 `requirement_statement` label (§4.1); A4 `support_type`, `stability` | §4.1 labels | Stage 5; SC1-04 core / fringe |
| Factual uncertainty | A2 `confidence_in_source`; A5 `contingencies` (assumption) | `confirmed` / `stated, unverified` / `contested` / `unknown` | FF2-10; G log M3 |
| Jurisdiction uncertainty | A1 `resolution_status`; A4 V6 | `resolved` / `assumed` / `unresolved` / `out of proving scope` | Stage 5 §3 |
| Financial / operational exposure | A5 `exposure` | Kind and order of magnitude in words, with its source; never a score | A-16 (impact kept apart) |
| Consumer or user harm | A5 `exposure` | Who is harmed, how, how many, reversibility | D log (Consumer Duty; CMA guidance) |
| Enforcement exposure | A5 `exposure` (what a regulator or court **could** do) and A5 `enforcement_likelihood` (only on request) | Powers and consequences stated as facts; likelihood labelled "not a statement of law" | D log M8; G-19 |
| Brand / reputation impact | A5 `exposure` | Stated in words | WG-OV-01 (loss includes reputational), unverified wording |
| Irreversibility | A5 `exposure`; A1 `review_points` | `reversible` / `costly to reverse` / `irreversible` — for example trade mark specification at filing, publication, signature, data already shared | E log M5 |
| Deadlines | A5 `exposure`; A8 `by_when`; Stage 8 impact report "timing" | Date and what lapses | B log M9; E-08 |
| Need for specialist judgement | A3 `zone`; A8 `trigger` | Zone A / B / C + trigger name (§5) | Stage 1 §4 |

---

## 4. Controlled language

### 4.1 Statement labels for what the law requires (field `requirement_statement`)

The eight example labels in the bootstrap were checked against the evidence. All are kept. Three are added because Stage 4 and Stage 5 showed they are needed.

| Label | Use when | Must also state | Must not |
| --- | --- | --- | --- |
| **Clear requirement** | The provision's words, read in context, cover the facts (core case); V1–V4 and V6 pass | The provision and as-at date | Carry any likelihood term; be offered as one option among others |
| **Strong interpretation** | Fringe case, but text, context and purpose point one way and guidance or authority agrees | The main reason; any contrary reading | Be written as if the words alone compelled it (SC1-07) |
| **Reasonable but contestable interpretation** | A respectable contrary reading exists | Both readings; what each rests on; an outcome-likelihood band or a non-numeric exit | Be delivered without the counter-position |
| **Open / unsettled question** | No authority decides it, or authorities conflict | What would settle it; escalation consideration | Be banded from fluency alone |
| **Guidance-based expectation** *(added)* | The only support is regulator guidance or a code | Legal status, who applies it, reliance effect, currency state (Stage 5 §4.5) | Be stated as "the law requires" or dismissed as "only guidance" (D-F9) |
| **Prospective / not yet in force** *(added)* | Enacted but not commenced, or announced only | State (`enacted, prospective` or `announced`), latest official timing statement and its date | Be applied as current law, or ignored for a future launch (Stage 5 §7.1) |
| **Insufficient facts** | A material fact is unknown | The question to be answered and by whom; conditional analysis across realistic alternatives | Be filled with an assumption believed untrue |
| **Insufficient authority** | Research found nothing adequate, or verification failed | Sources searched and nil results; inspection modes used | Be replaced by commentary or model memory |
| **Jurisdiction unresolved** | A jurisdiction field that matters is `unresolved` | Which conclusions depend on it | Default silently to the proving jurisdiction |
| **Professional opinion required** | A Zone B or Zone C trigger fired (§5) | The trigger; the escalation package | Be used as a generic disclaimer on Zone A work |
| **Not lawful on the stated facts** *(added)* | A clear requirement is breached by the proposed course | The requirement; lawful alternatives if any | Be softened into a risk rating, or listed as a neutral option (MVG-OV-03, MVG-OV-07 qualified; A-16 floor by analogy) |

Exactly one label per conclusion. Roll-ups at issue and matter level list the labels of their parts; they do not average them.

### 4.2 Outcome likelihood (field `outcome_likelihood`)

Meaning: how a competent tribunal or regulator would probably decide **if the point were tested**. It is used only with the labels "reasonable but contestable" and, with care, "strong interpretation".

Default ladder (configuration; the default is the published UK yardstick, S9-02):

| Term | Range shown with the term |
| --- | --- |
| Almost certain | about 95% to under 100% |
| Highly likely | about 80% to about 90% |
| Likely | about 55% to about 75% |
| Realistic possibility | about 40% to under 50% |
| Unlikely | about 25% to about 35% |
| Highly unlikely | about 10% to about 20% |
| Remote chance | above 0% to about 5% |

Rules:

1. The word and its range always appear together.
2. Every band states its **basis**: authority level and standing; core or fringe; forum; the factual contingencies.
3. The tool never produces a point percentage. A figure supplied by counsel is reported as counsel's figure, with date and addressee.
4. Two exits are always available, modelled on S9-01: **cannot be banded** (disputed law, fact or expert evidence prevents it) and **unclear — pending named investigation** (say which investigation).
5. For a conclusion that needs several elements, the band cannot be higher than the weakest required element supports.
6. A consuming project may configure another published ladder (for example the legal-aid bands). It may not remove the ranges, the basis, or the exits.

Why the yardstick is the default and not the legal-aid bands: the legal-aid bands are built around a 50% funding threshold and have no gaps; the yardstick has gaps on purpose and comes with a separate confidence concept. This is a **design choice**, recorded as such. Stage 18 tests whether readers interpret it consistently.

### 4.3 Exposure and enforcement

- **Exposure** is described in kind, using the §3 dimensions. Two tracks where they differ: private-law effect (for example an unenforceable term, refunds) and public enforcement (for example penalties, orders). Amounts are given only when a source states them, with the source.
- **Enforcement or detection likelihood** is given only when the user asks. It sits in its own field, is labelled "not a statement of law", needs a source (for example published enforcement priorities or figures), and never changes the requirement statement. Reasoning from "unlikely to be enforced" to "permitted" is a named failure (A-F3).

### 4.4 Confidence in the analysis (field `confidence_in_analysis`)

Separate from likelihood (S9-02). Set from recorded states, not from self-assessment.

| Value | Conditions |
| --- | --- |
| **High** | All material propositions pass V1–V6; V2 on raw text; V5 by a declared citator method or not applicable; material facts `confirmed`; `stability = settled` |
| **Moderate** | Any of: V2 `extract only`; V4 `qualified` (banner, guidance under review); V5 `qualified (no citator)`; a material fact `stated, unverified`; `stability = moving` |
| **Low** | Any of: a material `not checked`; support from commentary only; a material fact `contested` or unknown; jurisdiction `assumed` on a point that matters |

Low confidence blocks the labels "clear requirement" and "strong interpretation". It does not block delivery; it is disclosed.

### 4.5 Words that are not used

| Not used | Reason | Use instead |
| --- | --- | --- |
| "compliant", "legally safe", "fully covered" | Stage 1 non-goal; only scoped, dated statements are possible | The label, jurisdiction and as-at date |
| "clear", "available" for a trade mark screen | Search is not clearance (E log F1) | "No identical mark found on (register) at (time) for (query); this does not show …" |
| "no risk", "low risk", "high risk" alone; a colour alone | Unanchored ratings (A-F4) | The four separate statements |
| Any bare point percentage | G-10, G-14, G-17 | Band with range and basis |
| "counsel has cleared it" as a reason | MVG-OV-06 | The opinion's addressee, date, question and assumptions, verified |
| "aggressive", "pragmatic", "commercial view" as substitutes for legal characterisation | Ethical fading (MVG-OV-09, MVG-OV-10) | Plain restatement |
| "As an AI I cannot give legal advice" as a blanket | Stage 1: Zone A work is lawful to support in the proving jurisdiction; generic disclaimers fail the quality definition | The zone check and its reason |

---

## 5. Escalation triggers

Each trigger stops analysis **at the trigger**, keeps the lawful preparatory work, and starts the escalation sub-loop (Stage 7 §1.2). The bootstrap's candidate list is covered; the evidence added the rest.

| # | Trigger | Zone | Typical specialist | What Legal Skills still does | Evidence |
| --- | --- | --- | --- | --- | --- |
| T1 | Reserved legal activity, or representation or advocacy | C | Authorised person | Explain the boundary; prepare facts and documents | Stage 1 E1, E2 |
| T2 | Immigration advice or services; carrying on a regulated financial activity; claims management; insolvency practice | C | Regulated adviser | Spot and package only | Stage 1 E5, E6; F-28 to F-30 |
| T3 | Financial-regulatory perimeter question | B — always | Financial-services lawyer | Spot list from the PERG sequence; no conclusion | D-12 to D-16, D-24, D-28 |
| T4 | Material enforcement or litigation exposure; regulator contact; a dispute in prospect | B | Disputes or regulatory lawyer | Facts, chronology, authority table; privilege warning | Stage 1; F-27; D log F14 |
| T5 | Conflicting authority at a high level, or an open question on a material point | B | Specialist in the field | Both readings; what would settle it | SC1-18; bootstrap §15 |
| T6 | Uncertain cross-border applicability; jurisdiction unresolved on a material point; territory outside proving scope | B | Local counsel | Per-jurisdiction issue list; what is unknown | Stage 5 §3; F-21 to F-25 |
| T7 | Trade mark: similar-mark assessment, clearance opinion, filing strategy; mandatory representation (USPTO for foreign-domiciled applicants; EUIPO for non-EEA parties — search-level evidence) | B | Trade mark attorney (per office) | Knockout screen, dated evidence, specification draft | E-01, E-20, E-22; Stage 5 G1 |
| T8 | Novel AI / IP question: authorship of generated works, training or text-and-data-mining use, likeness | B | IP specialist | Provenance record; dated statement of the UK and US positions as found; reform tracking | E log M9, M10 |
| T9 | Doctrinally loaded contract term under the governing law (endeavours, warranties and representations, consequential loss, discretion), or governing law not verified for the drafting checks | B | Contract lawyer in that law | Inventory; flag mixed use; express-steps remedy | B-04 to B-10 |
| T10 | Departure from the clear words of a provision, or reliance on purpose against text | B | Specialist | Text-first analysis; the competing reading | SC1-08; SC2-12 |
| T11 | High-risk personal-data processing; DPIA indicates high residual risk; special category or children's data; new transfers | B | Privacy counsel / DPO | Inventory, DPIA questions, requirement set | C-08, C-12, C-13 |
| T12 | Copyleft in a distributed or network-served product; licence incompatibility | B | Open-source licensing lawyer | Component and licence record from the licence text | E log F16, F17 |
| T13 | Request to build in ambiguity, to find a loophole, or to rely on a gap in the law | B | Senior counsel | Lawful-structure alternatives for a lawful goal only | AD2-02; MVG-OV-05; A-01 to A-05 |
| T14 | Knowing non-compliance proposed ("we know, we will do it anyway") | B → recorded human decision | Senior decision-maker; counsel | State "not lawful on the stated facts"; record who decides; do not rate it | G log M7; A-16 floor by analogy |
| T15 | Material ambiguity in a provision during requirement extraction | B | Legal expert | Annotate readings; carry the flag | C-32 |
| T16 | Irreversible commitment about to be made on unverified analysis (filing, publication, signature) | B | Reviewer fit for the document | Limits list; what is unverified | E log M5; Stage 1 §7 |
| T17 | Confidential, personal or possibly privileged material would have to go to an unsuitable provider | Routing stop (Stage 10) | — | Minimise, redact, or stop | SRA notice (Stage 1 E4); F-X11 |
| T18 | Low `confidence_in_analysis` on a point the user is about to rely on | B | Reviewer | Say what would raise confidence | §4.4 |

An escalation is **specific**: question, facts (including adverse ones), jurisdiction, authorities, analysis, conflicts, options, exact decision required (Stage 6 A8). "Consult a lawyer" alone fails.

---

## 6. Human review points

Refines Stage 1 §7. Every point is a recorded event: who, when, what was decided, on what version.

| Point | Decider | Record | Blocks |
| --- | --- | --- | --- |
| Scope, client / instruction and jurisdiction accepted | User | A1 | Analysis |
| Material facts and assumptions confirmed; unknowns answered or accepted as open | User / consuming project | A2 statuses | Labels above "insufficient facts" |
| Reliance on a contestable or unsettled reading | User; counsel where exposure is material | A5 + A8 outcome | Delivery as settled |
| Risk acceptance | User / project owner — never the tool | A5 `options` decision; T14 record | — |
| Approval of a legal document or clause | User; qualified reviewer in Zone B | A7 `approved (by, on)` | Publication; later edits without re-review (A-F13) |
| Filing, registration, signature | Applicant or authorised person | A1 review point | — |
| New use of personal data going live | User, after people are told | Stage 8 impact report "timing" | Go-live |
| Sending sensitive material to a provider | User, before it is sent | A1 `sensitivity` decision | The tool call |
| Decision not to implement a required control | Named person with role | A6 status note | — |

---

## 7. Stability under pressure

Rules (Stage 4 §3.3 MVG-OV-01 adapted; G-28 to G-34):

1. A conclusion changes only for one of three causes: **new fact**, **new authority**, **identified reasoning error**. The `change_log` names the cause. Disagreement, displeasure, repetition and urgency are not causes.
2. A correct user correction **is** a cause. Refusing it is also a failure (G-F10). The rule is warranted change, not no change.
3. A user's claimed status or expertise is a fact about the user. It supports no proposition (G-33).
4. A rationale that appears only after pushback is suspect (G-34). The changed conclusion must be re-derived from the records, not argued backwards.
5. Before treating a conclusion as settled on a material point, run a **baseline stability check**: re-derive it in a fresh context from the same records and compare. A difference with no change of input is an instability finding, reported as low confidence.
6. Euphemistic briefs are restated plainly at intake. Rationalisation patterns in a brief ("everyone does it", "the board signed off", "it is only technical", "counsel cleared it") are noted as facts about the brief. They never appear as supporting reasons.
7. These rules bind the workflow. They do not rely on the agent "being careful" (MVG-OV-11).

The transfer from captured in-house lawyers to AI assistants remains this project's inference. General-domain evidence is strong. No legal-task study was found.

---

## 8. Remaining useful without certainty

The exit criterion asks that the system "remain useful without inventing certainty". What is delivered when a conclusion cannot be reached:

| Situation | Still delivered |
| --- | --- |
| Insufficient facts | The questions, who can answer them, and the conditional analysis for each realistic answer |
| Insufficient authority | The research log, what was found and why it is not enough, and the specialist question |
| Jurisdiction unresolved | The issue list per candidate territory in proving scope; the dependency of each conclusion; escalation for the rest |
| Unsettled law | Both readings, what each rests on, what would settle it, and what the project can do that is lawful under both |
| Prospective law | What changes, when (with the source and date of the timing statement), and what to prepare |
| Zone B trigger | The preparatory work and the escalation package |
| Low confidence | What would raise it: which source to read in raw text, which fact to confirm, which check to run |
| Easy core case | A plain, confident answer. Over-hedging an easy case is also a failure (SC2-03 qualified) — but confidence comes from verified text, not fluency. |

---

## 9. Correct and incorrect forms (synthetic)

Illustrative only. Not statements of law.

| Incorrect | Why | Correct |
| --- | --- | --- |
| "Risk: amber. 30% chance of a fine." | Composite colour; point figure; enforcement blended with merits | "**Clear requirement:** the notice must state the retention period or criteria (provision, as at 19 Sep 2026). The notice states 12 months; configuration shows 26. **Exposure:** regulator enforcement powers apply; users were given inaccurate information. **Confidence in analysis:** moderate — guidance page is under review; read as an extract." |
| "This clause is probably fine." | No label, no basis | "**Reasonable but contestable interpretation.** Reading A …; reading B …. **Outcome likelihood:** likely (about 55% to about 75%) that reading A prevails — basis: first-instance authority only; fringe case; consumer forum. **Counter-position:** …" |
| "No conflicts found — the name is clear." | Search is not clearance | "No identical mark for identical goods found on the UK register at 10:40 on 19 Sep 2026 for the query '…' in classes 9 and 42. Two similar marks are **candidates — legal assessment required**. This screen cannot show unregistered rights, very recent filings, marks with a reputation, or use." |
| "Regulators rarely enforce this, so you can proceed." | Enforcement likelihood used as permission | "**Not lawful on the stated facts.** Lawful alternatives: …. Whether to proceed is a recorded decision for (named person); see escalation T14." |
| (after the user says "I'm a lawyer, you're wrong") "You're right, it is permitted." | Capitulation; status is not authority | "What fact, authority or error should I take into account? Without one, the conclusion stands. If you have an authority, I will verify it and re-run the analysis." |
| "It depends." | No contingency named | "**Insufficient facts.** It turns on U-002 (is any analytics data sent outside the UK?). If yes → …; if no → …. Engineering can answer." |

---

## 10. Hooks for Stage 18

Each can fail on its own: label correctness; label–gate consistency (no "clear requirement" on low confidence); band has word + range + basis; no point figures; enforcement kept apart; exits used when warranted; trigger fires when it should and **does not fire** on plain Zone A work; escalation package completeness, including adverse facts; stability under pressure with and without a real correction; baseline instability; forbidden words absent; easy case not over-hedged.

---

## 11. Bounded gaps

| # | Gap | Bound |
| --- | --- | --- |
| G1 | No evidence on how readers of **legal** outputs interpret the chosen ladder | Design choice; Stage 18 tests it; ladder is configuration |
| G2 | No legal-task study of user-pressure effects | §7 keeps the inference flag; Stage 18 fixtures |
| G3 | Lawyer-overconfidence figure rests on a secondary report | Used for direction only |
| G4 | Attorney General's guidance read by one agent; main session confirmed it at search level only | Used as one of several independent supports |
| G5 | The correspondence between labels (§4.1) and bands (§4.2) is not evidenced | None is asserted. Labels and bands are separate fields. |
| G6 | ISO 31022 not read | Not relied on |

---

## 12. Exit verification

| Requirement (bootstrap §15) | Where | Met |
| --- | --- | --- |
| No single numeric legal-risk score by default | §2; §4.2 rule 3; §4.5 | Yes — upheld after testing |
| The ten candidate dimensions researched and kept visible | §3 | Yes |
| Controlled confidence language defined | §4.1 (eleven labels: eight proposed, three added), §4.2–§4.5 | Yes |
| Escalation triggers researched, including reserved activity / representation, enforcement or litigation risk, conflicting high-level authority, cross-border uncertainty, trade mark conflicts, financial perimeter, novel AI / IP | §5 T1–T8, plus T9–T18 from the evidence | Yes |
| Human review defined | §6 | Yes |
| **Exit: the system can remain useful without inventing certainty** | §8, §9 | Yes |
