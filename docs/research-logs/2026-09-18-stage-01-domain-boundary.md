# Stage 1 — Project Goal, Users and Professional Boundary

**Stage:** 1 of the Legal Skills bootstrap (v1.2)  
**Date:** 18 September 2026  
**Branch:** `feat/bootstrap-3`  
**Status:** Complete — accepted input for Stage 2  
**Governing section:** §7 of `2026-09-08-legal-skills-new-project-bootstrap-process.md`  
**Family rule applied:** `production-skills/docs/bootstrap/new-project-process.md` Stage 1 (seven charter questions)

This log persists the project charter, professional-boundary map, intended-user map, jurisdiction strategy, quality definition, review/escalation points and non-goals. It does not fix a skill count, a command list or a template catalogue.

---

## 1. Inputs read

| Input | Use |
| --- | --- |
| Bootstrap specification §1–§4, §7, §33 | Purpose, seed evidence, principles, Stage 1 requirements, initial non-goals |
| Bootstrap execution contract (17 Sep 2026) | Execution mechanics, evidence rules |
| `production-skills` family docs (fetched from `sb-dev/production-skills` on 18 Sep 2026): `new-project-process.md`, `domain-research-process.md`, specs `01` and `04` | Charter questions, ownership model, handoff model, Pactwright boundary |
| External sources in §2 below | Professional-boundary evidence |

Local supplied PDFs were inventoried (8 files under `books/`). They are **not** used as Stage 1 evidence. Their assessment belongs to Stage 2.

---

## 2. Evidence record

Retrieval method for all web sources: Claude Code `WebFetch` / `WebSearch`, 18 September 2026. `WebFetch` returns a model-processed rendering of the page. Quoted text below is as returned by that rendering. Each change-sensitive proposition must be re-resolved at matter execution.

Book rule reminder: nothing below is a live legal conclusion for any matter. These sources define **where the professional boundary lies for design purposes**.

