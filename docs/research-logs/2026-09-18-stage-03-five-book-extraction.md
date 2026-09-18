# Stage 3 — Extract and Reconcile the Five-Book Corpus

**Stage:** 3 of the Legal Skills bootstrap (v1.2)  
**Date opened:** 18 September 2026  
**Branch:** `feat/bootstrap-3`  
**Status:** IN PROGRESS — 3 of 5 books examined. **Stage 3 is NOT complete.** See §1.  
**Governing section:** §9 of `2026-09-08-legal-skills-new-project-bootstrap-process.md`  
**Inputs:** `2026-09-18-stage-01-domain-boundary.md`; `2026-09-18-stage-02-five-book-corpus-selection.md` (corpus revision 1)

Supporting per-book records (full finding records with all required fields):

- `2026-09-18-stage-03a-adams-findings.md` — 79 findings (AD1-, AD2-, AD3-)
- `2026-09-18-stage-03b-finch-fafinski-findings.md` — 52 findings (FF1-, FF2-)
- `2026-09-18-stage-03c-schauer-findings.md` — 50 findings (SC1-, SC2-)

---

## 1. Source-access blocker (open)

Stage 3 cannot be completed until these two selected books are directly accessible under `books/`:

| Slot | Exact missing source | What is present now |
| --- | --- | --- |
| 4 | Matthew Whalley and Chris Guzelian, *The Legal Risk Management Handbook: An International Guide to Protect Your Business from Legal Loss* (Kogan Page, 2016) — full text | `books/legal-risk-management-handbook-expanded-overview.pdf` — a 14-page overview. Secondary material only. |
| 5 | Richard Moorhead, Steven Vaughan and Cristina Godinho, *In-House Lawyers' Ethics: Institutional Logics, Legal Risk and the Tournament of Influence* (Hart, 2018) — full text | `books/in-house-lawyers-ethics-expanded-overview (1).pdf` — a 15-page overview. Secondary material only. |

Decision A2 (Stage 2 log §7): the user will supply the full texts. No replacement is authorised. The overviews have **not** been used as extraction evidence. No finding in this log comes from them.

---

## 2. Reading coverage (what was actually examined)

| Book | Access | Read fully | Skimmed | Not read |
| --- | --- | --- | --- | --- |
| S1 Adams, *MSCD* 4th ed. | Full text | Introduction; ch 1; ch 2 ¶2.1–2.72 and ¶2.129–2.217; ch 3 (all); ch 6, 7, 8, 9, 11, 12 (all); ch 10 ¶10.1–10.81 and ¶10.91–10.129; ch 4 ¶4.79–4.114; ch 5 ¶5.75–5.115; 80 named entries of ch 13; ch 14, 15, 18, 19 (all); Appendix A (all 214 annotations) compared with Appendix B | ch 2 ¶2.72–2.128; ch 16 (except ¶16.18–16.36, read); ch 17 (except ¶17.1–17.6, read) | Foreword and early Preface; rest of ch 4 and ch 5; ch 10 ¶10.81–10.90 and ¶10.130–end; ch 13 entries outside the 80 listed; works cited, table of cases, index |
| S2 Finch & Fafinski, *Legal Skills* 3rd ed. | Full text | Introduction; ch 1; ch 2 and ch 5 (method; click-paths and screenshots skipped); ch 3; ch 4 except §4.1.1; ch 6; ch 7; ch 8 (method); ch 14; ch 10 §10.1–10.2, §10.4–10.6; ch 11 §11.1–11.2, §11.3.3.2, §11.3.7; ch 12 §12.3; ch 13 §13.5; ch 17 §17.1, §17.3–17.4, §17.5.2–17.5.3; ch 18 §18.1–18.3, §18.4.5 | Headings only: ch 9, 15, 16; rest of ch 12 and ch 13; referencing-style mechanics in ch 11 | ch 4 §4.1.1; ch 10 §10.3, §10.7; ch 17 §17.2, §17.5.1; most of ch 18 §18.4–18.5 |
| S3 Schauer, *Thinking Like a Lawyer* | Full text | Preface; ch 1–12 (all, including argument-bearing footnotes) | Purely bibliographic footnotes; index (checked only to confirm the book ends at ch 12) | — |
| S8 Whalley & Guzelian | **Secondary only** | — | — | Whole book |
| S7 Moorhead et al. | **Secondary only** | — | — | Whole book |

