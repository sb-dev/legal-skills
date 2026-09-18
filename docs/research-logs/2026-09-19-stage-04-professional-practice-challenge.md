# Stage 4 — Challenge and Extend Through Professional Legal Practice

**Stage:** 4 of the Legal Skills bootstrap (v1.2)  
**Date:** 19 September 2026 (research retrieved 18–19 September 2026)  
**Branch:** `feat/bootstrap-3`  
**Status:** Complete — evidence-qualified legal-production model accepted as input for Stage 5  
**Governing section:** §10 of `2026-09-08-legal-skills-new-project-bootstrap-process.md`  
**Inputs:** Stage 1 boundary log; Stage 2 corpus log; Stage 3 extraction log and supporting logs a–d

Supporting records (full evidence registers, practice descriptions, challenge tables, failure modes, glossaries, benchmark ideas):

| Log | Streams | Inspected sources |
| --- | --- | --- |
| `2026-09-19-stage-04a-inhouse-legalops.md` | In-house product / technology counsel; legal operations / matter management | 33 |
| `2026-09-19-stage-04b-contracting-diligence.md` | Commercial contracting; transactional due diligence | 42 |
| `2026-09-19-stage-04c-privacy-ai-traceability.md` | Privacy / data protection; AI regulation; law-to-requirements traceability | 37 |
| `2026-09-19-stage-04d-consumer-fintech.md` | Consumer / digital commerce; financial-services perimeter | 40 |
| `2026-09-19-stage-04e-ip-licensing-oss.md` | Trade marks; copyright / licensing / media; open-source compliance | 50 |
| `2026-09-19-stage-04f-research-boundary.md` | Legal research and memorandum practice; open boundary questions from Stage 1 | 39 |
| `2026-09-19-stage-04g-compliance-risk-communication.md` | Regulatory compliance / controls; risk communication; AI under user pressure | 33 |
| `2026-09-19-stage-04h-glossary.md` | Terminology glossary (187 rows) | — |

Total: 274 inspected sources. All 13 practice streams named in bootstrap §10 are covered.

---

## 1. Method and its limits

1. Seven research agents worked in parallel under one written brief. Each had named streams, named Stage 3 claims to challenge, and a duty to seek contrary evidence and missing responsibilities.
2. Retrieval was native-first: web search for discovery; a fetch tool or local text extraction of public PDFs for inspection. Firecrawl was not needed. No supplied book was uploaded.
3. A usage limit interrupted all seven agents on 18 September. They resumed with context intact on 19 September. Each register row carries its own retrieved-at date.
4. **Tool-reliability finding (material).** The fetch tool returns a model-written extract. Agents caught it, by checking raw text, doing the following: reversing the holding of a judgment; inventing page content that matched the question; fabricating quotations (twice); misquoting an EU article; giving a wrong author, date and in-force status; mislabelling an annex. Consequences:
   - quotations are marked text-verified or "as reported" in the supporting logs;
   - a model-written summary of a source is not the source — this becomes a production rule (§6, N12);
   - the same failure is recorded in six independent streams (A-F15, B-F8, C-F9, D-F13, F-X14, G-F14).
5. Main-session verification at primary sources (19 September 2026):

| Claim checked | Source | Result |
| --- | --- | --- |
| DMCC Act 2024 subscription-contract chapter is not in force | legislation.gov.uk, 2024 c. 13, Part 4 ch 2 | Marked "Prospective"; sections "not in force at Royal Assent" |
| Trade Marks Act 1994 s 82 (agents) and s 84 (protected title) | legislation.gov.uk | As reported by stream E; no known outstanding effects |
| EU AI Act amended by Regulation (EU) 2026/1744 | Search results incl. EUR-Lex entry and three law-firm notes | Consistent with stream C (search-level check; stream C inspected EUR-Lex) |
| Attorney General's legal-risk guidance exists, uses a "tenable argument" floor | Search results incl. gov.uk PDF (2024) and news of the update | Consistent with stream A (search-level check; stream A read the 2026 text) |
| Stage 3 wording on Adams and English good faith | Stage 3 supporting log a, research question 15 | Recorded there as the author's view in a research question, not as a finding |

6. Limits: many law-firm notes were undated or blocked (403). ISO standards were read only in preview. WorldCC research is paywalled. EUIPO pages were blocked. No study was found that applies user pushback to legal-advice tasks. Public evidence on how product counsel really work is thin and partly from vendors.

---

## 2. Practice comparison matrix

One row per stream. Detail and evidence IDs are in the supporting logs.

