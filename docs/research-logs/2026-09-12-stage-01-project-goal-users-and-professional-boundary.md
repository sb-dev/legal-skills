# Stage 1 — Project Goal, Users and Professional Boundary

**Project:** `legal-skills`  
**Bootstrap stage:** 1 — Define Project Goal, Users and Professional Boundary  
**Status:** Complete  
**Date:** 12 September 2026

## 1. Stage purpose

This stage defines what `legal-skills` owns before foundational-book selection, broader professional-practice research, jurisdiction modelling, workflow design, tool selection or skill decomposition begins.

The project is a Production Skills repository for reusable expertise that helps an agent perform **evidence-backed legal production for software, product, creative and Pactwright-governed projects**.

The core boundary is:

> `legal-skills` owns reusable legal-production judgement for scoping a matter, identifying legal issues, finding and verifying appropriate authority, analysing applicability, framing options and uncertainty, drafting or reviewing legal artefacts, tracing legal requirements into project reality, detecting legal change impact, and packaging work for human or specialist review.

It does not own the consuming project's product decisions, project facts, implementation, lifecycle governance, regulated professional status, reserved legal activities, court advocacy, filing representation or specialist substantive-law expertise that has not been researched and validated for the matter.

The project should make strong legal work more reproducible without pretending that an AI system becomes a solicitor, barrister, trade mark attorney or other regulated professional.

## 2. Canonical inputs reviewed

This charter is grounded in the current repository bootstrap and Production Skills family contracts:

- [`2026-09-08-legal-skills-new-project-bootstrap-process.md`](2026-09-08-legal-skills-new-project-bootstrap-process.md)
- [`production-skills/docs/bootstrap/new-project-process.md`](https://github.com/sb-dev/production-skills/blob/main/docs/bootstrap/new-project-process.md)
- [`production-skills/docs/specs/02-production-skills-project-contract.md`](https://github.com/sb-dev/production-skills/blob/main/docs/specs/02-production-skills-project-contract.md)
- [`production-skills/docs/specs/04-cross-domain-orchestration-and-integration.md`](https://github.com/sb-dev/production-skills/blob/main/docs/specs/04-cross-domain-orchestration-and-integration.md)

Bounded professional-practice and authoritative-source checks were performed only far enough to test the Stage 1 boundary:

- Legal Services Board, [Reserved legal activities](https://legalservicesboard.org.uk/enquiries/frequently-asked-questions/reserved-legal-activities)
- Solicitors Regulation Authority, [Misuse of AI — Warning notice](https://media.sra.org.uk/solicitors/guidance/misuse-ai/), published 17 August 2026
- Competition and Markets Authority, [Unregulated legal services: Consumer protection law guidance](https://www.gov.uk/government/publications/unregulated-legal-services-consumer-protection-law-guidance/unregulated-legal-services-consumer-protection-law-guidance)
- Legal Services Board, [AI in legal services: consumer expectations and existing standards](https://legalservicesboard.org.uk/research-2/ai-in-legal-services-consumer-expectations-and-existing-standards), published 10 June 2026
- Information Commissioner's Office, [Right to be informed](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/individual-rights/individual-rights/right-to-be-informed/)
- Competition and Markets Authority, [Unfair contract terms](https://www.gov.uk/government/publications/unfair-contract-terms-cma37), updated 22 July 2026
- UK Intellectual Property Office, [Register a trade mark: Before you apply](https://www.gov.uk/how-to-register-a-trade-mark/before-you-apply)
- UK Government / DSIT / DCMS / IPO, [Report and impact assessment on Copyright and Artificial Intelligence](https://www.gov.uk/government/publications/report-and-impact-assessment-on-copyright-and-artificial-intelligence), published 18 March 2026

This is not Stage 2 book selection and not Stage 4 professional-practice challenge research. No foundational corpus, fixed skill list or complete substantive-law model is claimed here.

## 3. Bounded professional-practice observations

### 3.1 Legal production is not document generation

The initial evidence reinforces the bootstrap premise that legal output must be derived from the actual matter.

A privacy notice cannot be treated as correct independently from the processing it describes. ICO guidance requires privacy information to reflect matters such as purposes, lawful basis, recipients, transfers, retention, rights and automated decision-making where applicable, and it expects information to be reviewed and updated when processing changes.

Consumer terms likewise cannot be validated only as prose. The CMA's current unfair-contract-terms guidance evaluates fairness and transparency in context, including what is sold, related terms and the circumstances in which the term is agreed.

Trade mark work also depends on territory, relevant goods/services, classification and similarity evidence. The IPO explicitly requires applicants to select relevant classes and check for identical or similar marks, and recommends professional advice when similar marks are found.

The reusable production problem is therefore broader than drafting:

```text
project reality
→ legal scope
→ legal proposition
→ authority
→ applicability
→ obligation / right / risk / option
→ project requirement or legal artefact
→ implementation / behaviour consistency
→ review and change impact
```

A polished document without that chain is not a sufficient legal-production outcome.

### 3.2 AI output is evidence to inspect, not legal authority

The SRA's 17 August 2026 warning notice identifies fabricated or inaccurate legal material and confidentiality failures as concrete AI risks. It states that regulated professionals remain accountable for work produced through AI, must verify authorities and must maintain appropriate supervision and safeguards.

`legal-skills` therefore needs an invariant stronger than a generic hallucination warning:

```text
model output
≠ authority
≠ verified legal proposition
≠ professional approval
```

Legal propositions must be traceable to sources appropriate to their evidential role, and material authorities must be checked rather than merely cited by a model.

The system should support authorised professionals, but it must not imply that using the repository transfers their professional responsibility to the model or repository.

### 3.3 The professional boundary is activity-based, not disclaimer-based

England and Wales distinguishes reserved legal activities from other legal services. The Legal Services Board identifies six reserved activities under the Legal Services Act 2007: rights of audience, conduct of litigation, reserved instrument activities, probate activities, notarial activities and administration of oaths.

The boundary must therefore not be reduced to:

```text
"not legal advice"
```

A disclaimer cannot convert an unauthorised reserved activity into a permitted activity, create professional privilege, confer regulated status or remove duties created by the actual service being provided.

The CMA's guidance to unregulated legal-service providers is particularly useful as a design constraint: providers must be clear about the nature and limits of their service, must not imply regulatory protections that do not exist, and should identify when another professional is needed. It also notes that non-reserved legal services can exist outside the regulated legal-services framework.

The repository should therefore describe what it actually does and where its outputs require review rather than using a blanket disclaimer as a substitute for a professional-boundary model.

### 3.4 Public consumer legal tools require a stricter service boundary

The Legal Services Board's June 2026 research on AI-powered legal tools found strong consumer expectations around accuracy, informed consent before consequential action, human oversight, redress and personal-data protection.

This does not mean the core repository should become a consumer-lawtech product. It means the default deployment posture should be **internal or project-team legal production support**.

If a consuming project exposes Legal Skills directly to consumers as a legal-information or legal-support service, that deployment becomes a separate legal/product matter requiring explicit analysis of:

- service claims and marketing;
- regulatory status;
- consumer protection;
- human oversight;
- consequential actions;
- redress;
- data handling;
- jurisdiction-specific restrictions.

Direct-to-consumer lawtech is therefore not an assumed core delivery model.

### 3.5 Jurisdiction and time are part of correctness

The initial sources already show why durable prompts cannot encode apparently universal conclusions.

Examples include:

- the ICO noting that guidance is under review following the Data (Use and Access) Act;
- CMA unfair-contract-terms guidance updated on 22 July 2026;
- UK government copyright-and-AI policy work published on 18 March 2026;
- trade mark rights depending on selected goods/services and territorial registration.

A correct legal-production workflow must preserve at least:

```text
matter jurisdiction / legal system
relevant actor locations
market / user territory
matter date
source date
law effective / commencement date where material
amendment / repeal / later treatment where material
retrieved-at date
analysis valid-as-of date
```

The core can provide the method for resolving those fields. It must not pretend one jurisdiction's answer is a global answer.

### 3.6 Product consistency is a core differentiator

The target repository is most useful when it can bridge legal analysis and project reality without taking over the project.

Examples:

```text
privacy requirement
↔ actual data flow / processor / retention / user control

consumer cancellation rule
↔ purchase flow / renewal / cancellation implementation

licence obligation
↔ dependency / content / distribution behaviour

trade mark constraint
↔ proposed product name / territory / goods and services

AI disclosure requirement
↔ actual automated behaviour and user-facing experience
```

This legal-to-project consistency work is reusable and belongs in core. The implementation itself remains with the consuming project and the relevant Production Skills family.

## 4. Project charter

### Mission

Make rigorous, traceable legal-production practice installable for AI agents so they can support project teams with verified legal research, analysis, drafting, review and change-impact reasoning without impersonating regulated legal professionals.

### The project owns

```text
matter intake and legal scoping
→ jurisdiction / actor / date resolution
→ material-fact and assumption inventory
→ issue spotting
→ legal-research strategy
→ authority retrieval and verification
→ proposition extraction
→ applicability analysis
→ options / obligations / rights / risks
→ uncertainty and evidence-strength communication
→ legal drafting where appropriate
→ contract / policy / notice review and redlining
→ legal-to-product consistency checks
→ project requirement traceability
→ legal change-impact analysis
→ adversarial legal review
→ bounded correction
→ specialist escalation package
→ valid-as-of evidence package
```

### Core responsibility decision

Stage 1 resolves the bootstrap's candidate responsibilities as follows:

| Candidate responsibility | Core decision | Boundary |
| --- | --- | --- |
| Legal scoping / issue spotting | **Core** | Identify issues and missing facts; do not invent facts or decide project strategy. |
| Authoritative legal research | **Core** | Prefer primary/authoritative sources and preserve evidential role; generic web summaries are not authority by default. |
| Analysis / option framing | **Core** | Separate rule, facts, application, uncertainty and options; do not present model confidence as legal certainty. |
| Drafting | **Core** | Draft from established matter facts and authority; publication/execution may require human or specialist approval. |
| Review / redlining | **Core** | Review against matter goals, authority, risk and project reality; preserve acceptable text and target the failing clause or issue. |
| Legal-product consistency | **Core** | Compare legal artefacts and obligations with actual product behaviour; implementation remains with the owning project/domain. |
| Legal change impact | **Core** | Identify affected legal conclusions, requirements and artefacts when law, facts or product behaviour changes. |
| Risk / uncertainty communication | **Core** | Keep factual, authority, jurisdictional, temporal and interpretive uncertainty inspectable; no single magic score. |
| Specialist escalation packaging | **Core** | Produce a precise handoff containing the question, facts, sources, analysis, disagreement/uncertainty and decision required. |
| Regulated representation / reserved activity | **Not core execution** | Detect and escalate; do not claim authorisation or silently perform a reserved role. |
| Court advocacy / litigation conduct | **Not core execution** | Research/support may be possible under an authorised workflow; representation and conduct remain outside autonomous core. |

### The project does not own

```text
whether a product should be built
commercial strategy or pricing decisions
project requirements as the source of truth
software implementation
UI/UX design
creative production
Pactwright lifecycle or Project Graph governance
the consuming project's research archive
regulated professional identity
a solicitor-client or barrister-client relationship
legal professional privilege by default
reserved legal activities by an unauthorised system
court or tribunal representation
filing authority before registries or regulators
client-money handling
universal substantive law for every jurisdiction
specialist matter competence merely because a question is legal
```

### Boundary test

A reusable capability belongs in `legal-skills` when it primarily answers:

> Given a defined matter, its facts, jurisdiction, date and project context, what legal issues matter, what authority supports the relevant propositions, how do those rules apply, what uncertainty remains, what project action or legal artefact follows, and what level of review is required?

If the capability instead decides the product roadmap, implements the control, operates the project's lifecycle, represents someone before a court/registry, or requires specialist legal competence not yet validated for core, it belongs elsewhere or requires escalation.

## 5. Intended users

### Primary users

The repository should support:

- founders and product owners who need structured legal-production work around a real product or service;
- engineers, designers and creators who need legal requirements translated into inspectable project constraints;
- legal operations and in-house legal teams using AI for research, drafting, review and traceability;
- solicitors, barristers, trade mark attorneys and other authorised professionals using AI under their own professional duties and supervision;
- AI agents and coding/production agents that need a disciplined legal capability rather than ad-hoc prompting;
- multidisciplinary projects that need reusable legal production alongside Software Engineering, UI/UX, Narrative, Video, Music, Game Development, Deep Research or other Production Skills;
- Pactwright-governed projects that need legal analysis and evidence while Pactwright retains lifecycle authority.

### Secondary users

The repository may also help non-lawyer project contributors understand legal issues and prepare questions, evidence and draft artefacts for review.

It should not require users to be lawyers, but it must make the limits of the output and the required approval path explicit.

### Default service posture

The default posture is:

```text
internal/project legal-production support
```

not:

```text
autonomous public legal adviser
or
regulated law firm replacement
```

A consumer-facing legal-service use case must be treated as an explicit deployment context with its own legal and product analysis.

## 6. Core matter classes

The core should be organised around reusable legal-production work, not a fixed catalogue of document templates.

The following matter classes are appropriate initial proving ground because they recur across software, product and creative projects and expose the legal-to-project traceability problem.

### 6.1 Product and service launch/change review

Examples:

- new feature or service launch;
- change in business model;
- new market or territory;
- new data use;
- new content or user-generated-content capability;
- changed subscription, cancellation or refund behaviour;
- new AI-assisted functionality.

Core value: scope the legal impact and derive project requirements before drafting isolated documents.

### 6.2 Consumer terms, notices and commercial promises

Examples:

- consumer terms of service;
- subscription terms;
- cancellation/refund conditions;
- product notices;
- material disclaimers or eligibility conditions.

Core value: test the terms against the actual commercial/product behaviour and relevant fairness/transparency requirements.

### 6.3 Privacy, data protection and tracking

Examples:

- privacy notices;
- data-flow/legal-basis mapping;
- retention and recipient analysis;
- cookie/tracking requirements;
- processor/controller questions;
- automated-decision or profiling disclosures where relevant.

Core value: keep legal artefacts synchronized with actual processing rather than treating the privacy notice as the source of truth.

### 6.4 Intellectual property, content rights and branding

Examples:

- copyright ownership/licensing questions;
- AI/content provenance questions;
- open-source and third-party licence obligations;
- trade mark knockout/search preparation and risk framing;
- brand-use constraints;
- content permissions and rights chains.

Core value: distinguish evidence, ownership assumptions, territory, scope and professional filing/clearance decisions.

### 6.5 Product-facing commercial agreements

Examples:

- NDAs;
- supplier/vendor terms;
- data-processing terms;
- software/service agreements;
- content or licence agreements;
- straightforward partnership/commercial clauses linked to project delivery.

Core value: review obligations, allocation of risk, operational feasibility and implementation consequences.

High-value, unusual, heavily negotiated or transaction-structuring work should escalate rather than being treated as automatically covered because the document is a contract.

### 6.6 AI/product governance and legal change impact

Examples:

- mapping new AI behaviour to disclosure, data, copyright or consumer issues;
- checking whether a regulatory/guidance change affects existing product requirements;
- identifying which legal artefacts and implementation controls are invalidated by a changed fact or rule.

Core value: maintain traceability between law, interpretation, project requirements and implemented behaviour.

## 7. Matters outside the default core

The project must not claim competence across all legal domains merely because its research method is reusable.

The following are **not initial core matter classes** and should require specialist treatment, a researched Extension Pack or explicit professional handoff before mature support is claimed:

- litigation strategy and conduct;
- criminal law;
- family law;
- immigration advice/services;
- tax advice;
- employment disputes and specialist employment matters;
- conveyancing and land transactions;
- probate and estate administration;
- insolvency proceedings;
- financial-services regulatory advice;
- sanctions / export-control specialist advice;
- competition/antitrust investigations or merger control;
- complex corporate finance, M&A or securities transactions;
- patentability opinions and patent prosecution;
- formal legal opinions intended for reliance by third parties;
- court, tribunal, registry or regulator representation requiring authorisation.

Some of these domains may later justify Extension Packs or adjacent projects. Stage 1 only prevents them from silently inflating the core.

## 8. Professional-boundary map

### 8.1 Work the core may perform autonomously within a project

Subject to source access, confidentiality and matter scope, the core may:

- structure the matter and identify missing facts;
- identify candidate legal issues;
- search for and retrieve authoritative sources;
- verify citations and extract propositions;
- distinguish authority from commentary;
- build issue, authority and applicability tables;
- compare law/guidance with project artefacts;
- identify inconsistencies and change impact;
- draft internal research notes, checklists, clause inventories and preliminary text;
- compare/redline text and explain the legal significance of changes;
- prepare options, uncertainties and questions for human review;
- package evidence for an authorised professional or specialist.

These outputs remain subject to the review level appropriate to the matter.

### 8.2 Human approval points

A human with authority for the project should approve before the system causes or represents a material external commitment, including normally:

- publishing or materially changing consumer-facing legal terms/notices;
- executing or accepting a contract;
- choosing a position where the legal analysis presents material alternatives or uncertainty;
- making a representation to a regulator, registry, court, counterparty or user population;
- taking a consequential step based on an unresolved legal assumption;
- intentionally accepting a material legal risk;
- disclosing confidential or privileged material to an external tool/provider;
- implementing a legal requirement where the project owner has not accepted the product/commercial consequence.

Human approval is a project-authority requirement. It does not by itself mean specialist legal review is unnecessary.

### 8.3 Specialist/authorised-practitioner handoff points

Escalate when any of the following applies:

```text
reserved legal activity may be implicated
court / tribunal conduct or advocacy is required
filing or representation requires authorised status
similar trade marks create a material clearance/filing decision
material litigation or dispute strategy is required
high-consequence bespoke contract or transaction risk is unresolved
cross-border conflict-of-laws or local-law analysis is material
substantive-law competence falls outside validated core coverage
material authority is conflicting, missing or genuinely ambiguous
facts are too incomplete for a responsible conclusion
regulated-sector specialist rules drive the outcome
vulnerable consumers or severe personal consequences materially raise the review threshold
formal opinion / reliance by third parties is requested
```

The handoff should not be a vague instruction to "ask a lawyer". It should carry the work already completed:

```text
question
+ material facts and assumptions
+ jurisdiction/date
+ issue list
+ authorities checked
+ competing interpretations
+ project constraints
+ precise decision required
```

### 8.4 No automatic privilege claim

The repository must not assert that material is legally privileged merely because it was generated for legal work or passed through an AI system.

Where privilege or confidentiality matters, the workflow must identify it as a legal/professional issue, restrict tool handling appropriately and obtain specialist guidance where necessary.

## 9. Initial jurisdiction strategy

### 9.1 Core method is jurisdiction-parametric

The reusable core should encode **how to resolve law**, not embed one jurisdiction as universal truth.

Each substantive matter should establish, where material:

```text
legal system / jurisdiction
relevant territory
actor location / establishment
user or customer location
market offered into
asset / right territory
governing law / forum if contractual
matter date
analysis valid-as-of date
```

The core should stop rather than silently assume jurisdiction when the answer materially affects the conclusion.

### 9.2 Primary proving context: England & Wales with relevant UK-wide regimes

The first proving context should be **England & Wales**, using UK-wide statutes, regulators or registration systems where the matter itself operates at UK level.

Reasons:

- the professional-boundary framework under the Legal Services Act 2007 is explicit and inspectable;
- the SRA and Legal Services Board provide current evidence on AI-supported legal services and supervision;
- the ICO, CMA and UK IPO provide authoritative material for the initial product/privacy/consumer/IP matter classes;
- Kakeibo and other software/product stress tests can be framed realistically in a UK launch context;
- it creates a bounded legal system before cross-border complexity is introduced.

This must not be labelled simply "UK law" when Scots or Northern Irish law could differ materially.

### 9.3 Secondary proving layer: European Union law for cross-border digital products

A second proving layer should test the ability to switch and compose legal sources when a UK-origin product is offered into the EU/EEA.

The purpose is **not** to claim that "EU law" replaces Member State law. Instead it should prove that the system can:

- distinguish EU-level legislation/guidance from domestic UK law;
- detect when Member State implementation, procedure, consumer law, enforcement or local advice is required;
- avoid carrying UK conclusions across the border by analogy;
- preserve separate authority chains and valid-as-of dates.

A particular Member State should be selected only when a proving matter requires it. Stage 1 therefore does not nominate a universal EU Member State.

### 9.4 Deferred jurisdictions

United States federal/state law, other common-law systems and other international contexts remain valid future targets, but should not expand the core before the England & Wales/UK baseline and cross-border switching behaviour are proven.

Jurisdiction-specific knowledge should later be represented through researched references, Extension Packs or matter-local research rather than hidden assumptions in generic prompts.

## 10. Owned legal outcomes

A mature `legal-skills` installation should be able to help produce the following outcomes without claiming professional authorisation:

1. turn a project change or legal question into a bounded matter with explicit actors, facts, assumptions, jurisdictions and dates;
2. identify the legal issues that materially affect the project rather than producing an exhaustive list of everything remotely legal;
3. build a research plan that prioritises authoritative sources and records why each source matters;
4. verify that cited authorities exist and support the propositions attributed to them;
5. distinguish binding law, persuasive authority, regulator guidance, official registry evidence, government guidance and secondary commentary;
6. express legal propositions separately from facts, assumptions, application and conclusions;
7. identify when an apparently relevant rule does not apply because of scope, actor, territory, date or factual conditions;
8. communicate uncertainty without converting it into false precision or a single opaque risk score;
9. derive actionable project requirements from the analysis while preserving the reasoning and source chain;
10. draft or revise legal artefacts from actual project facts and accepted positions rather than generic templates;
11. review/redline an artefact while preserving acceptable language and isolating the clauses or issues that require repair;
12. test whether terms, privacy information, licence obligations, disclosures or other legal artefacts match implemented project behaviour;
13. detect when a changed law, authority, fact, product flow or business decision invalidates dependent legal conclusions or artefacts;
14. preserve unaffected verified work while repairing only the dependent legal units;
15. stop before reserved, regulated or high-consequence work exceeds the system's validated boundary;
16. prepare a compact, evidence-rich escalation package for a qualified specialist;
17. produce a final evidence package that records the analysis valid-as-of date and important unresolved limitations.

## 11. Quality definition

Legal quality must remain multidimensional. Passing a citation check or producing polished prose is insufficient.

The core quality dimensions are:

### 11.1 Scope correctness

- the matter is defined at the right level;
- actors, decisions and intended outcomes are explicit;
- adjacent issues are excluded or escalated rather than silently absorbed.

### 11.2 Factual adequacy

- material facts are sourced from the consuming project or other evidence;
- assumptions are visible;
- missing facts capable of changing the outcome are identified.

### 11.3 Jurisdiction and temporal validity

- the relevant legal system/territory is explicit;
- sources are evaluated for the relevant date;
- commencement, amendment, repeal, later guidance or later treatment is checked where material.

### 11.4 Authority quality

- authoritative/primary sources are preferred where available;
- source type and legal weight are not collapsed together;
- citations are verified;
- commentary is not promoted into law merely because it is well written.

### 11.5 Applicability reasoning

- rule elements and conditions are matched to facts;
- contrary authority or scope limitations are considered;
- inference is distinguishable from sourced proposition.

### 11.6 Legal-to-project consistency

- requirements and artefacts match actual product/commercial behaviour;
- legal documents do not claim controls, rights or practices that the project does not implement;
- project changes trigger legal re-evaluation where dependencies exist.

### 11.7 Drafting and review quality

- text is accurate to accepted analysis and facts;
- obligations, rights and consequences are intelligible;
- ambiguity and internal inconsistency are detected;
- redlines preserve unaffected approved work where possible.

### 11.8 Uncertainty and risk calibration

Keep separate dimensions such as:

```text
factual completeness
authority strength
jurisdiction certainty
temporal currency
interpretive uncertainty
potential harm / exposure
reversibility
need for specialist review
```

Do not hide them behind one universal "legal risk score".

### 11.9 Professional-boundary correctness

- outputs do not imply a regulated title or protection that does not exist;
- review and escalation are proportional to the matter;
- reserved or specialist work is detected before execution crosses the boundary.

### 11.10 Confidentiality and evidence handling

- sensitive information is handled according to the tool/provider context;
- source provenance is preserved;
- the system does not assume that confidentiality or privilege survives a disclosure merely because the disclosure served legal analysis.

## 12. Review and escalation model

Use the cheapest responsible level that can resolve the matter.

### Level A — autonomous research/analysis support

Suitable for:

- matter structuring;
- source discovery;
- authority tables;
- citation verification;
- factual/assumption inventories;
- internal comparisons;
- change-impact discovery;
- preliminary drafting where no external commitment occurs.

### Level B — project-owner approval

Required when the legal work changes product behaviour, public text, commercial position or another externally meaningful project commitment.

### Level C — legal specialist review

Required when legal judgement is materially consequential, the source/application problem remains uncertain, the matter falls into a specialist domain, or professional reliance is expected.

### Level D — authorised-practitioner execution

Required where law or professional rules require an authorised person, reserved activity, filing representative, advocate or other regulated role.

The levels are escalation categories, not maturity scores. One matter may move between them as facts and intended actions change.

## 13. Interfaces with adjacent Production Skills

Cross-domain composition should use explicit handoffs rather than duplicate domain expertise.

| Adjacent discipline | Adjacent discipline owns | Legal Skills owns | Typical handoff |
| --- | --- | --- | --- |
| Deep Research Skills | general evidence/research production, broad source discovery methods, research synthesis | legal source hierarchy, legal authority, jurisdiction/date applicability, proposition verification and legal conclusions | Legal Skills may delegate broad discovery while retaining legal evidential judgement. |
| Software Engineering Skills | architecture, implementation, tests, software change evidence | legal requirements, constraints, legal-to-implementation traceability and legal change impact | legal requirement → implementation; code/config evidence → legal consistency review |
| UI/UX Design Skills | user research, information architecture, interaction/visual design, usability | legal content requirements, disclosure/consent constraints, fairness/transparency legal questions | legal requirement → UX design; tested UX behaviour → legal review |
| Business Building Skills | business model, commercial strategy, pricing, market and operating model | legal consequences, constraints, contract/regulatory issues and option framing | proposed business model → legal analysis; legal constraint → business decision |
| Narrative / Video / Music / other Creative Skills | creative intent and production | rights, permissions, provenance, licence and distribution constraints | planned/created asset → legal rights analysis; legal constraint → creative production decision |
| Game Development Skills | game design/runtime/game-specific production | legal issues affecting product, content, users, monetisation and rights | design/monetisation behaviour → legal scope; legal constraints → game/product implementation |
| QA / evaluation capabilities | integrated product validation and behaviour evidence | legal correctness criteria and legal-to-product consistency checks | implementation evidence → legal compliance review; legal requirement → acceptance condition |
| Pactwright | lifecycle, Project Graph, approvals, orchestration and consuming-project state | reusable legal-production capability and legal artefacts/evidence | Pactwright provides project context/authority; Legal Skills returns conclusions, requirements, evidence and escalation needs |

### Pactwright boundary

`legal-skills` must remain independently usable without Pactwright.

When Pactwright is present:

```text
Pactwright
→ owns lifecycle, project state and approval topology

Legal Skills
→ consumes the relevant project snapshot / artefacts
→ performs legal production
→ returns requirements, constraints, legal artefacts, evidence and unresolved decisions

Pactwright / consuming project
→ decides how those outputs affect the Project Graph and delivery plan
```

Legal Skills must not maintain a competing universal legal Project Graph or silently mutate consuming-project lifecycle state.

## 14. Reusable legal knowledge vs project-specific legal knowledge

This boundary is critical for keeping the repository useful across projects.

### Reusable and appropriate for Legal Skills

```text
legal scoping methods
issue-spotting methods
source hierarchy / authority handling
citation verification
applicability reasoning
legal research records
risk / uncertainty communication
legal drafting and review methods
traceability methods
change-impact methods
escalation methods
jurisdiction-specific validated reference material
Extension Pack behaviour that has been researched as reusable
```

### Project-specific and owned by the consuming project

```text
its users and markets
its actual data flows
its commercial model
its contract counterparties
its selected product name
its dependencies and licences
its accepted legal positions
its implemented controls
its correspondence and negotiations
its internal risk appetite
its legal-provider relationships
its matter-specific confidential facts
its lifecycle and approval history
```

Legal Skills may inspect or transform project-specific evidence during a run. It does not become the authoritative store for those facts merely because it analysed them.

## 15. Explicit non-goals

Stage 1 rejects the following as core goals:

- a generic "AI lawyer" persona;
- replacing regulated legal professionals;
- guaranteeing legal compliance;
- a universal jurisdiction engine;
- a global legal knowledge base embedded in prompts;
- one fixed legal-risk score;
- a template library presented as the legal workflow;
- one skill per document type;
- one skill per book;
- automatically filing trade marks, court papers or regulatory submissions;
- autonomous litigation, advocacy or negotiation with legal effect;
- storing all consuming-project legal state in this repository;
- duplicating software, product, UX, research or creative production skills;
- making Pactwright mandatory;
- assuming public AI tools are acceptable for confidential or privileged material;
- treating a disclaimer as a substitute for proper professional boundaries;
- claiming that five foundational books will provide current substantive law for live matters.

## 16. Stage 1 decisions

The following decisions are accepted for later bootstrap stages:

1. **Legal Skills is a legal-production system, not a legal-template library.**
2. **Core scope includes scoping, issue spotting, authoritative research, applicability analysis, option/risk framing, drafting, review/redlining, project consistency, legal change impact and escalation packaging.**
3. **The system may support both lawyers and non-lawyers, but it never claims regulated professional status.**
4. **Professional boundaries are determined by activity, jurisdiction, service model and consequence; a disclaimer alone is not a boundary.**
5. **Reserved/authorised activity and specialist high-consequence judgement require explicit handoff.**
6. **The default delivery posture is internal/project legal-production support, not autonomous direct-to-consumer legal advice.**
7. **England & Wales is the first legal-system proving context, using relevant UK-wide authorities where appropriate.**
8. **EU-level law is the first cross-border proving layer; Member State law must be selected when material rather than assumed away.**
9. **Initial substantive proving matters centre on digital/software/creative products: consumer terms, privacy/data, IP/rights/branding, product-facing commercial agreements and AI/product change impact.**
10. **Litigation, tax, immigration, family, criminal, probate, conveyancing, patent prosecution and other specialist domains are not silently core.**
11. **Legal correctness includes jurisdiction and valid-as-of time.**
12. **Legal-to-product traceability is core, while implementation remains with the consuming project and adjacent Production Skills.**
13. **Quality is multidimensional; no universal legal-quality or risk score is accepted.**
14. **Human approval is required before material external legal/commercial commitments; specialist review is triggered separately by competence, uncertainty, consequence or regulated activity.**
15. **Project-specific facts and legal decisions remain owned by the consuming project.**

## 17. Implications for Stage 2 book selection

Stage 2 should select exactly five complementary foundational books against the boundary established here.

The corpus should collectively strengthen durable method across dimensions such as:

```text
legal research and source evaluation
legal reasoning / applicability
legal drafting and contract review
professional judgement / risk / ethics / supervision
legal operations / product counsel / requirement traceability
```

These are coverage dimensions, not one-book-per-slot requirements.

The selection should avoid a corpus dominated by substantive doctrine for one jurisdiction because live legal propositions must still be resolved from current authority.

A book may be valuable for durable legal method even if it is not itself authoritative law. Conversely, a respected substantive-law text must not be treated as current authority merely because it is foundational.

Stage 2 must therefore preserve the distinction:

```text
books
→ durable legal-production method and professional practice

authoritative current sources
→ proposition actually applicable to the matter and date
```

No book is selected by this Stage 1 log.

## 18. Deferred questions

The following are intentionally deferred rather than unresolved blockers:

- exact five-book corpus — Stage 2;
- direct book extraction and reconciliation — Stage 3;
- comprehensive professional-practice challenge — Stage 4;
- detailed jurisdiction, authority hierarchy and temporal-validity data model — Stage 5;
- matter/fact/issue/reasoning artefact schemas — Stage 6;
- legal workflow stages and repair loops — Stage 7 onward;
- precise legal-to-project dependency model — Stage 8;
- risk/escalation implementation detail — Stage 9;
- confidentiality/privilege execution controls — Stage 10;
- legal databases, registries, AI skills and tools — Stage 11;
- execution providers — Stage 12;
- exact skill count and command model — Stage 14;
- Extension Pack catalogue — Stage 15;
- progressive examples, Kakeibo/Worldstack stress tests and benchmarks — later stages.

None of these prevent the Stage 1 boundary from being used as the input to Stage 2.

## 19. Exit evidence

Stage 1 exit requirement:

> a defensible legal-production boundary exists without a fixed skill count or template catalogue.

Evidence in this log:

- [x] project goal defined;
- [x] owned legal outcomes defined;
- [x] intended users defined;
- [x] core matter classes bounded;
- [x] initial jurisdiction strategy defined;
- [x] human approval points defined;
- [x] regulated/specialist handoffs defined;
- [x] explicit non-goals defined;
- [x] reusable-vs-project-specific knowledge boundary defined;
- [x] Pactwright and Production Skills interfaces defined;
- [x] multidimensional quality definition defined;
- [x] candidate core responsibilities accepted/rejected;
- [x] later-stage questions kept deferred rather than prematurely designed.

**Stage 1 status: COMPLETE.**

The next permitted bootstrap task is **Stage 2 — Select the Complementary Five-Book Legal Corpus**.