Exact per-part coverage tables are in the supporting logs.

Extraction limits recorded by the readers:

- S1: acceptability symbols in ch 3 tables, Figure 4 (ch 8) and sample images (ch 18, 19) did not survive text extraction. Readers relied on the prose.
- S1: six usages requested for sampling are not ch 13 entries; five are treated in ch 3, 8 and 11 (which were read).
- S2: tools, databases, EU material and court details are 2010-era. Method only was retained.
- S2: the assigned text gives no hierarchy of law report series (it names only the most authoritative series). Recorded as a research question.
- Internal inconsistencies found in the sources are recorded, not corrected: S1 ¶7.3 says "five sources" and lists six; S2 has inconsistent Act dates and a doubtful explanation of the "(C. n)" element of a statutory-instrument citation; S3 has an apparently wrong "5 U.S.C." citation and a probable "within / not within" slip at p. 228.

---

## 3. Method and verification

1. Text of S1–S3 was extracted locally with `pypdf`. No file was uploaded. No PDF was changed.
2. Seven reading agents each examined one assigned part directly from the extracted text, under a written brief: no web, no model memory as evidence, own-words expression, honest coverage record, substantive law as research questions only.
3. Each agent produced finding records with the fields required by bootstrap §9.
4. The main session verified a sample of findings against the book text:

| Finding | Location checked | Result |
| --- | --- | --- |
| FF1-03 (territorial extent) | S2 ch 1, p. 15 | Content matches; index confirms p. 15 |
| AD2-01 (sources of uncertain meaning) | S1 ¶7.3–7.4 | Content matches; the "five/six" inconsistency is real |
| AD3-16 (amend vs amend-and-restate) | S1 ¶18.3–18.4 | Content matches |
| SC2-08 (three-way interpretive triage) | S3 ch 8 §8.2, pp. 157–158 | Content matches |

Limit: 4 of 181 findings were verified by the main session. The rest rest on the agents' direct reading. Stage 4 challenges the material ones in any case.

---

## 4. What each examined book contributes

### S1 Adams — drafting and review language (high contribution)

- A functional taxonomy of contract language (agreement, performance, obligation, discretion, prohibition, policy, condition, declaration, intention, recommendation) with a per-provision selection test: ask what each category implies on non-compliance (AD1-12, AD1-22, AD1-26).
- A taxonomy of uncertain meaning — ambiguity, under-specificity, mistake, conflict, omission, vagueness — each with its own detection and repair (AD2-01 to AD2-06).
- Pattern-level ambiguity checks: antecedents, "and"/"or", quantifiers, plural, modifiers before and after lists, commas (AD2-04, AD2-22 to AD2-27).
- Defined-term discipline and structural consistency (AD2-07 to AD2-11, AD2-28, AD3-14, AD3-21).
- A review method: triage what is worth raising; annotate each defect with fix and rule; leave deal terms alone; stop when change costs more than it gains (AD1-03, AD2-25, AD3-17, AD3-18).
- Amendment drafting as a smallest-sufficient-change rule set (AD3-16).
- Low contribution: layout, typography, signature blocks, letter agreements. Specialist only: material adverse change (AD2-17, AD2-18).
- Limits: US-centred; business-to-business contracts; many prescriptions are the author's own and are contested (see §7).

### S2 Finch & Fafinski — UK source system and structured problem-solving (medium–high contribution from about one third of the book)