| Stream | Primary fact base | Source ecology (first places to look) | Core working artefacts | Commitment / approval points | Escalation boundary | Change triggers | Typical failure |
| --- | --- | --- | --- | --- | --- | --- | --- |
| In-house product / technology counsel (a) | Product behaviour and planned change; who the client entity is | Statute → regulator guidance → internal policy and playbooks | Intake record; launch / review gate; requirement library; options note | Launch gate; risk acceptance by the business with a record | SRA in-house guidance: independence, escalation ladder, records; unlawful = say so | "New or modified" product; law change | Clear requirement priced as a risk; approval under time pressure |
| Legal operations / matter management (a) | Request and matter data | Internal knowledge base; playbooks | Front-door intake; triage rules; matter record; knowledge capture with owner and review date | Triage decision; playbook approval | Threshold breach → senior legal / outside counsel | Playbook review date | Ad hoc handling; stale templates; repeated purchase of the same advice |
| Commercial contracting (b) | The deal as agreed; side; paper origin; governing law | Governing-law case law and statute (UCTA, Misrepresentation Act) → market standard forms → house playbook | Review brief; issue list; playbook (preferred / fallback / walk-away); tracked redline; obligations register | Signature; variation (formalities) | Doctrinally loaded terms; liability architecture; discretion clauses | Amendment; renewal; related-document change | Normalising endeavours or warranty wording under English law; untracked change |
| Transactional due diligence (b) | Data room; disclosure bundle | Deal documents; registers; searches | Scoping record (materiality, lookback, exclusions); red-flag report with source links and "not reviewed" list | Scope sign-off; disclosure; claims notice deadlines | Specialist areas outside scope | New disclosure; price or structure change | Generic checklist; buried material issue; defective disclosure or late notice |
| Privacy / data protection (c) | Data-flow inventory per processing activity | UK GDPR / DPA 2018 as amended → ICO guidance (with status banner) → case law; EDPB for EU | ROPA; role analysis; lawful-basis record; LIA; DPIA; transfer assessment; notice; processor terms | DPIA sign-off; launch; new purpose (tell people before processing) | High-risk processing; novel AI use; transfers; regulator contact | Product, law / guidance, third party (three directions) | Notice from a template; notice frozen while product moves; "Act in force" treated as "provision applied" |
| AI / automated-system regulation (c) | Actor role (provider / deployer); system behaviour; user interface | EU AI Act as amended (application dates) → Commission guidelines; UK GDPR Arts 22A–22D → ICO | Role and risk-class record; disclosure text tested per regime | Placing on market; interface release | High-risk classification; cross-border scope | Application dates (which were amended three weeks before they applied) | Stale dates; one regime's rule carried into another |
| Consumer / digital commerce (d) | The real user journey (sign-up, renewal, cancellation, checkout) | CRA 2015; CCRs 2013; DMCC Act 2024 (provision-level commencement) → CMA guidance (CMA37, 22 July 2026) | Terms; pre-contract information; prominence map; journey-vs-document consistency check; choice-architecture review | Publication of terms; flow release | Regulator engagement; sector overlays | Flow change; commencement of prospective provisions; guidance reissue | Clear, precise, unfair term; readable but non-transparent term; flow contradicts terms |
| Financial-services perimeter (d) | What the feature actually does for the user | FSMA ss 19, 21, 23; RAO; PERG; PSRs 2017 | Perimeter issue list; specialist package | Any launch of a finance-adjacent feature | **Always Zone B**: breach of the general prohibition is criminal; PERG itself says seek advice if in doubt | New feature; AI assistant scope creep | Concluding "it is only information"; assistant drifts into advice |
| Trade marks (e) | Candidate mark; territory; goods / services; dated register evidence | TMA 1994 s 5; UK IPO manual; EUIPO / USPTO equivalents | Knockout screen (identical / similar separated); dated hit list; specification draft | Filing (specification cannot be widened later) | Similar-mark assessment; opinion; filing strategy; USPTO requires a US attorney for foreign applicants | New filings; new territory; brand change | Registry search reported as "clear"; exact-match only |
| Copyright / licensing / media (e) | Provenance chain per asset | CDPA 1988; licence text (versioned); government reports are proposals | Provenance record; licence-scope analysis (rights, territory, term, media, exclusivity) | Publication / distribution | Likeness; layered rights; AI-generated works (UK and US differ) | Source or distribution change; pending reform | "We paid, so we own it"; reform proposal stated as law |
| Open-source compliance (e) | Component list with versions; distribution model | Licence text (SPDX expression, -only / -or-later) → steward interpretation | SBOM; notices file; obligations by distribution model | Release | Copyleft in distributed or network-served product; incompatibility | Dependency change; distribution-model change | Licence summary used instead of text; scanner output accepted unreviewed |
| Legal research and memorandum (f) | The question presented and the stated facts | Official legislation with status apparatus; official case law; citators (commercial); EUR-Lex (OJ is authentic, consolidated text is not) | Research log (sources searched, nil results); authority record; answer-first memo with assumptions, as-at date, limits | Delivery of advice; any citation to a court | Material point with no later-treatment check; conflicting authority | Later treatment; amendment; commencement | Non-existent case; real case that does not support the proposition; banner not read |
| Regulatory compliance / controls (g) | Obligations register (law **and** voluntary commitments) | ISO 37301 structure; sector regulator pipelines | Obligation → control → dated operating evidence; decision record when a control is declined | Control sign-off; periodic review | Knowing non-compliance is a recorded human decision | Law change; third-party process change | Paper programme; opinion used as risk transfer |

Cross-stream pattern: every stream has **its own primary fact base**, and the legal document is a derived view of it. This independently supports the bootstrap principle "the document must match the product".

---

## 3. Challenge findings — accepted dispositions

Standing key: **SF** supported finding · **CM** context-dependent method · **PH** practical heuristic · **DC** disputed claim · **UQ** unresolved question.

### 3.1 Drafting and review (S1 Adams)