| ID | Source | Type | Date / version | Location | Proposition used | Standing |
| --- | --- | --- | --- | --- | --- | --- |
| E1 | Legal Services Act 2007, s 12 — https://www.legislation.gov.uk/ukpga/2007/29/section/12 | Primary legislation (England and Wales) | Latest available (revised); page reports no known outstanding effects | s 12(1), s 12(3) | Six reserved legal activities: right of audience; conduct of litigation; reserved instrument activities; probate activities; notarial activities; administration of oaths. "Legal activity" also includes legal advice or assistance on the application of the law, which is **not** in the reserved list. | Supported finding |
| E2 | Legal Services Act 2007, s 14 — https://www.legislation.gov.uk/ukpga/2007/29/section/14 | Primary legislation | Latest available (revised); no known outstanding effects | s 14(1) | Carrying on a reserved legal activity when not entitled is a criminal offence. | Supported finding |
| E3 | Legal Services Board, "Reserved legal activities" FAQ — https://legalservicesboard.org.uk/enquiries/frequently-asked-questions/reserved-legal-activities | Oversight-regulator guidance | No page date shown (site copyright 2026) | Whole page | Confirms E1/E2. General legal advice or assistance is outside the reserved category. | Supported finding (repeats E1; not independent) |
| E4 | SRA, "Misuse of AI — Warning notice" — https://www.sra.org.uk/solicitors/guidance/misuse-ai/ | Regulator warning notice | Published 17 August 2026 | Whole notice | AI use does not diminish or transfer professional responsibility. Named authorities must be genuine, relevant and verifiable. Supervisors stay accountable. Client information enters AI systems only with appropriate contractual, technical and organisational safeguards. Public-tool input can put privilege at risk. Firms need governance, systems and controls. | Supported finding |
| E5 | Immigration and Asylum Act 1999, s 84 — https://www.legislation.gov.uk/ukpga/1999/33/section/84 | Primary legislation (UK) | Latest available (revised) as at 17 Sep 2026; page reports **outstanding changes not yet applied** (2025 c. 31 affecting s 84(3)(b), new s 84(3C)) | s 84(1)–(2) | "No person may provide immigration advice or immigration services unless he is a qualified person." | Supported finding; text currency qualified |
| E6 | Financial Services and Markets Act 2000, s 19 — https://www.legislation.gov.uk/ukpga/2000/8/section/19 | Primary legislation (UK) | Latest available (revised) as at 16 Sep 2026; page reports **outstanding changes not yet applied** | s 19(1) | The general prohibition: no regulated activity in the UK unless authorised or exempt. | Supported finding; text currency qualified |
| E7 | WebSearch results: IPReg (https://ipreg.org.uk/what-is-an-attorney), UK regulated-professions register (https://www.regulated-professions.service.gov.uk/professions/registered-trade-mark-attorney), CITMA | Regulator / government / professional body pages | Search-result level only; pages **not individually inspected** | — | "Registered Trade Mark Attorney" is a protected title. Applicants may file at the UK IPO without a representative. | Practical heuristic — discovery-level only; verify in Stage 4/5 |
| E8 | NCBE *Bar Examiner*, article on ABA Formal Opinion 512 — https://thebarexaminer.ncbex.org/article/fall-2024/generative-artificial-intelligence-tools/ | Secondary professional commentary (US) | Fall 2024; opinion dated 29 July 2024 | Whole article | The opinion applies existing duties (competence, confidentiality, communication, candour, supervision, fees) to generative-AI use. Uncritical reliance on output is a competence failure. Informed client consent is needed before client information goes into self-learning tools. | Context-dependent (secondary; the ABA primary page returned HTTP 403) |
| E9 | WebSearch results on US state-bar AI guidance and unauthorised practice of law (UPL) | Mixed secondary | 2026 | — | US jurisdictions treat applying law to a person's specific facts with a recommendation as the practice of law. The UK position (E1) is materially different. | Unresolved question — not inspected at source; hand to Stage 4 |
| E10 | J. Robinson, "The Role of Product Counsel", ACC Docket — https://corporatecounselnow.com/node/3533 (redirect from docket.acc.com/node/3533) | Practitioner article | 15 March 2023 | Whole article | Product counsel work across the whole product lifecycle, translate between legal and product teams, identify risk early, and source specialist guidance for knowledge gaps. | Practical heuristic |

### Failed retrievals (recorded honestly)

| URL | Result | Repair |
| --- | --- | --- |
| https://media.sra.org.uk/solicitors/guidance/misuse-ai/ (URL in the bootstrap specification) | HTTP 404 | Found the live notice at `www.sra.org.uk` (E4). The specification URL is stale. |
| https://www.americanbar.org/news/abanews/aba-news-archives/2024/07/aba-issues-first-ethics-guidance-ai-tools/ | HTTP 403 | Used secondary source E8; marked as secondary. |

### Contrary evidence and limits

- E1 shows that in England and Wales legal advice is **not** reserved. A design that refuses all advice-like output would be more restrictive than that jurisdiction requires.
- E9 indicates that at least some US jurisdictions draw the line differently (information vs advice). The boundary is therefore **jurisdiction-dependent**. One fixed global rule would be wrong in one direction or the other.
- E5 and E6 show that "unreserved under the Legal Services Act" does not mean "unregulated". Separate statutory perimeters exist (immigration advice; financial regulated activities). Others may exist (for example claims management, insolvency). Stage 4 must investigate them.
- E4 and E8 address regulated lawyers. They do not directly regulate a non-lawyer user of an AI tool. They are still the best available evidence of the professional standard of care that Legal Skills outputs must support.

---

## 3. Project charter

### 3.1 Production discipline owned

**Legal production:** turning project reality into scoped, authority-backed, time-qualified legal work product that a consuming project can act on and that a human reviewer can check.

### 3.2 Owned outcomes

| Outcome | Description |
| --- | --- |
| Scoped matter | A bounded legal question with material facts, assumptions, actors, jurisdiction and dates |
| Issue list | Legal issues spotted from project facts, with reasons |
| Verified authority record | Authorities that exist, match the jurisdiction, support the proposition and carry retrieval / valid-as-of data |
| Applicability analysis | Facts applied to authority, with uncertainty and counter-positions visible |
| Options, risks and recommendations | Framed for a decision-maker; not collapsed into one score |
| Legal requirements and constraints | Actionable by product, engineering, design and content teams |
| Legal drafts and reviews | Documents and redlines derived from actual product or transaction behaviour |
| Legal-product consistency findings | Mismatches between legal text and actual behaviour |
| Change-impact findings | Which legal work a project change invalidates |
| Escalation package | Question, facts, jurisdiction, authorities, analysis, conflicts, options and the exact decision required from a specialist |
| Legal evidence package | All of the above, valid as of a stated date |

### 3.3 Core responsibility decisions

The bootstrap asked whether each candidate belongs in core. Decisions below are **boundary decisions**, not skill or command decisions.

| Candidate responsibility | In core? | Reason | Limit |
| --- | --- | --- | --- |
| Legal scoping / issue spotting | Yes | Every matter starts here. Reusable across all matter classes. | Issue spotting outside proving matter classes flags and escalates; it does not analyse deeply. |
| Authoritative legal research | Yes | E4: unverified authority is the leading AI failure. | Core owns method and verification. It does not own a legal database. |
| Analysis / option framing | Yes | E1: not reserved in the first proving jurisdiction. Core value of the project. | Jurisdiction-dependent (E9). Human review points in §7 apply. |
| Drafting | Yes | Product-facing documents are a main consuming-project need. | Reserved instrument and probate documents are excluded (E1). |
| Review / redlining | Yes | Same reasoning as drafting; smallest-sufficient repair is a family principle. | Same exclusion. |
| Legal-product consistency | Yes | Distinguishes legal production from template generation (spec §4). | Needs project facts from the consuming project. |
| Legal change impact | Yes | Needed for bounded re-review. | Core defines the method. Pactwright owns lifecycle triggers when present. |
| Risk / uncertainty communication | Yes | E4, E8: false certainty is a professional failure. | No single numeric score by default. |
| Specialist escalation packaging | Yes | Makes the professional boundary useful rather than a disclaimer. | — |

### 3.4 What the project does not own

- Consuming-project product decisions, legal conclusions, matter records and risk acceptance.
- Pactwright lifecycle, Contracts and Evidence semantics (family spec `04` §8).
- Regulated professional status, representation, advocacy and reserved legal activities.
- Legal databases, registries and citators (execution layer; Stages 11–12).
- General evidence acquisition method (Deep Research candidate boundary; Stage 21).

### 3.5 Why the discipline is reusable

The chain `fact → issue → proposition → authority → applicability → conclusion → action` has the same shape for privacy, consumer, IP, licensing and AI-disclosure matters. The content changes. The production discipline does not. Matter specialisation is a Stage 15 Extension Pack question. Jurisdiction is execution context.

---

## 4. Professional-boundary map

Three zones. The zone depends on **activity + jurisdiction**, not on the area of law alone.

| Zone | Meaning | Examples | Required behaviour |
| --- | --- | --- | --- |
| A — Support freely | Legal-production work that is not reserved or separately perimetered in the matter jurisdiction | Scoping; issue spotting; research; authority verification; analysis; drafting and review of product-facing documents; consistency checks; trade mark knockout screening as **search evidence** | Produce the work. Keep verification, valid-as-of data and uncertainty visible. Never claim professional status. |
| B — Support with mandatory human review or specialist handoff | Work that is lawful to assist but where error cost, judgement or a filing/registration step justifies a qualified human | Trade mark clearance opinion and filing strategy; financial-regulatory perimeter questions (E6); novel AI/IP questions; material enforcement or litigation exposure; conflicting high-level authority; uncertain cross-border applicability; matters in a jurisdiction whose practice-of-law rule is unresolved (E9) | Produce preparatory work and an escalation package. State the exact decision the specialist must make. Do not present output as final advice. |
| C — Do not perform | Reserved or criminally perimetered activity, or claimed status | Conduct of litigation; rights of audience; reserved instrument, probate, notarial activities; administering oaths (E1, E2); immigration advice or services (E5); carrying on an FSMA regulated activity (E6); use of protected titles (E7); filing or representing as an agent | Refuse the activity itself. Explain the boundary. Offer Zone A/B preparatory work where that is lawful. |

Design consequences:

1. The boundary check needs the matter jurisdiction first. This confirms the spec principle "jurisdiction before rule application".
2. Zone C is a list of **activities**, not areas of law. A privacy matter can enter Zone C if it becomes litigation.
3. The Zone C list above is evidence-backed for England and Wales / UK only. Other jurisdictions need their own resolution at matter time. Stage 4 must test this and Stage 5 must model it.
4. Legal Skills is a tool used by a person. The user remains the accountable actor (E4 by analogy). Skills must never state or imply that the AI is a solicitor, barrister, trade mark attorney or other regulated professional.

---

## 5. Intended-user map

| User | Need | What Legal Skills gives | What the user must still own |
| --- | --- | --- | --- |
| Founder / product owner without in-house counsel | Understand legal issues in a product; get usable documents | Scoped analysis, requirements, drafts, clear escalation triggers | Decisions; risk acceptance; instructing a professional when Zone B/C applies |
| Engineer / designer in a consuming project | Actionable legal constraints | Requirements traced to authority; consistency findings | Implementation; reporting project changes |
| In-house or product counsel | Faster first-pass work that stays checkable | Authority tables, issue lists, redlines, change-impact findings | Professional judgement, supervision and sign-off (E4, E8, E10) |
| External specialist receiving an escalation | Efficient instruction | Escalation package | The specialist opinion |
| AI agents under Pactwright-governed delivery | Legal inputs to Contracts and Evidence | Legal requirements, constraints, review findings, verification inputs | Lifecycle gates stay with Pactwright |
| Other Production Skills (Software Engineering, UI/UX, Game Development, Video, Narrative, Music, Deep Research) | Legal constraints on their outputs; provenance checks | Handoff artefacts defined per family spec `04` §4 | Their own domain production |

Not intended users: a member of the public seeking representation in a dispute; anyone seeking a compliance certificate; anyone seeking Zone C activity.

---

## 6. Core matter classes and jurisdiction strategy

### 6.1 Core proving matter classes

Chosen because the seed evidence (spec §3) and both canonical stress tests (Kakeibo, Worldstack) need them, and because they are mostly Zone A/B work:

```text
privacy / data protection artefacts and consistency
consumer terms and digital-commerce flows
trade mark / brand screening (search evidence, not clearance)
copyright, content and asset licensing, provenance
open-source licence obligations
AI / automated-system disclosures
commercial contract drafting and review (general method)
```

These are **proving classes for the core method**. They are not a commitment that each becomes a skill or a pack. Stage 15 decides packs.

### 6.2 Not assumed to be core

Litigation, tax, criminal, family, immigration, employment, corporate transactions and patent prosecution. Core may **spot and escalate** issues in these fields. It does not own analysis in them. Immigration has a hard statutory perimeter (E5). Litigation conduct is reserved (E1).

### 6.3 Jurisdiction strategy

| Decision | Position |
| --- | --- |
| First proving jurisdiction | England and Wales / UK. All seed evidence and the boundary evidence in §2 are UK sources. |
| Second proving surface | EU instruments where a UK-origin product offers into the EU (privacy, consumer, AI). Used to prove cross-border handling, not full EU coverage. |
| Third reference | US federal / state sources only where a stress test needs them (for example USPTO search, US UPL boundary). Expect more Zone B outcomes. |
| All other jurisdictions | Core method still runs. Output must mark jurisdiction as unresolved or unverified and escalate. |
| Modelling rule | Jurisdiction is matter context resolved on every run. It is never a pack identity and never a directory tree. |
| Out of scope | A universal conflict-of-laws engine. |

---

## 7. Human review, commitment and escalation points

| Point | Who decides | Why |
| --- | --- | --- |
| Matter scope and jurisdiction accepted | User | Wrong scope invalidates all later work |
| Material facts and assumptions confirmed | User / consuming project | Only the project knows its real behaviour |
| Reliance on an unsettled or contestable interpretation | User, with counsel where exposure is material | Conclusion must not exceed certainty |
| Risk acceptance | User / project owner | Never the tool |
| Publication or execution of a legal document | User; qualified reviewer in Zone B | Commitment point; hard to reverse |
| Filing, registration, representation | Authorised person or the applicant personally | Zone B/C |
| Sending confidential or privileged material to any provider | User, before it is sent | E4: confidentiality and privilege risk |
| Zone C trigger | Mandatory handoff | E1, E2, E5, E6 |

Escalation must be specific: question, facts, jurisdiction, authorities, analysis, conflicts, options, exact decision required. A generic "consult a lawyer" line fails the quality definition.

---

## 8. Quality definition

Legal-production quality is multi-dimensional. The dimensions stay separate so that each can fail independently (needed later by Stage 18).

| Dimension | Pass condition |
| --- | --- |
| Fact discipline | Facts, assumptions and unknowns are distinguished; no invented project facts |
| Jurisdiction | Resolved, or explicitly unresolved |
| Authority | Exists; right type and jurisdiction; supports the stated proposition; primary/official preferred |
| Currency | Retrieved-at and valid-as-of stated; commencement, amendment and later treatment checked where material |
| Reasoning | Application is visible; counter-positions and exceptions shown where material |
| Calibration | Conclusion never more certain than facts, authority, jurisdiction or time allow |
| Actionability | Requirements can be acted on by the consuming project |
| Product consistency | Legal text matches actual behaviour |
| Repair economy | Smallest responsible unit repaired; verified unaffected work preserved |
| Boundary | No claimed professional status; Zone B/C handled correctly |
| Confidentiality | Tool routing matches sensitivity |
| Escalation usefulness | Package is specific and complete |

---

## 9. Interfaces

| Counterpart | Legal Skills receives | Legal Skills supplies | Owner of the rest |
| --- | --- | --- | --- |
| Consuming project | Product facts, data flows, commercial model, dependency manifests, assets, change notices | Legal requirements, constraints, drafts, reviews, consistency and change-impact findings, escalation packages | Project owns decisions, matter records and legal conclusions |
| Pactwright (optional) | Contract / change context | Legal requirements, constraints, review findings, verification inputs | Pactwright owns lifecycle, Contracts, Evidence semantics, gates |
| Deep Research | General evidence acquisition where useful | Legal authority, applicability and legal reasoning | Boundary confirmed at Stage 21 |
| Software Engineering / UI/UX / Game Development | Implementation facts, UI flows, dependency and asset lists | Traceable legal requirements and consistency findings | Those domains own implementation |
| Video / Narrative / Music | Asset provenance, references, likeness and licence facts | Licence, copyright, likeness and provenance constraints | Those domains own creative production |
| Central `production-skills` repo | Family contracts | Registry facts only | No consuming-project state stored centrally (family spec `04` §6) |

Handoff instances belong to the consuming project. Reusable handoff contracts are recorded only when later evidence supports them (Stages 21 and 27).

---

## 10. Non-goals

The initial non-goals in spec §33 are **confirmed** by Stage 1 evidence. Additions from this stage:

- not a provider of immigration advice or services (E5);
- not a person carrying on any financial regulated activity (E6);
- not a user of protected professional titles (E7);
- not a system with one fixed global advice boundary (E1 vs E9).

Deliberately **not decided** at this stage: skill count, command list, template catalogue, pack catalogue.

---

## 11. Questions handed to later stages

| # | Question | Stage |
| --- | --- | --- |
| Q1 | Which book-derived methods support scoping, research, reasoning, drafting, risk and escalation? | 2–3 |
| Q2 | How do US and EU member-state rules on practice of law / legal advice affect Zone A in those jurisdictions? Inspect primary sources. | 4, 5 |
| Q3 | Which other UK statutory perimeters exist beside E1, E5, E6 (for example claims management, insolvency)? | 4 |
| Q4 | Verify E7 at source: protected titles and self-filing at UK IPO, EUIPO, USPTO. | 4, 5 |
| Q5 | Read ABA Formal Opinion 512 at source if access allows; find equivalent Law Society / Bar Council / CCBE guidance. | 4 |
| Q6 | How does privilege apply to material processed by an AI tool used by a non-lawyer? | 4, 10 |
| Q7 | The specification's SRA URL is stale (404). Correct it when the specification is next revised with authority. Live URL: https://www.sra.org.uk/solicitors/guidance/misuse-ai/ | Maintenance |

---

## 12. Exit verification

Requirement source: spec §7 and family Stage 1.

| Requirement | Evidence in this log | Met |
| --- | --- | --- |
| Owned legal outcomes | §3.2 | Yes |
| Intended users | §5 | Yes |
| Core matter classes | §6.1–6.2 | Yes |
| Initial proving jurisdictions | §6.3 | Yes |
| Human review requirements | §7 | Yes |
| Regulated-practitioner handoffs | §4 (Zones B, C), §7 | Yes |
| Explicit non-goals | §10 | Yes |
| Reusable production vs project-specific knowledge | §3.4, §9 | Yes |
| Interfaces with Pactwright and other Production Skills | §9 | Yes |
| Nine candidate core responsibilities investigated | §3.3 | Yes |
| Litigation, tax, etc. not assumed core | §6.2 | Yes |
| Family charter questions (discipline, outcomes, non-ownership, adjacent skills, reusability, approval points, quality) | §3.1, §3.2, §3.4, §9, §3.5, §7, §8 | Yes |
| Persisted charter, boundary map, user map, jurisdiction strategy, quality definition, review/escalation points, non-goals | §3–§10 | Yes |
| No fixed skill count or template catalogue | §3.3 note, §10 | Yes |

**Exit:** a defensible legal-production boundary exists without a fixed skill count or template catalogue. Evidence limits are recorded in §2 and §11.