- Legislation currency as a provision-level check: enactment vs commencement, extent, staged commencement, typed legislative effects, amending text vs revised text, point-in-time research (FF1-01 to FF1-08).
- Reading methods for an Act, a statutory instrument and a case report (FF1-10, FF1-12, FF1-20).
- Case authority: citation parsing, appellate history vs later treatment, version differences between services, three-part binding test, ratio method, options for adverse precedent (FF1-17 to FF1-24).
- Derivative texts (headnotes, digests, explanatory notes, paraphrases) are finding aids, not law (FF1-09). Graded standing of secondary sources, web sources and soft law (FF2-15 to FF2-19).
- Structured problem-solving: one rule–application–conclusion cycle per sub-issue; party/event grid; element decomposition; named application defects; conditional reasoning on missing facts; counter-argument search; three-level conclusions (FF2-01 to FF2-14).
- Honest low-contribution record: ch 9, 12, 13, 15, 16 (study, essay, exam, presentation skills) are out of scope. Negotiation (ch 18) gave two adaptable findings only. All tool guidance is obsolete.

### S3 Schauer — reasoning, authority and calibration (high contribution; mostly as qualification)

- Rule vs purpose; core vs fringe; over- and under-inclusiveness; two senses of formalism (SC1-03 to SC1-08).
- Authority is content-independent; vertical vs horizontal precedent; follow-or-distinguish; a three-way source status (mandatory / optional / not permissible); "support" citations prove little (SC1-09 to SC1-19).
- What a case stands for is uncertain; the court's own stated categories are the best guide; the holding/dicta line is unstable (SC1-11 to SC1-13, SC2-14, SC2-15).
- The selection effect: reported cases are a biased sample of hard cases; most everyday applications are easy (SC1-05, SC2-03).
- Advice as prediction; predictive power of doctrine varies by forum and issue type (SC2-01, SC2-02, SC2-06).
- Text-first interpretation with a three-way triage; literal meaning as a rebuttable presumption; canons are weak (SC2-07 to SC2-13).
- Rules vs standards: precision allocates discretion and divides decisions between now and later; breadth and vagueness are separate axes (SC2-17 to SC2-19).
- Law vs fact; hidden empirical premises; burdens, presumptions and deference as structures for uncertainty (SC2-21 to SC2-26).
- Limits: US common-law focus; theoretical; several transfers to drafting and AI-system design are the reader's inference and are flagged as such in the supporting log.

---

## 5. Provisional legal-production capability model (partial — 3 of 5 books)

Each row maps `source finding → capability → workflow implication → evaluation criterion → candidate benchmark`. Capabilities are **not** skills or commands. C20 and C21 are empty until S8 and S7 are examined.