| Claim | Disposition | Standing | Key evidence (log b / d / e) |
| --- | --- | --- | --- |
| AD1-02 reject reliance on "tested" language | **Qualify.** Bespoke wording: "tested" is a weak reason. Standard forms and doctrinal labels: treat as operative; no rewrite without governing-law research. | CM | English judgments give labels real effect |
| AD2-12 no hierarchy of endeavours / efforts | **Reject as English law; retain the drafting remedy** (state the steps). Never equate or normalise endeavours formulas under English law. | SF (E&W) | *Rhodia* distinguishes best from reasonable endeavours |
| AD1-24 replace "represents and warrants" with "states" | **Reject for English-law documents.** Lock these verbs against style edits. Add a remedy-coherence check (non-reliance, entire agreement, Misrepresentation Act s 3). | SF (E&W) | *Sycamore*; *Idemitsu*; materially different damages |
| AD3-01 "including" | **Adapt.** Keep list classification. Do not strip "without limitation" from English-law paper. | CM | *Transocean* |
| AD3-05 consequential loss | **Retain with an English overlay:** name heads of loss; check UCTA / CRA; scenario-test. | CM | |
| AD1-20 "sole discretion" | **Qualify; Stage 3 research question 15 answered for E&W:** English law implies rationality and good faith into a contractual discretion (*Braganza*). Never advise that "sole / absolute" makes a decision unchallengeable. Stays an escalation trigger. | SF (E&W) | *Braganza*; *Tesco v USDAW* (concurring remarks) |
| AD3-16 / 17 / 18 amendment and review method | **Retain, extend:** pre-amendment gates (no-oral-modification clause; consideration or deed; authority; third-party and guarantor consent; related documents). Add review mode "do not edit — locked standard". | SF | *Rock Advertising*; C(RTP)A 1999 s 2 |
| AD1-06, AD1-08, Adams generally → consumer terms | **Adapt / split.** Adams is a *clarity* layer only. For consumer documents **reject** "no explaining" and "never repeat". Replace with: explain, layer, then check consistency across every layer. Mandatory second test: can the average consumer understand the practical consequences? | SF (UK) | CMA37 (22 July 2026); CRA ss 64, 68 |
| AD3-23 do not emphasise provisions | **Adapt.** For consumer terms build a prominence map: which terms are onerous or price-related, and where in the journey each is surfaced. | SF (UK) | CRA s 64 prominence condition |
| AD3-14 frozen vs ambulatory references → licences | **Adapt.** Licence-version default is frozen; record who holds the "or later" option; pin component and licence version together. | SF / PH | SPDX practice; compatibility depends on version |

### 3.2 Research, authority and reasoning (S2 Finch & Fafinski; S3 Schauer)

| Claim | Disposition | Standing |
| --- | --- | --- |
| FF1-02 commencement modes | **Retain and extend:** transitional and saving provisions; check the *amended* instrument; EU "application date" equivalent. Ask "which version governed this event on this date?" | SF (live test: Data (Use and Access) Act 2025) |
| FF1-04 provision-level in-force check | **Retain.** Record the outstanding-changes banner state and the page as-at date. A regulator's "all in force" statement is a finding aid. | SF |
| FF1-05 layered updating | **Adapt:** fields "site current-to date" and "gap check from / to". Official revised text can lag. | SF |
| FF1-06 typed legislative effects | **Retain.** Use the official effect vocabulary; add "applied to text: yes / not yet". | SF |
| FF1-17, FF1-19 citations and versions | **Retain / adapt:** record "best report available", "version actually read", and handed-down vs report. | SF |
| FF1-18 later treatment | **Qualify.** No free official UK citator was found. Output must state the method used: commercial citator / free-text search / none. "None" blocks a confident conclusion on a material point. | CM |
| FF1-24 court hierarchy as reference data | **Adapt.** Needs a verification date and a prospective-changes column. 2011 content must be rebuilt (Supreme Court; assimilated EU law; REUL Act 2023). | SF (design) |
| FF1-14, FF1-25 EU and rights-based interpretation | **Adapt.** Keep provenance as a mandatory field (domestic / assimilated / implements international obligation / rights-sensitive). Flag every EU citation authentic vs consolidated. Substance is perishable. | SF (method) |
| FF1-13; SC2-08; SC2-12 interpretation | **Merge and retain with a UK note:** build readings text → context → purpose → external aids. "Plain meaning" means meaning in statutory context. Check statutory interpretive duties first. | SF (UK form) |
| SC2-10 vague vs open-textured wording | **Adapt.** In regulated fields the lookup order is settled: statute → statutory code → regulator guidance (dated, status-checked) → case law. Vagueness moves: statute can convert a standard into a rule. | CM |
| FF2-18 soft law "uncertain until tested" | **Qualify.** Keep status labelling. Add fields: who applies it and with what power; stated reliance effect (safe harbour / "have regard" / none); practical weight; currency state. | SF |
| SC1-16 mandatory / optional / not permissible | **Adapt.** Keyed by forum. Add a fourth working value: usable for research, not citable. | SF |
| SC1-11, SC1-21 similarity needs a legal test | **Retain, adapted to trade marks:** separate identical from similar hits; name the dimensions screened; label similar hits "candidate — legal assessment required"; never output "no confusingly similar marks". | SF |
| FF1-09 finding aids are not law | **Retain and extend** with source classes: licence text (versioned), register entry (dated), steward interpretation, licence summary, scanner output, registry guidance. | SF |
| FF2-01 four-move reasoning cycle | **Retain** per issue. **Merge** into an answer-first memo: answer, facts / assumptions / unknowns, as-at date, sources searched, limits, next steps. | CM |
| FF2-13 three-level conclusions | **Retain.** Type each contingency as assumption (fact) or qualification (law). An assumption believed untrue is not allowed. | SF |
| SC2-01 advice as prediction | **Adapt.** Predict the tribunal outcome. Give enforcement likelihood separately, only on request, only with a source. | PH |
| SC2-03 easy cases dominate | **Qualify.** Confident wording only after the authority is resolved, read and currency-checked. Confidence comes from verified text, not fluency. | PH |
| SC2-24 burdens as confidence model | **Adapt.** Use categorical gates tied to the action (publish / rely / escalate), stated in verification terms. | CM |
| SC2-17, SC2-18 rules vs standards | **Adapt.** Keep as a change-impact lens (open standard + moving guidance = monitoring). Consumer rule of thumb: trader-side discretion needs stated reasons, limits, notice and an exit right. | CM |

### 3.3 Overview-derived claims (S8 Whalley & Guzelian; S7 Moorhead et al.)

These entered Stage 4 as unverified. Result of independent checking:

| Claim | Result of challenge | Disposition | Standing |
| --- | --- | --- | --- |
| WG-OV-01 four-cause definition | Wording found only in tertiary sources. The IBA / McCormick definition excludes wilful or reckless behaviour — a direct contradiction of the fourth cause. ISO 31022 has no cause taxonomy. | **Adapt.** Use the causes only as a diagnostic tag that selects the control. "Indifference" is a conduct and escalation item, not a rated risk. | DC (as a definition); PH (as a tag) |
| WG-OV-02 risk sits where the business acts | Regulators start from actual behaviour. But obligations also move when law, guidance or third parties move. | **Retain as the fact-gathering rule only.** | SF / PH |
| WG-OV-06 vs MVG-OV-03 vs "no single score" | Evidence on all sides (see §4). | **Qualify — controlled-language position in §4.** | CM; empirical parts SF |
| WG-OV-05, WG-OV-08 vs MVG-OV-06 | DOJ "paper programme" test; UK failure-to-prevent-fraud guidance; Post Office Swift Review; FTC bar on relying on management assertions. | **Adapt.** Every register row needs dated evidence that the control operated. "Counsel cleared it" is verified: who was asked, what question, on what facts, what was withheld, what the opinion says including adverse parts. | SF (that it happens); PH (the checklist) |
| WG-OV-07 control effectiveness; risk → requirement → control → evidence | Supported by ICO duties, NIST and the requirements-engineering literature. But many duties apply whatever the risk. | **Adapt.** Chain becomes `provision (as-at date, source type) → obligation → product fact → requirement → control / implementation → operating evidence`. Risk is a branch condition, not the root. | SF / CM |
| WG-OV-09 horizon scanning | ISO 37301 supports change monitoring with ownership. | **Retain, scoped.** Legal Skills defines the trigger and the bounded re-review and records the source to watch. It does not run the watch. | CM |
| WG-OV-10 conduct / fairness regulation | Now independently supported for the UK (Consumer Duty; DMCC enforcement since 6 April 2025). Senior-manager limb not tested. | **Retain**, re-based on current evidence. | SF (UK, 2026); UQ (one limb) |
| WG-OV-11 legal vs compliance | A difference of function, not person. Only an audit certifies. | **Retain as heuristic.** | PH |
| WG-OV-12 contract loss and obligation tracking | NAO guide supports obligation tracking and handover. All WorldCC figures trace to one gated source family. The "non-performance, not drafting" split is too sharp. | **Adapt.** Obligations register is a standard review output. Never quote the "9%" figure as fact. | PH; UQ (figures) |
| WG-OV-14 IP ownership, freedom to operate, territoriality | Ownership chain supported (UK). | **Adapt:** three separate checks — brand clearance, content / asset rights chain, patent FTO (spot and escalate). Add licence scope and provenance. | SF / CM |
| MVG-OV-01 capture → AI sycophancy (project inference) | Strong general-domain evidence from independent groups. No legal-task study. Most stance changes in one study were *towards* the correct answer. | **Adapt; keep the inference flag.** A conclusion may move only on a new fact, a new authority or an identified reasoning error, and the output names which. Run a baseline stability check before any pressure test. | SF (general); UQ (legal tasks) |
| MVG-OV-03 boundary becomes a price | The failure mode is real. Official guidance legislates against it while still using numeric bands. | **Retain, qualified** — a named failure mode plus the §4 safeguards. | SF (failure mode); CM (remedy) |
| MVG-OV-04 interpretive drift | Supported by the authors' data and by two official texts. | **Retain, qualified.** Enforcement likelihood may appear only in its own field, after the merits answer. | SF |
| MVG-OV-06 theatre; opinions as risk transfer | Supported (see above). | **Retain, adapted** into an instruction-quality checklist for escalation packages. | SF / PH |
| MVG-OV-07 neutral adviser as abdication | The authors' own survey regression does not support the strong reading. SRA guidance: advice not followed is not reportable, and accepting a degree of legal risk can be proper. | **Qualify.** The user decides. The output names an unlawful option as unlawful and carries the escalation trigger. | DC (strong form); SF (narrow form) |
| MVG-OV-08, MVG-OV-12 reported figures | Checked against the authors' 2016 UCL report: n = 400 verified; five orientations verified; "36%" verified with corrected item wording and it includes "somewhat agree". **The overview's claim that the commercial orientation predicts moral disengagement is contradicted** by the report's regression (only "exploiting uncertainty" predicts it). "67 interviews" not verified. | **Adapt.** Cite the authors' free report, not the overview. | Mixed |

**Observation for the final audit:** independent checking found at least one inaccuracy and one unverifiable figure in the supplied overviews. This is the practical cost of the Stage 3 waiver. It is now bounded by the dispositions above.

---

## 4. Controlled-language position on legal uncertainty (for Stage 9 to test)

Evidence for numbers: verbal probability words are read very differently by different readers; words plus ranges perform better than words alone; England and Wales legal aid rules and the Attorney General's legal-risk guidance (reissued 8 September 2026) use fixed percentage bands with fixed wording. Evidence against point figures: lawyers' predictions are overconfident; UK intelligence practice leaves gaps between bands to avoid false accuracy; model answers can flip with no change in input. Evidence for separation: US tax-opinion practice excludes audit likelihood from the merits percentage; the Attorney General's guidance keeps merits, likelihood of challenge and impact apart and sets a floor below which the advice is "unlawful".