| # | Provisional capability | Source findings | Workflow / command implication | Evaluation criterion | Candidate benchmark case (synthetic) |
| --- | --- | --- | --- | --- | --- |
| C1 | Matter framing and issue decomposition | FF2-03, FF2-04, FF2-05, FF2-06, FF2-22 | Build a party/event grid; enumerate candidate legal areas and eliminate; decompose each issue into elements; keep the question visible | Every issue has elements; every element has its own rule–application–conclusion | Brief with two plausible legal bases and one irrelevant actor |
| C2 | Fact discipline | FF1-22, FF2-10, FF2-22, SC2-21, SC2-22, SC2-23, SC2-25 | Separate fact, assumption, unknown; test materiality by counterfactual; reason conditionally on gaps and ask for the fact; surface empirical premises | No conclusion rests on an unlabelled assumption or an unsourced general factual belief | Brief missing one binary fact and one open-textured fact |
| C3 | Jurisdiction, extent and forum gating | FF1-03, FF1-24, FF1-25, SC1-09, SC1-24 | Check territorial extent and forum before applying a rule; authority status depends on the forum | Output states extent and forum, or marks them unresolved | Statute that does not extend to the user's part of the UK |
| C4 | Legislation currency verification | FF1-01, FF1-02, FF1-04, FF1-05, FF1-06, FF1-07, FF1-08, FF1-12 | Per-provision check: in force? for whom? amended, disapplied or varied? as at which date? Look for instruments under the Act | Record shows provision-level status and an as-at date | Provision enacted but not commenced; section amended by a later Act |
| C5 | Case authority verification and status | FF1-17, FF1-18, FF1-19, FF1-20, FF1-21, SC1-14, SC1-15, SC2-16 | Record appellate history and later treatment separately; record court level; check precedential status | Authority record has history, treatment, court and status fields filled or marked unknown | Case reversed on appeal; non-precedential decision cited as binding |
| C6 | Source-standing classification | FF1-09, FF2-15, FF2-16, FF2-17, FF2-18, FF2-19, FF2-23, SC1-16, SC1-17, SC1-19 | Classify every source: primary / official guidance / soft law / commentary / finding aid; mandatory / optional / not permissible in the forum | No proposition rests only on a finding aid or paraphrase | Headnote or firm blog used as the only support |
| C7 | Proposition extraction from authority | FF1-22, SC1-11, SC1-12, SC1-13, SC2-14, SC2-15 | State what the authority holds in the court's own categories; record the level of generality chosen; flag possible dicta | Proposition does not exceed what the authority decided | Broad proposition drawn from a narrow holding |
| C8 | Applicability analysis | SC1-03, SC1-04, SC1-06, SC1-07, SC1-08, SC2-07 to SC2-12, FF1-10, FF1-11, FF1-13 to FF1-16, FF2-01, FF2-02, FF2-08, FF2-09 | Text first; classify core or fringe; three-way triage (plausible / no answer / bad answer); name the facts that satisfy each element; departure from clear wording is an escalation point | No "lazy application"; fringe cases are labelled as such | Literal rule gives a result against its evident purpose |
| C9 | Counter-position and adverse authority | FF1-23, FF2-11, FF2-24, FF2-25, SC1-18, SC1-20, SC1-21, SC2-04 | Search for contrary authority; report the balance; test whether the opposite conclusion could be written | Contrary authority is reported when it exists; no invented opposition | One supporting and two weightier contrary sources |
| C10 | Calibrated conclusions | FF2-13, SC1-02, SC1-05, SC2-01, SC2-02, SC2-03, SC2-06, SC2-24 | Conclude at sub-issue, issue and matter level; confidence depends on core/fringe, forum and sample bias; advice frames a forecast, argument frames reasons | Confidence wording matches evidence strength; the three levels are consistent | Easy core question answered with needless hedging; fringe question answered with false certainty |
| C11 | Citation and provenance discipline | FF2-07, FF2-12, FF2-20 | Record exact wording and full citation when read; every statement of law, quotation, figure and definition has a source; a citation states the principle and links it to the facts | No bare parenthetical citations | Citation that names a case without saying what it establishes |
| C12 | Drafting: functional category selection | AD1-12 to AD1-26 | For each provision choose the category by asking what should follow non-compliance; name the actor; do not put duties on non-parties or uncontrolled outcomes | Each provision is classifiable; condition vs obligation is deliberate | Deadline drafted as an obligation where a condition was intended |
| C13 | Uncertain-meaning detection and repair | AD1-05 to AD1-08, AD2-01 to AD2-06, AD2-22 to AD2-27, SC2-10, SC2-11, SC2-17, SC2-18, SC2-19 | Classify the defect source before repair; keep vagueness only where deliberate; treat precision as an allocation of discretion | Each flagged defect has a type, the competing readings and a repair | Trailing modifier after a list; "and" under a discretion |
| C14 | Defined terms, references and structural consistency | AD1-08, AD2-07 to AD2-11, AD2-28, AD3-14, AD3-21 | Check circular, overlapping and unused definitions; state each fact once; decide frozen vs ambulatory references | No term is used in both a defined and an undefined sense; no duplicate statements | Number stated in words and digits that disagree |
| C15 | Usage-level review checks | AD2-12 to AD2-21, AD3-01 to AD3-13, AD3-19, AD3-20, AD3-22 to AD3-24 | A configurable check library (efforts, material, time, "including", provisos, indemnity, termination, notice, formulas, tiers) | Each check cites its rule and is jurisdiction-qualified where needed | Tier table ambiguous between stepped and flat rates |
| C16 | Review triage and smallest-sufficient change | AD1-03, AD2-25, AD3-15, AD3-16, AD3-17, AD3-18 | Raise only mismatch with the deal and real confusion risk; annotate defect, fix and rule; leave approved terms; choose the amendment vehicle | Redline does not touch unaffected approved text; each change has a reason | One defective clause in an otherwise approved document |
| C17 | House-style and precedent governance | AD1-01, AD1-04, AD3-25, SC1-23, SC2-20 | Standards are pluggable; copy only from compliant precedents; do not generalise a rule from one vivid matter | Style rules are configuration, not hard-coded law | Template rule created from a single unusual dispute |
| C18 | Escalation triggers found in the books | AD1-20, AD2-02, AD3-12, SC1-08, FF2-25 | Escalate: deliberate ambiguity; departure from clear statutory wording; terms whose meaning depends on governing law (gross negligence, sole discretion); duties of candour about adverse authority | Trigger produces a specific question for a specialist | Client asks for an intentionally ambiguous clause |
| C19 | Position preparation for negotiation | FF2-26, FF2-27 | Interests vs positions; anchor in the litigated alternative | — | — (low contribution; likely outside core; decide at Stage 13) |
| C20 | Legal-risk definition, taxonomy, reporting and uncertainty language | **None yet — awaits S8 full text** | — | — | — |
| C21 | Professional independence, pressure and escalation infrastructure | **None yet — awaits S7 full text** | — | — | — |