Position:

1. **Four separate statements, never merged:** (a) what the law requires on the stated facts; (b) how a competent tribunal or regulator would probably decide if the point were tested; (c) exposure if wrong; (d) enforcement or detection likelihood — only on request, labelled "not a statement of law", never used to soften (a).
2. **A clear requirement is stated as a requirement.** No likelihood term attaches to it. Knowing non-compliance is a recorded human decision and an escalation item.
3. **Likelihood uses a fixed verbal ladder shown with its range.** Five to seven bands with gaps. The exact ladder is configuration.
4. **No tool-generated point percentages.** A band needs a stated basis (authority level, core / fringe, forum, factual contingencies). Counsel's figure is reported as counsel's.
5. **Two mandatory non-numeric exits:** "cannot be banded — disputed law, fact or expert evidence" and "unclear — these named investigations would allow a band".
6. **Confidence in the analysis is a separate rating** over source base, verification status and volatility of the law. It is not multiplied with likelihood.
7. **No composite score and no single colour for a matter.** A consuming project may derive its own per-item rating; the requirement statement travels with it.
8. **Conjunctive claims:** the overall band cannot exceed what the weakest required element supports; every "depends" names its contingency.

Not imported: the government "tenable argument" floor. It is built for ministerial decisions and does not transfer to product work. Standing of the whole position: context-dependent method.

---

## 5. Corrections and answers to earlier logs

Accepted logs are not edited. Later stages must read these corrections with them.

| Earlier item | Stage 4 result |
| --- | --- |
| Stage 1 §4 Zone C lists "filing or representing as an agent" | **For the UK this is a project policy choice, not a legal bar.** TMA 1994 s 82 lets a person act through an agent authorised orally or in writing; trade mark filing is not a reserved legal activity; the statutory bar (s 84) is on the *title*. Keep the policy (an AI tool should not act as a filing agent), but describe it correctly. USPTO: foreign-domiciled applicants must use a US-licensed attorney — a true mandatory escalation. EUIPO representation rules: **unresolved** (pages blocked). |
| Stage 1 E7 (protected title, self-filing) — discovery-level | UK and US verified at primary source. EUIPO not. |
| Stage 1 Q2 (US / EU advice boundary) | **Confirmed jurisdiction-dependent.** The dividing test is *individualised advice on a concrete case*: Germany RDG §2(1); New York; Texas takes software with a clear disclaimer outside the definition; the FTC acted against DoNotPay for deceptive claims, not for unauthorised practice. New design rule: provider-side claims discipline — never describe the tool as a lawyer or lawyer-equivalent. |
| Stage 1 Q3 (other UK perimeters) | Added: claims management (FCA-regulated); insolvency practitioners (Insolvency Act 1986 Part XIII). Will-writing confirmed not reserved. |
| Stage 1 Q5 (ABA 512; other guidance) | ABA opinion still read only through a secondary source (403). Law Society guidance blocked (403). Inspected instead: *Ayinde* [2025] EWHC 1383 (Admin); SRA notice; CCBE guide; SRA in-house guidance suite (2024–2026). Bar Council and judicial AI guidance: landing pages only. |
| Stage 1 Q6 (privilege and AI tools used by non-lawyers) | *Prudential* [2013] UKSC 1 confines legal advice privilege to lawyers. A founder's AI work product is **probably not privileged**; pasting a lawyer's advice into a public tool risks waiver. The UK position for a non-lawyer's AI output is an **inference, not a decided point** → Stage 10. |
| Stage 3 supporting log a, research question 15 (Adams: England implies no good-faith limit on discretion) | Not accurate for England and Wales as at September 2026 (§3.1, AD1-20). |
| Stage 3 supporting log d, MVG-OV-08 | One reported correlation is contradicted by the authors' own report (§3.3). |
| Stage 3 §7 "US-centred drafting advice must be tested for transfer" | Done for England and Wales and for UK consumer terms. **Not done** for EU member-state contract law or for the US position on each challenged claim. |

---

## 6. Missing-capability analysis

Responsibilities that the five books do not cover and that professional practice requires. "→ C" shows the Stage 3 capability extended; **N** marks a new capability.

| # | Capability | Evidence streams | Standing | Handling |
| --- | --- | --- | --- | --- |
| N1 | **Domain fact base before documents**: data-flow inventory; real user journey; provenance chain; component list; deal terms | c, d, e, b | SF | No drafting or review without the relevant fact base; missing rows are recorded unknowns (→ C2) |
| N2 | **Role and client identification**: which entity is the client, who instructs, with what authority; controller / processor and provider / deployer decided from facts, not labels | a, c | SF | Gating step at intake (→ C1) |
| N3 | **Derived-document consistency**: notice, ROPA, DPIA, contracts, summaries, FAQs, journey copy and marketing are views of one fact base | c, d | SF | Consistency check across every layer |
| N4 | **Guidance as soft law with status**: enforcing body and power; reliance effect; practical weight; currency state (current / under review / updated / consultation / withdrawn) | c, d | SF | Extends C6; input to Stage 5 |
| N5 | **Three-state legislative currency** plus transitional and saving provisions and the amended-instrument check: in force / enacted but prospective / announced only | c, d, f | SF | Extends C4; input to Stage 5 |
| N6 | **Three-test citation verification**: exists; quotation is in it; supports the proposition. "Misgrounded" citations pass an existence check. | f | SF | Extends C5, C11. Measured rates (US-law queries, 2024): 17%–33% for commercial legal research tools; 43% for a general model |
| N7 | **Declared later-treatment method** with an honest "not available" state; research log of sources searched and nil results | f | CM | Extends C5 |
| N8 | **Law-to-requirement extraction method**: statement-level coverage; cross-reference closure; exception priority; definitions dictionary; ambiguity annotation with escalation; dated trace links | c | SF (method) | Core of Stage 8. Measured risks for model extraction: omission (16 of 61 expert requirements covered in one study) and wrong citation (50%–68% correct) |
| N9 | **Coverage as its own quality dimension**, separate from correctness | c | SF | Stage 18 |
| N10 | **Change triggers from three directions**: product, law / guidance, third party; review gate tied to "new or modified" | a, c | SF | Extends C-level change impact; Stage 8 |
| N11 | **Governing-law label lock**: a list of doctrinally loaded terms that must not be restyled; locked standard forms | b | SF (E&W) | Extends C12, C15, C17: checks are keyed by governing law |
| N12 | **Distrust of summarising intermediaries**: a model-written summary is not the source; holdings and quotations are checked against raw text | a, b, c, d, f, g | SF (observed six times in this stage) | New verification rule; Stage 18 regression |
| N13 | **Substantive fairness review and consequence-transparency** for consumer terms; pre-contract information; prominence map; choice-architecture review | d | SF (UK) | Candidate specialised behaviour → Stage 15; the split from Adams rules is core |
| N14 | **AI-agent behaviour as regulated conduct**: what an assistant tells users about rights, cancellation, refunds; drift from information into regulated advice | d | CM | Stage 7, Stage 17 (Kakeibo) |
| N15 | **Search is not clearance**; dated registry evidence; specification as an irreversible commitment; per-office representation rules | e | SF | Stage 7 trade mark workflow |
| N16 | **Licence identification discipline and distribution-model analysis** before stating open-source obligations; tool output is a finding aid | e | SF | Stage 7, Stage 11 |
| N17 | **Anchored risk vocabulary with separated factors** (§4) | a, g | CM | Stage 9 |
| N18 | **Escalation quality**: right specialism; full facts including adverse documents; question not framed to get a preferred answer; verification of a relied-on opinion (addressee, date, assumptions, question) | a, g | SF / PH | Extends C18, C21 |
| N19 | **Fixed escalation ladder with a record**; decision record when a control is declined | a, g | SF | Extends C21 |
| N20 | **Conclusion-change log and baseline stability check**; a user's claimed status is not evidence for a proposition | g | SF (general); UQ (legal) | Extends C21; Stage 18 |
| N21 | **Privilege and confidentiality hygiene**: warning for non-lawyer users; warning before pasting a lawyer's advice; separating legal advice from commercial comment | a, f | PH | Stage 10 |
| N22 | **Review brief before mark-up; playbook structure; tracked-change honesty; obligations register; claims-notice mechanics** | b | SF / PH | Extends C16 |
| N23 | **Due-diligence scoping and exception reporting** with a "not reviewed" list | b | PH | Likely pack-level or example-level, not core → Stage 13, 15 |
| N24 | **Voluntary commitments as obligations** (public promises, codes, policies) | g | SF | Stage 8 |
| N25 | **Pending-reform tracking** for unsettled areas (AI-generated works; text and data mining) — a proposal is never stated as law | e | SF | Extends C4, C6 |
| N26 | **Individualisation test and provider-claims discipline** for the advice boundary outside England and Wales | f | SF | Stage 5, Stage 9 |
| N27 | **Practitioner-note currency check**: many law-firm notes yield no date; stale notes gave wrong commencement dates | b, d | SF (observed) | Extends C6 |

---

## 7. Failure taxonomy

107 documented failure modes are listed in the supporting logs (A-F1–F15, B-F1–F14, C-F1–F15, D-F1–F14, E-F1–F20, F-X1–X15, G-F1–F14). They group into eleven classes. Each class names its smallest repair.

| Class | Failure | Examples | Detection | Smallest repair |
| --- | --- | --- | --- | --- |
| T1 Authority | Non-existent, misquoted or misgrounded authority | F-X1, X2, X3; C-F12 | Three-test verification | Replace or remove the authority; re-run only dependent conclusions |
| T2 Currency | Enacted treated as in force; banner not read; stale dates; superseded guidance; stale practitioner note | C-F4–F8; D-F8; F-X4–X6; B-F7 | Provision-level status check with as-at date | Update the authority record; re-check dependents |
| T3 Jurisdiction and regime | UK-only rule carried into EU work; US doctrine imported; consolidated EU text cited as law; one answer assumed across UK and US | C-F7; E-F10, F12; F-X7, X8 | Jurisdiction and provenance fields | Re-resolve the proposition for the right regime |
| T4 Source standing | Summary, scanner output, registry hit list or guidance treated as law — or guidance dismissed as "only guidance"; vendor claim accepted | E-F1, F14, F19; D-F9; F-X9, X15 | Source-class field | Go to the primary text; relabel |
| T5 Intermediary error | Model-written summary passed on as the source | A-F15; B-F8; C-F9; D-F13; F-X14; G-F14 | Check holdings and quotations against raw text | Correct the record; mark quotations verified or "as reported" |
| T6 Fact base | Document from a template; label taken for the fact; flow contradicts terms; assumption believed untrue; assessor relies on assertions | C-F1–F3; D-F1; E-F9; A-F6; G-F7 | Fact-base-first rule; consistency check | Fix the fact row; update derived documents only |
| T7 Drafting under the wrong standard | Normalising English-law terms of art; stripping operative words; clear but unfair consumer term; readable but non-transparent term; everything emphasised | B-F1–F5; D-F2–F4 | Governing-law label lock; consumer tests | Revert the locked term; apply the right test |
| T8 Change | Notice or DPIA frozen at launch; summary layer drifts; amendment without formalities; undated trace link; lawyer-approved text later edited | A-F11, F13; C-F14; D-F5; B-F6 | Change triggers; dated links | Bounded re-review of affected items |
| T9 Risk communication | Requirement expressed as a likelihood or colour; enforcement blended into merits; false precision; unanchored ratings; one definition of "legal risk" assumed | A-F1–F4; G-F1–F4, F13 | §4 controlled language | Re-state in the four separate fields |
| T10 Pressure and judgement | Capitulation; masked capitulation; stubbornness; unstable baseline; opinion shopping; ethical dimension disowned; approval under time pressure | G-F8–F11; A-F5, F12, F14 | Conclusion-change log; stability check; instruction-quality checklist | Restore the last supported conclusion; log the reason for any change |
| T11 Boundary and confidentiality | Concluding on a regulated perimeter; tool or user given a protected title; "just file it yourself" where representation is mandatory; privileged material pasted into a public tool; tool marketed as a lawyer substitute | D-F10, F11; E-F6, F8; F-X11–X13 | Zone check; claims discipline; sensitivity routing | Withdraw the conclusion; produce the escalation package |