No skill is created per book. S1 feeds C12–C17; S2 feeds C1–C6, C8, C9, C11; S3 feeds and qualifies C2, C3, C5–C10, C13, C17.

---

## 6. Overlap, support and conflict (across S1–S3)

| Topic | Sources | Relationship | Accepted handling |
| --- | --- | --- | --- |
| Taxonomy of unclear text | AD2-01 (six sources) vs SC2-11 (ambiguity / vagueness / open texture) | Overlap with different cuts | **Merge** into one uncertainty taxonomy used for contracts and legislation. Keep "open texture" (latent, surfaces on new facts) because S1 lacks it; it links to change impact. |
| Vagueness as a tool | AD2-06; SC2-17, SC2-18, SC2-19 | Reinforcing, from independent disciplines | **Retain.** Precision is a choice that allocates discretion and timing. |
| "Tested" contract language | AD1-02 rejects reliance on litigated wording vs SC1-10 (authority binds regardless of reasoning quality) and AD1-24 (English courts may treat "represents"/"warrants" labels as operative, per the author's own report) | **Conflict**, jurisdiction-dependent | **Qualify.** Never normalise legally loaded verbs or terms of art automatically. Treat as a governing-law research question. |
| Canons of interpretation | FF1-15 (checklist) vs SC2-13 (sceptical) vs AD3-15 (do not lean on internal interpretation rules) | Partial conflict | **Qualify.** Canons are issue-spotting aids and drafting risks. They are not predictive rules. |
| Interpretive approach | FF1-13 (literal / golden / mischief / purposive are descriptions, not rules) and SC2-08, SC2-12 (text-first triage; literal meaning as rebuttable presumption); SC1-08 (UK somewhat less willing to depart from words) | Reinforcing, with a jurisdiction difference | **Merge.** Use the triage; record jurisdiction; treat departure from clear words as an escalation point. |
| Ratio / holding | FF1-22 (a workable method) vs SC1-13, SC2-15 (the line is unstable) | Tension | **Qualify.** Use the method, anchor on the court's own words (SC1-12), and record uncertainty about level of generality. |
| Binding vs persuasive | FF1-21 (three-part binding test) vs SC1-16, SC1-17 ("persuasive authority" is a confused label; three classes by decision-maker freedom) | Different models | **Adapt.** The authority record needs both hierarchy status and mode of use (deference vs persuasion vs mere support). Input to Stage 5. |
| Doctrine as answer vs doctrine as forecast | FF2-01 to FF2-13 (assume doctrine yields answers) vs SC1-02, SC2-01 to SC2-04 (realist limits) | Tension | **Qualify.** Keep the structured cycle. Calibrate confidence by core/fringe, forum and sample bias. Note SC2-03: most everyday questions are easy cases — this supports useful, confident answers on core questions. |
| Scope discipline | FF2-06 (ignore issues outside the instruction) vs Stage 1 owned outcome "issue spotting" | **Conflict** with the project boundary | **Qualify.** Do not analyse out-of-scope issues, but flag them. |
| Missing facts | FF2-10 (reason conditionally) and SC2-25 (presumptions fix the default) | Reinforcing | **Adapt.** Add the professional step absent from the student text: ask for the fact. |
| Secondary sources | FF1-09, FF2-15 to FF2-19; SC1-19 | Reinforcing | **Retain.** |
| Smallest-sufficient change | AD1-03, AD2-25, AD3-16 to AD3-18; SC2-18 (specific rules misfit later) | Reinforcing | **Retain.** Direct book support for a family principle. |
| Over-generalising from one case | SC1-23, SC2-20; AD1-04 (central style guide) | Mild tension | **Adapt.** Central standards yes; rules derived from single matters no. |
| Negotiation ethics | FF2-25, FF2-27 contain a casual approval of "bluffing" and a claim that a negotiated settlement "is not binding" | Book error / unsafe advice | **Reject** both statements. Recorded as research questions. |

Repeated claims are not independent corroboration: S2 and S3 both describe common-law precedent from standard doctrine. Agreement between them is not two pieces of evidence.

---

## 7. Claims handed to Stage 4

1. **Substantive-law research questions:** 166 recorded across the supporting logs (S1: 79; S2: 38; S3: 49). None may support a live legal conclusion without current authority for the matter jurisdiction and date.
2. **Contested author positions (S1):** no hierarchy of efforts standards; "double materiality" as a myth; "shall" discipline; "states" in place of "represents and warrants"; omitting "sole discretion"; the consideration recital; "including" (dispute with Garner); "arising out of or relating to". All are dispositioned *qualify* or *adapt*. The author himself reports English, Canadian and Singapore authority against some of them.
3. **Jurisdiction transfer:** S1 and S3 are US-centred; S2 is England and Wales, 2011. Stage 4 must test transfer to UK and EU consumer-facing documents, which none of the three books addresses.
4. **Currency:** S2 court hierarchy, EU and human-rights material, and all tools; S3 examples of binding US precedent. Rebuild from current sources in Stages 4, 5 and 11.
5. **Gaps confirmed by reading:** no examined book covers requirement traceability or change impact (D9), confidentiality in tool use (D10), notice-style and consumer document drafting, or product-counsel workflow. S1's process evidence is asserted, not measured (AD3-25).
6. **Still unexamined:** legal-risk method (S8) and professional independence and escalation (S7).

---

## 8. Plan for the two pending books

When the full texts are present under `books/`:

| Book | Intended contribution | Priority reading |
| --- | --- | --- |
| S8 Whalley & Guzelian | C20: definition and causes of legal risk; taxonomy; identification, quantification, control, reporting; risk appetite; probability language. Test against the bootstrap's "no single score" default. | Part 1 fully; Part 2 category chapters for method |
| S7 Moorhead et al. | C21: how pressure and role shape legal-risk advice; ethical infrastructure; escalation routes; what makes independence hold. Evidence quality and limits of the empirical method. | Methods; tournament of influence; competing logics; legal-risk chapter(s); moral compass; ecologies; conclusions |

Then: update §2, §4–§7, fill C20 and C21, re-run the overlap/conflict analysis across all five, and re-check the exit criteria.

---

## 9. Exit check

| Exit requirement (bootstrap §9) | State |
| --- | --- |
| All five books meaningfully examined for their contributions | **NOT MET — 3 of 5.** S7 and S8 are blocked on source access (§1). |
| Material findings traceable | Met for S1–S3 (181 findings with chapter / paragraph / page locations) |
| Per-book findings and examined-source locations | Met for S1–S3 (supporting logs) |
| Reading coverage recorded honestly | Met for S1–S3 (§2) |
| Source-to-capability matrix | Partial (§5): C20, C21 empty |
| Overlap / conflict analysis | Partial (§6): three books only |
| Provisional capability model | Partial (§5) |
| Limitations, conflicts and unresolved claims explicit | Met for S1–S3 (§2, §6, §7) |
| Book-derived law not treated as authority | Met (§7 item 1) |

**Stage 3 remains open.** Stage 4 must not start until this stage is complete.