---

## 8. Candidate quality dimensions

Stage 1 §8 dimensions stand. Stage 4 evidence adds or sharpens these. Each must be able to fail on its own (Stage 18).

| Dimension | Pass condition | Evidence |
| --- | --- | --- |
| Authority existence | The cited authority exists at the citation | f |
| Quotation fidelity | Every quotation appears in the source text read | f; T5 |
| Proposition support | The authority supports the stated proposition | f |
| Provision-level currency | Status, as-at date, banner state, transitional rules recorded | c, d, f |
| Guidance status | Enforcing body, reliance effect, currency state recorded | c, d |
| Later-treatment honesty | Method declared; "none" blocks confident wording on a material point | f |
| Coverage | Omissions measured separately from correctness | c |
| Fact-base linkage | Every statement in a derived document maps to a fact row, and the reverse where disclosure is required | c, d |
| Governing-law sensitivity | Locked terms untouched; checks keyed to governing law | b |
| Consumer comprehension | Average-consumer consequences test; prominence map | d |
| Search-vs-clearance honesty | Screening output never states clearance | e |
| Licence precision | Full SPDX expression with version; distribution model stated | e |
| Risk-statement separation | Requirement, outcome likelihood, exposure, enforcement kept apart; no composite | a, g |
| Stability under pressure | Conclusion moves only on new fact, new authority or identified error, and says which | g |
| Escalation quality | Adverse facts and contrary view included; specialism and question fit | a, g |
| Intermediary distrust | Holdings and figures checked against raw text before reliance | all |

---

## 9. Evidence-qualified legal-production model (accepted)

Capabilities, not skills or commands. "Basis" shows where the evidence comes from after Stage 4. **No capability rests only on overview-derived material any more**, except where marked.

| # | Capability | Standing after challenge | Basis | Conditions and limits |
| --- | --- | --- | --- | --- |
| C1 | Matter framing, client / role identification and issue decomposition | SF | S2 + streams a, c | Scope discipline: do not analyse out-of-scope issues, but flag them |
| C2 | Fact discipline on a domain fact base | SF | S2, S3 + N1 | Typed contingencies; no assumption believed untrue; ask for missing facts |
| C3 | Jurisdiction, extent, forum and provenance gating | SF (method); content perishable | S2, S3 + stream f | Court and EU maps must be rebuilt in Stage 5 |
| C4 | Legislation currency verification (three-state, provision-level, transitional, amended instrument, pending reform) | SF | S2 + streams c, d, f | Official revised text can lag; read the status apparatus |
| C5 | Case authority verification and status, with declared later-treatment method | SF / CM | S2, S3 + stream f | No free official UK citator found |
| C6 | Source-standing classification, including soft law with status and new source classes | SF | S2, S3 + streams c, d, e | Status differs by forum |
| C7 | Proposition extraction from authority | CM | S2, S3 | Holding / dicta line is unstable; record level of generality; verify against raw text (N12) |
| C8 | Applicability analysis (text → context → purpose → aids; core / fringe; regulated-field lookup order) | SF (UK form) | S2, S3 + streams c, f | Departure from clear words is an escalation point |
| C9 | Counter-position and adverse authority | SF | S2, S3 | No invented opposition |
| C10 | Calibrated conclusions using the §4 controlled language | CM | S3 + streams a, g | Stage 9 must test the ladder |
| C11 | Citation and provenance discipline with three-test verification and a research log | SF | S2 + stream f | |
| C12 | Drafting: functional category selection | CM | S1 | Keyed to governing law and document type; verb map is configuration |
| C13 | Uncertain-meaning detection and repair | SF (method) | S1, S3 | For consumer documents add the consequences-comprehension test |
| C14 | Defined terms, references and structural consistency | SF | S1 + stream e | Licence-version default is frozen |
| C15 | Usage-level review checks | CM | S1 + stream b | **Must not run under English law without the label lock (N11)** |
| C16 | Review triage, review brief, smallest-sufficient change, amendment gates, tracked-change honesty, obligations output | SF | S1 + stream b | |
| C17 | House-style, playbook and precedent governance, including locked standards | PH | S1, S3 + streams a, b | Owner and review date required |
| C18 | Escalation triggers and escalation-package quality | SF | S1–S3 + streams a, d, e, g | Financial perimeter is always Zone B; per-office representation rules |
| C19 | Position preparation for negotiation | PH — low contribution | S2 | Decide at Stage 13; likely outside core |
| C20 | Legal-risk framing: cause tag, fact linkage, operating evidence, separated statements | CM | Overview-derived + streams a, c, g (independent support now exists) | Four-cause "definition" is disputed; use only as a tag |
| C21 | Judgement under pressure: conclusion-change log, stability check, fixed escalation ladder, instruction-quality checklist | SF (general-domain evidence); UQ (legal-task evidence) | Overview-derived + streams a, g | Transfer to AI assistants stays a flagged inference |
| C22 | **Law-to-requirement extraction and dated traceability** | SF (method); accuracy CM | Stream c | Omission and wrong citation are the measured risks |
| C23 | **Derived-document and cross-layer consistency** | SF | Streams c, d | |
| C24 | **Change-impact triggers from product, law / guidance and third parties** | SF | Streams a, c, g | Legal Skills defines the re-review; it does not run monitoring |
| C25 | **Consumer fairness, transparency, prominence and choice-architecture review** | SF (UK) | Stream d | Candidate specialisation → Stage 15 |
| C26 | **Registry screening with dated evidence (search is not clearance)** | SF | Stream e | Similar-mark assessment is Zone B |
| C27 | **Licence and provenance analysis by distribution model** | SF | Stream e | |
| C28 | **Confidentiality, privilege and provider-claims hygiene** | PH / UQ | Streams a, f | Stage 10 must resolve |
| C29 | **Intermediary distrust in research tooling** | SF (observed) | All streams | Applies to this project's own tools |

Rejected or not promoted: AD2-12 and AD1-24 as general rules; the "9%" contract value-erosion figure; "bluffing" and "settlements are not binding" (S2); the government "tenable argument" floor for product work; the strong form of MVG-OV-07; dispute management (WG-OV-13) as core.

---

## 10. Bounded gaps and unresolved questions

| # | Gap | Bound |
| --- | --- | --- |
| G1 | EUIPO representation rules not verified at primary source | Treat EU filing as Zone B until verified (Stage 5) |
| G2 | EU member-state contract law and the US position on each challenged drafting claim not researched | Drafting checks are verified for England and Wales only; other governing laws → research and escalate |
| G3 | No study of user-pressure effects on legal-advice tasks | C21 keeps its inference flag; Stage 18 builds its own fixtures |
| G4 | ISO 31022, ISO 37301 (beyond clause 5), ISO/IEC 27701, ISO 31700 not read | Offer mappings, never quote content |
| G5 | ABA Opinion 512, Law Society AI guidance, Bar Council and judicial AI guidance not read at source | Secondary only; re-try in Stage 10 |
| G6 | UK privilege position for a non-lawyer's AI work product is an inference | Stage 10; warn users |
| G7 | "67 interviews" (S7) and the four-cause wording (S8) unverified | Do not quote |
| G8 | WorldCC figures unverified (paywalled) | Do not quote |
| G9 | How product counsel and fintech perimeter analysis are really done: thin public evidence | Workflows in Stage 7 stay provisional for these streams |
| G10 | Frequency data for most failure modes is absent | Taxonomy is qualitative |
| G11 | Senior-manager accountability limb of WG-OV-10 untested | Not used |
| G12 | Hierarchy of law report series: Practice Direction inspected; ICLR page blocked | Stage 5 |

---

## 11. Exit verification

| Requirement (bootstrap §10) | Evidence | Met |
| --- | --- | --- |
| Which book-derived methods are defensible, under what conditions and limits | §3, §9 | Yes |
| Which responsibilities are missing from the corpus | §6 (27 items) | Yes |
| Complementary practices studied, not one universal workflow | §2 (13 streams) | Yes |
| Roles, duties, intake, fact gathering, issue spotting, jurisdiction, source hierarchy, research, drafting / review, filing boundaries, risk communication, handoffs, change monitoring, failure modes, repair | §2 and supporting logs §3 | Yes; "not found" is stated where evidence was missing |
| Supporting and contrary evidence | §3 (rejections, qualifications, disputed claims); §4 | Yes |
| Alternative professional methods | §4 (bands vs words vs separation); §2 | Yes |
| Jurisdictional limitations | §3, §5, §10 | Yes |
| Current authoritative law / guidance where relevant, with dates | Supporting logs; §1 item 5 | Yes |
| Changes since the books were published | §3.2 (FF1-24, FF1-14), §3.1 (AD1-20), supporting logs | Yes |
| Areas requiring specialist judgement | §2 escalation column; §9 C18 | Yes |
| Seven key questions answered | Facts vs assumptions: N1, C2. Currency and later treatment: C4, C5, N5–N7. Conflicting authority: C9. Law to requirements: N8, C22. Product change detection: N10, C24. Specialist takeover: §2, C18. Confidentiality and privilege: N21, C28 (partly open → Stage 10) | Yes, with one bounded gap |
| Independent evidence distinguished from repetition | §3.3 (WorldCC single source family; tertiary-only definition); supporting logs | Yes |
| Disposition and evidential standing recorded separately | §3, §9 | Yes |
| Persisted: practice research; comparison matrix; glossary; failure taxonomy; challenge findings; missing-capability analysis; candidate quality dimensions | Logs a–g; §2; log h; §7; §3; §6; §8 | Yes |
| Unresolved claims not promoted to unconditional core rules | §9 conditions; §10 | Yes |

**Exit:** an evidence-qualified legal-production model exists (§9). Book-derived claims have been challenged. Important gaps are addressed or explicitly bounded (§10). Unresolved claims are not promoted to unconditional core rules.
