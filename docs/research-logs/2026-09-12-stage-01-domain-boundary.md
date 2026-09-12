# Stage 01: Project charter and legal-production boundary

**Status:** Complete for Stage 1; research and design decisions, not implemented capability  
**Version:** 1.0  
**Date:** 12 September 2026  
**Bootstrap:** [Legal Skills bootstrap v1.2, Stage 1](2026-09-08-legal-skills-new-project-bootstrap-process.md#7-stage-1--define-project-goal-users-and-professional-boundary)  
**Execution branch:** `feat/bootstrap-2`

## 1. Execution scope and evidence basis

This log completes the definition of the project goal, users, owned outcomes, professional boundary, initial jurisdiction strategy, quality criteria and human review responsibilities. It is the seed for Stage 2. It does not select books, claim direct book examination, complete the professional-practice challenge, design a fixed skill set or publish an Extension Pack catalogue.

The repository baseline is [`b15f313`](https://github.com/sb-dev/legal-skills/commit/b15f3134552ea763d434783d655aea44c0e01925). Its tree contains the provisional root README, research-log README and bootstrap specification. There are no prior stage execution logs or repository `AGENTS.md` instructions on this baseline. The separate `feat/bootstrap` branch is not an input to this execution; no completion claim or corpus decision is imported from it.

The governing Production Skills revision is [`20979e0`](https://github.com/sb-dev/production-skills/commit/20979e0c68ac4b37433374df7fe10ceb2e7ee69a). The following contracts govern the decisions here:

| Governing source | Requirement applied to Stage 1 |
|---|---|
| [Bootstrap generation guide](https://github.com/sb-dev/production-skills/blob/20979e0c68ac4b37433374df7fe10ceb2e7ee69a/docs/bootstrap/README.md) | Define the discipline, users, outcomes, quality, commitment points and adjacent responsibilities before architecture. |
| [New-project process](https://github.com/sb-dev/production-skills/blob/20979e0c68ac4b37433374df7fe10ceb2e7ee69a/docs/bootstrap/new-project-process.md) | Complete and commit each standalone stage; retain the minimal bootstrap workspace. |
| [Domain research process](https://github.com/sb-dev/production-skills/blob/20979e0c68ac4b37433374df7fe10ceb2e7ee69a/docs/bootstrap/domain-research-process.md) | Stage 1 supplies the seed; selection, direct extraction and broader challenge have separate gates. |
| [Family system](https://github.com/sb-dev/production-skills/blob/20979e0c68ac4b37433374df7fe10ceb2e7ee69a/docs/specs/01-production-skills-family-system.md) | Domain expertise stays reusable and standalone; consuming-project knowledge and Pactwright governance remain outside it. |
| [Project contract](https://github.com/sb-dev/production-skills/blob/20979e0c68ac4b37433374df7fe10ceb2e7ee69a/docs/specs/02-production-skills-project-contract.md) | Persist substantive research; do not infer implemented or scaffolded maturity from documents. |
| [Evaluation and Extension Packs](https://github.com/sb-dev/production-skills/blob/20979e0c68ac4b37433374df7fe10ceb2e7ee69a/docs/specs/03-production-skills-evaluation-and-extension-packs.md) | Keep quality dimensions separate; the core remains useful without a pack. |
| [Extension Pack process](https://github.com/sb-dev/production-skills/blob/20979e0c68ac4b37433374df7fe10ceb2e7ee69a/docs/bootstrap/extension-pack-process.md) | Specialisation needs its own evidence and behavioural difference; this boundary does not select packs. |
| [Cross-domain integration](https://github.com/sb-dev/production-skills/blob/20979e0c68ac4b37433374df7fe10ceb2e7ee69a/docs/specs/04-cross-domain-orchestration-and-integration.md) | Define handoff information and change authority without centralising project state. |
| [Shared-abstraction process](https://github.com/sb-dev/production-skills/blob/20979e0c68ac4b37433374df7fe10ceb2e7ee69a/docs/bootstrap/shared-abstraction-process.md) | A proposed common concept needs evidence from at least two independent domain implementations before promotion. |

Official-source examination below is bounded reconnaissance for this charter. Source-backed observations, project policy decisions and future validation needs are distinguished. No claim is made that the complete legal discipline or a consuming project's legal position has been validated.

## 2. Project charter

`legal-skills` owns reusable, evidence-backed legal production for people building software, digital products and creative works. It turns a defined project question or change into a traceable account of applicable legal issues, supported analysis, practical options, requirements and, when needed, draft or reviewed legal documents.

The unit of work is a **bounded legal matter**: a question or decision with identifiable actors, facts, jurisdictions, dates, intended use and an accountable human owner. A matter can concern a single clause, a product release, a licence, a brand decision or a change affecting several artefacts. It is not synonymous with a court case.

The useful outcome is a project decision that people can inspect and act on: what must change, what can remain, what is uncertain, what evidence supports the position and which decision needs specialist judgement. A document is one possible output, not the definition of success.

The project supplies production expertise through independently installable Agent Skills. It remains useful in an ordinary consumer repository without Pactwright, a central matter database or a specialist pack. The eventual packaging follows research; this charter fixes neither skill count nor command names.

Accountability stays with people and organisations. Legal Skills does not act as a law firm, hold professional status, accept an engagement as counsel, make binding business decisions or confer authority to represent another person.

## 3. Owned outcomes and responsibility decisions

All nine responsibilities proposed by Stage 1 belong within the reusable boundary. Their scope differs from owning every substantive field of law. These are responsibility decisions to challenge through Stages 2–4, not nine proposed skills.

| Responsibility | Owned outcome and reason for inclusion | Limit and handoff |
|---|---|---|
| Legal scoping and issue spotting | A bounded question, material fact gaps, likely legal surfaces and required expertise. Prevents work on the wrong question before expensive research or drafting. | The matter owner confirms purpose and facts. Missing facts remain questions or explicit assumptions. |
| Authoritative legal research | A source-supported account of relevant propositions, limitations and temporal context. Authority selection and applicability are legal responsibilities. | Retrieval tools supply material; Legal Skills checks its legal relevance. It does not operate a universal legal database or treat search snippets as verified authority. |
| Analysis and option framing | Application of authority to facts, material counterarguments, uncertainties and feasible options. A bibliography alone cannot guide production. | Recommendations remain scoped decision support. Business trade-offs and specialist opinions retain human owners. |
| Drafting | Documents or clauses derived from known behaviour, intended audience and supported legal positions. Connects analysis to usable artefacts. | Drafting cannot invent retention periods, refund rights, permissions or commercial agreements to fill a template. External adoption requires the review route in section 8. |
| Review and redlining | Located defects, rationale and bounded amendments that preserve unaffected approved work. Supports existing projects as well as new ones. | A redline is not authority to accept terms, execute an agreement or reopen every agreed position. |
| Legal-product consistency | An inspectable comparison between legal requirements or statements and actual implementation, UX, commercial practice or asset use. | Engineering, design, operations and creative teams own implementation. Legal Skills assesses the legal meaning of their evidence. |
| Legal change impact | Affected facts, propositions, requirements, documents and decisions identified after a supplied product or legal change; targeted re-review. | The consuming project initiates monitoring and lifecycle work. No regulatory monitoring service or central project graph is created. |
| Risk and uncertainty communication | Clear separation of known requirements, contestable interpretation, missing evidence, exposure and actionable next steps. | No single risk score, unqualified compliance badge or reassurance unsupported by the evidence. |
| Specialist escalation packaging | A concise question with facts, sources, reasoning, unresolved issues, options and the decision required from a suitable professional. | Legal Skills prepares the handoff. The professional accepts the engagement and owns any professional opinion or regulated act. |

Each output must carry enough context to prevent reuse beyond its factual, jurisdictional or temporal basis. A previously accepted conclusion is a dependency to recheck when material inputs change, not a timeless rule to embed in the core.

## 4. Intended-user map

| User | Work they bring | Useful result | Responsibility they retain |
|---|---|---|---|
| Founder, product owner or open-source maintainer | A launch, commercial choice, dependency, brand or change needing legal treatment | Prioritised questions, supported options, draft materials and implementation requirements | Confirm facts and intent; choose permissible business options; obtain required review and authorise adoption |
| Engineer, architect, security or data practitioner | Data flows, dependencies, infrastructure, runtime behaviour and implementation evidence | Specific legal constraints and discrepancies tied to observable behaviour | Establish technical truth, implement changes and demonstrate the result |
| UX designer, researcher or content designer | Consent, disclosure, cancellation, onboarding and other user interactions | Legally relevant presentation and interaction requirements, with factual and audience assumptions | Design and test the experience; escalate changes that alter the legal basis |
| Creator, game developer or production lead | Assets, references, licences, provenance, distribution plans and representations of real people or organisations | Use restrictions, attribution needs, alternatives and specialist questions | Maintain provenance, secure permissions and implement approved production decisions |
| In-house lawyer, external counsel or supervised legal researcher | A scoped research, analysis, drafting or review assignment | Verifiable source work, assumptions, redlines and a reviewable reasoning trail | Apply professional judgement, determine competence and entitlement, supervise and take responsibility for legal services delivered |
| QA reviewer, delivery lead or Pactwright-selected agent | Acceptance criteria, change information and evidence from other disciplines | Legal verification findings with affected requirements and unresolved decisions | Own product QA or orchestration decisions within the consuming project's authority model |

Non-specialist users must be able to understand the question, proposed action and limits without reading a full legal memo. Expert reviewers must be able to inspect sources and reasoning without reconstructing the matter. These are two views of the same evidence, not two different standards of truth.

The initial audience is production teams working on their projects. A public service providing unsupervised individual advice on arbitrary legal problems is outside the charter. A professional using the skills does not transfer their responsibility to the agent; the SRA's AI warning expressly maintains accountability for regulated users. [SRA warning](https://www.sra.org.uk/solicitors/guidance/misuse-ai/).

## 5. Core matter classes and depth limits

Matter classes provide varied proving work for the same reusable discipline. They are not a template catalogue, pack list or promise that every question within a field can be resolved by the core.

| Matter class | Baseline responsibility | Specialist boundary |
|---|---|---|
| Product privacy and data use | Establish relevant processing facts; research a bounded question; connect disclosures and obligations to data flows, processors, retention and user controls | Complex international transfers, sensitive or high-impact processing, disputed applicability and regulator matters require appropriate specialist review |
| Consumer digital commerce | Relate terms, notices and bounded legal questions to subscriptions, payments, cancellation, refunds, claims and actual customer journeys | Material uncertainty about mandatory rights, novel commercial models and enforcement exposure require specialist judgement |
| Copyright, content and asset licensing | Trace origin, asserted ownership, permission or exception, licence version, intended use and distribution; identify missing evidence and practical alternatives | Contested ownership, exceptions, infringement, AI/IP novelty and significant clearance decisions require specialist review |
| Software and open-source licensing | Analyse bounded licence questions against actual dependencies, modifications and distribution; produce obligation and notice findings | Disputed compatibility, uncertain ownership, enforcement and significant disclosure or commercial implications require specialist review |
| Brand and trade mark screening | Scope territory, candidate mark, goods/services and search limitations; identify conflicts and next questions | Screening cannot grant clearance or guarantee registration. Conflicts and consequential adoption or filing strategy go to an appropriate IP professional |
| Routine product and production agreements | Research, draft or review bounded non-contentious service, supplier, confidentiality or content-permission terms against confirmed facts | Complex liability allocation, exclusivity, substantial rights transfers, deeds and unusual transactions need a separately scoped specialist route |
| AI features, games, media and user-generated content | Identify legal surfaces; apply the same research, analysis and consistency responsibilities to bounded issues; preserve provenance and operational facts | Specialist platform duties, children, financial services, real-person claims and unfamiliar jurisdictions are not resolved by generic core assumptions |

The overlap between the last row and privacy, consumer and IP work is deliberate. It describes a production setting; it does not create a parallel legal workflow. Whether a recurring specialisation warrants a pack is decided at Stage 15 using behavioural evidence.

Kakeibo and Worldstack justify breadth without enlarging core into an omnibus. A Kakeibo matter may expose a financial-regulatory question; core must recognise and frame it without claiming a definitive regulated-perimeter opinion. A Worldstack matter may expose defamation or publicity questions; core can assemble the representation, distribution facts and sources for specialist review. Neither project name supplies missing facts.

## 6. Professional-boundary map

### 6.1 Legal restrictions and project policy are different

For the England and Wales baseline, the Legal Services Act identifies six reserved categories: rights of audience, conduct of litigation, reserved instrument activities, probate activities, notarial activities and administration of oaths. The exact scope is defined in Schedule 2. Entitlement matters under section 14. [Section 12](https://www.legislation.gov.uk/ukpga/2007/29/section/12/data.html), [Schedule 2](https://www.legislation.gov.uk/ukpga/2007/29/schedule/2/data.html), [section 14](https://www.legislation.gov.uk/ukpga/2007/29/section/14/data.html).

The Legal Services Board also distinguishes unreserved advice and assistance and describes exemptions. It would therefore be inaccurate to say every legal analysis or draft requires a solicitor, or every filing is reserved. This charter deliberately sets a narrower operational remit than everything a particular user might lawfully do. Other activity-specific regimes still need checking when relevant. [LSB explanation](https://legalservicesboard.org.uk/enquiries/frequently-asked-questions/reserved-legal-activities).

| Boundary | Legal Skills may own | External authority or commitment |
|---|---|---|
| Legal information and preliminary analysis | Public-source research, issue identification and qualified application to a defined matter | A human owns the intended use and any reliance decision |
| Drafting and review | Research-backed drafts, issue lists, clause analysis and proposed redlines within scope | The appropriate reviewer approves the legal position; an authorised project representative adopts or signs |
| Specialist professional judgement | Prepare the record, alternatives and precise unresolved question; incorporate a received opinion with its scope and provenance | A competent professional makes the opinion; professional status is never inferred from a prompt or role name |
| Reserved activities, proceedings and representation | Identify the boundary, preserve supplied evidence and prepare an appropriate referral | No exercise of reserved powers, court conduct, advocacy or representation by the skills; the responsible person must establish the required entitlement |
| Registry or regulator action | Research public procedures and assemble a reviewable preparation package where within scope | No autonomous submission, filing fee, undertaking, notice or representation. This is project policy, not a claim that every such action legally requires a practitioner |
| Commercial commitment and risk acceptance | Explain requirements, options and residual uncertainty | The authorised owner selects a permissible course, accepts residual business risk, contracts, publishes or launches |
| Confidential or potentially privileged material | Identify sensitivity and the minimum information needed; use only a route eligible for that matter | The information owner and, where needed, counsel determine disclosure authority and appropriate handling |

Public trade mark guidance supports both scoping goods/services and checking similar marks, and advises professional help where conflicts are found. The project's screening-to-adoption distinction follows from that evidence; it does not turn a registry result into a legal clearance opinion. [UK IPO guidance](https://www.gov.uk/how-to-register-a-trade-mark/before-you-apply).

### 6.2 Useful escalation rather than blanket refusal

An out-of-scope issue changes the permitted outcome. The system can still identify the question, organise material already available, state what remains unknown and prepare a handoff without pretending to resolve the specialist matter. It must not cross a reserved or otherwise restricted boundary while doing so.

A user instruction, pack or previous approval cannot establish that a proposed act is lawful. If the requested conclusion conflicts with verified applicable authority, record the conflict and offer supported alternatives. If applicability itself is uncertain, preserve that uncertainty for review rather than declaring the user prohibited from acting on an unverified premise.

## 7. Initial proving-jurisdiction strategy

**Decision:** Start positive end-to-end proving work with explicitly scoped **England and Wales** matters. Include relevant UK-wide legislation, regulatory material and UK rights only after checking the provision's territorial and material applicability. Treat additional jurisdictions as separate research and review contexts, never as implied coverage.

This is a research sequencing choice. It matches the UK official-source seed in the bootstrap and gives a bounded professional-services baseline. It does not infer the domicile, incorporation, markets or users of Kakeibo, Worldstack or any other consuming project.

| Context | Initial treatment | Evidence needed before broader coverage can be claimed |
|---|---|---|
| England and Wales | Primary positive proving jurisdiction for the matter classes in section 5 | Matter facts, relevant current authorities, applicability reasoning and suitable review; later installed examples must demonstrate actual behaviour |
| Applicable UK-wide legal regimes and UK IP rights | Included when relevant to the specific E&W proving matter; record scope by provision or right | Check territorial extent, application, dates and regulator remit instead of assuming a uniform body of UK law |
| Scotland and Northern Ireland | Explicitly outside the initial positive jurisdiction claim | Separate professional-boundary and substantive-law research where the facts require it; do not reuse E&W conclusions silently |
| EU law and individual Member States | Cross-border issue detection and scoped referral initially | Identify the actual Member State and relevant EU/local layers, source access and reviewer competence; Stage 5 defines the detailed treatment |
| US federal law and individual states; other territories | Cross-border issue detection and scoped referral initially | Identify actual territories, applicable rules and qualified review; a label such as “US” or “worldwide” is insufficient |

A website being accessible elsewhere, a supplier's location, the place of establishment, the users targeted, a contract's chosen law and the territory of an IP right are questions to investigate. None is a universal shortcut for deciding applicable law. Stage 5 must develop that analysis without a universal conflict-of-laws engine.

For an unknown jurisdiction, factual intake, a question list and source planning can proceed. Material jurisdiction-dependent conclusions remain conditional or withheld until resolved. For mixed matters, assess each relevant issue in its own context and route unresolved conflicts to suitable counsel.

Jurisdiction, source currency and verification are core obligations. An ordinary matter must not need a “UK law pack” to obtain them. A future pack may add specialised production behaviour; it cannot manufacture territorial coverage or replace current authority.

| Alternative considered | Disposition and reason |
|---|---|
| Universal advice from the first release | Rejected: no demonstrated source, applicability, professional-boundary or review coverage supports it |
| An undifferentiated UK default | Rejected: obscures territorial and legal-system differences relevant to scoping |
| E&W positive proving, explicit additional-jurisdiction routing | Selected: concentrated verification with visible limits; expansion follows matter evidence |
| One installable pack per jurisdiction | Rejected: makes a mandatory property of every legal matter look like optional specialisation |

## 8. Human review, commitment and escalation

The following are **project review requirements**, not a claim that legislation mandates this exact process for every legal task. Review depth follows the proposed reliance, uncertainty, exposure and reversibility. Routine public research and reversible internal drafting can continue within an established scope without repeated approval requests.

| Decision point | Reviewer or owner | What must be resolved |
|---|---|---|
| Material intake uncertainty | Matter owner and the person responsible for the relevant facts | Confirm actors, behaviour, intended use, jurisdictions to investigate and dates; record assumptions that cannot yet be verified |
| Sensitive information entering a tool | Information owner; counsel or security/data specialist where required | Determine whether the route is suitable and disclosure is authorised; use minimisation, redaction, approved private/local execution or withhold the material |
| Adoption of a material legal position | A reviewer competent for that matter and jurisdiction | Check source support, application, material contrary evidence, uncertainty and required specialist involvement |
| Consequential specialist issue | Appropriate legal professional or specialist counsel | Resolve the precise question within their competence; establish any necessary professional authority separately |
| External reliance, publication, agreement or launch | Accountable project representative, with required legal review completed | Confirm final wording and implementation match the reviewed facts and position; make the actual business commitment |
| Material change after review | Owner of the changed fact or behaviour plus affected reviewers | Identify dependent conclusions and reopen only affected work; record why other accepted work remains valid |

A founder may hold several project roles, but a signature does not demonstrate specialist competence. An automated check or second model's agreement is supporting evidence, not a substitute for required human judgement. If no suitable reviewer is available, the outcome remains preliminary or awaiting specialist review; it cannot be labelled cleared.

Specialist handoff is required by this charter when a matter includes:

- a potentially reserved act, representation or uncertain entitlement;
- an active dispute, threatened proceedings, enforcement exposure or a consequential deadline;
- conflicting material authority or unresolved cross-border applicability that could change the decision;
- a material trade mark conflict, disputed ownership or a consequential IP-clearance question;
- financial-regulatory perimeter, tax, immigration, employment, criminal, family, patent-prosecution or complex corporate questions beyond the owned production remit;
- novel or high-impact AI, child-related, sensitive-data or real-person issues beyond the available evidence or reviewer competence;
- uncertain disclosure authority or privilege treatment for material the work would expose.

These are routing triggers, not substantive findings that a particular product is regulated or an act is unlawful. Record a supplied deadline and urgently direct a time-sensitive matter to its human owner; do not invent a deadline calculation or let the research process imply that time has stopped.

The escalation package should contain the exact decision requested, purpose and urgency; parties and relevant territories; confirmed facts, evidence and assumptions; authorities and pinpoints actually examined; competing interpretations; practical options and consequences; unresolved gaps; and the scope of advice or action needed. Send or expose it only through a route authorised for those recipients and that information.

The SRA identifies both inaccurate AI legal outputs and confidentiality risks, including in paid tools, and expects suitable safeguards for regulated work. The charter therefore treats tool eligibility as a prerequisite to disclosure. It makes no blanket claim that AI use creates, preserves or waives privilege; uncertain treatment goes to counsel. [SRA warning](https://www.sra.org.uk/solicitors/guidance/misuse-ai/).

## 9. Reusable expertise, project knowledge and adjacent interfaces

| Owner | Belongs there | Must not be silently transferred |
|---|---|---|
| Legal Skills | Reusable legal methods, verification requirements, reasoning discipline, review criteria, handoff semantics and generalised examples | Consumer identities, private documents, project-specific legal opinions, risk acceptance or operational state |
| Consuming project or its Project Intelligence equivalent | Matter instances, facts, approved decisions, counsel advice, legal artefacts, evidence and change history | Project conclusions cannot become universal Legal Skills rules merely because they worked once |
| Production Skills central repository | Family contracts, registry and validated cross-domain abstractions | Legal matter storage, legal-quality adjudication and a shared compliance runtime |
| Pactwright, when present | Delivery authority, Contracts, lifecycle, Evidence semantics and governance | Legal Skills cannot create its own competing lifecycle or claim authority to pass a Pactwright gate |
| Execution tools and source providers | Retrieval, registry queries, licence scans, document parsing and diffing | A successful tool call does not establish applicable law, licence compliance or professional authority |

The minimal handoff is a documented exchange of purpose, input evidence and revisions, relevant scope and dates, outputs with their basis and limitations, unresolved decisions, and the party authorised to change or accept the work. This is an information requirement, not a new schema, database or graph. Stage 6 defines artefacts; Stage 8 defines traceability.

| Adjacent discipline | Receives from it | Returns to it | Ownership that stays outside Legal Skills |
|---|---|---|---|
| Deep Research | Source discovery, background evidence, provenance and stated gaps | Legal questions, required authority types and legal applicability or verification findings | General research methods; Legal Skills retains legal authority and legal reasoning semantics |
| Software Engineering | Actual architecture, data flows, dependencies, behaviour, tests and changes | Supported requirements, implementation discrepancies and criteria for re-review | Architecture, coding, deployment and technical test execution |
| UI/UX Design | User journeys, notices, interaction behaviour and research evidence | Disclosure, consent or commercial-flow constraints and legal-content review findings | Interaction design, usability evaluation and user-research conclusions |
| Game Development and creative Production Skills | Asset provenance, rights evidence, representations, planned use and distribution | Use restrictions, unresolved rights questions, attribution and permissible-alternative analysis | Creative direction, asset generation and runtime integration |
| Business Building and Advertising Production | Commercial model, offers, claims, substantiation and go-to-market decisions | Consumer, contract, claims or regulatory issues and supported constraints | Pricing, strategy, campaign design and commercial risk decisions |
| Pactwright or another orchestrator | An authorised responsibility, project constraints and evidence references | Legal findings, requirements, review status, affected dependencies and verification inputs | Lifecycle transitions, task assignment, authority and integrated acceptance |

Standalone use requires the same information but can keep it in project-native documents and version control. Pactwright adds governance when selected; it is not required for legal reasoning or evidence traceability.

## 10. Quality definition and efficient production

Legal production is useful when a reviewer can trace a material statement from project facts through relevant authority and reasoning to the proposed action, and can see what would change that conclusion. Fluency and a complete-looking document cannot compensate for a missing part of that chain.

| Dimension | Evidence of adequate work | Failure that must remain visible |
|---|---|---|
| Scope and facts | Intended decision, actors, material facts, assumptions and exclusions are explicit | Invented product behaviour or an answer to a different question |
| Authority and traceability | Material propositions point to identifiable, examined sources and supporting locations | Fabricated citation, unsupported proposition or a source that says something different |
| Jurisdiction and time | Applicability and relevant dates are resolved or bounded; later treatment is checked where material | Wrong territory, future law treated as effective, stale guidance or an undated conclusion |
| Reasoning and uncertainty | Facts are applied to authority; exceptions and material competing readings are addressed | Correct quotation used to support an unjustified conclusion or concealed uncertainty |
| Drafting and communication | Audience can understand rights, obligations, choices and required action; internal and cross-document consistency is maintained | Ambiguous wording, unsupported promises, contradictions or polished but unfair consumer terms |
| Product consistency | Claims and requirements are compared with implementation, operations and actual asset use | A privacy notice contradicts retention, terms contradict cancellation or licence conditions are absent from distribution |
| Review and professional boundary | Review state, unresolved specialist questions and accountable decision makers are visible | A draft presented as approved, screening presented as clearance or a model presented as counsel |
| Confidentiality | Information use fits the eligible tool route and disclosure authority | Sensitive inputs placed in an unsuitable provider, public example, log or repository |
| Preservation and repair | A changed input leads to identified dependent updates and retained unaffected work | Wholesale rewriting or a stale downstream conclusion after a local correction |
| Proportionality | Depth and artefact cost fit the decision, uncertainty and consequence | Exhaustive research without decision value, or a cheap draft used to hide a material gap |

Examples of economical sequencing are a matter brief before a memo, an issue list before extended research, a clause inventory before a complete redraft, a redline before a replacement agreement, a bounded brand screen before specialist clearance work, and a data-flow inventory before a privacy notice. The adequate representation is the one that resolves the present question; low cost never excuses unsupported legal claims.

The ICO's disclosure guidance ties privacy information to processing facts and is visibly under review following legislative change. This supports both fact-led drafting and explicit currency checks, without treating that guidance as a complete current-law opinion. [ICO guidance](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/individual-rights/the-right-to-be-informed/what-privacy-information-should-we-provide/).

The CMA's consumer guide examines substantive fairness as well as transparency, in the context of what is sold and how terms operate. This supports a separate product-and-terms review rather than a prose-only check. [CMA guide](https://www.gov.uk/guidance/writing-a-fair-contract-for-customers).

These are quality requirements for later design. Stage 18 must turn them into independent failure cases and benchmark evidence. This stage makes no measured accuracy, efficiency or compliance claim.

## 11. Kakeibo and Worldstack boundary probes

The bootstrap names these consuming projects as later canonical stress tests. The probes below are hypothetical design checks using its stated surfaces, not research into either project's actual implementation, legal advice for them or executed benchmark results.

| Probe | Boundary decision and required outcome |
|---|---|
| Kakeibo privacy wording promises deletion after 30 days, while a hypothetical backup retains data longer | Establish the real retention facts and applicable requirements; identify affected wording, behaviour and review. Do not invent a technically convenient retention policy. |
| Kakeibo changes a hypothetical subscription refund flow after terms were reviewed | Trace the changed behaviour to affected terms, UX and conclusions. Commercial and implementation owners decide and deliver permissible changes. |
| Kei adds a hypothetical personalised investment recommendation | Recognise a possible financial-regulatory perimeter question, capture actual behaviour and claims, and prepare specialist review. A product label or disclaimer cannot settle it. |
| A Worldstack reference is publicly visible online | Ask about provenance, rights, proposed use and territory. Public visibility is not accepted as evidence of permission. |
| A Worldstack mark search finds a potentially similar mark | Preserve search scope and findings; route a consequential adoption or filing decision to appropriate IP review rather than declaring clearance. |
| Worldstack expands a hypothetical UK-only distribution brief worldwide | Reopen territorial scope and affected rights conclusions. Do not export the E&W analysis as worldwide coverage. |
| Either project asks the agent to file proceedings or claim professional approval | Apply the professional boundary and prepare a useful handoff; do not perform the act or invent approval. |
| Either project has a verified problem in one clause, source or dependency | Repair dependent work at the smallest sufficient scope and preserve unaffected approved material. |

A separate generic producer or small open-source project must also be able to use the same methods. If a proposed core rule only makes sense for Kakeibo or Worldstack, it belongs in that consuming project unless subsequent evidence establishes a reusable need.

## 12. Explicit non-goals

- Regulated professional status, a law-firm simulation, autonomous legal sign-off, court conduct, advocacy, representation or reserved activities.
- An all-purpose practice covering litigation, tax, criminal, family, immigration, employment, complex corporate transactions or patent prosecution. Core can recognise and route questions without taking ownership of these practices.
- Autonomous filings, regulator submissions, agreement execution, legal notices or other external commitments on behalf of a project.
- Universal substantive-law coverage, a jurisdiction ontology, conflict-of-laws engine, case-law database, registry mirror or custom citator.
- A compliance certification service, universal risk score or claim that a product is compliant without bounded facts, authority, jurisdiction and dates.
- A central legal matter store, regulatory-change SaaS service, universal legal workflow language or shared compliance graph.
- Ownership of product strategy, commercial decisions, UX, engineering, creative production or Pactwright lifecycle semantics.
- Static legal templates used as substitutes for facts and analysis; current legal conclusions frozen into durable core prompts or packs.
- Mandatory specialist packs for basic jurisdiction, authority verification, uncertainty handling or professional boundaries.
- Public storage of private matters, confidential advice, supplied books or proprietary source material. Public research logs and future benchmarks use public or synthetic material with appropriate publication rights.

## 13. Official-source register and limitations

All sources below were directly opened on **12 September 2026** for this boundary exercise. Publication or update dates are recorded only where displayed. Retrieval date does not establish commencement, continuing validity, completeness of research or applicability to a live matter. The legislation pages use the official HTML data view because the standard page's content type was not readable by the retrieval tool.

| ID | Source and material examined | Observation used | Limits |
|---|---|---|---|
| A1 | [Legal Services Act 2007, s12](https://www.legislation.gov.uk/ukpga/2007/29/section/12/data.html), including reserved and other legal activity definitions | Statutory basis for distinguishing reserved activity from legal advice and assistance more generally | A definition is not a determination of entitlement or an exhaustive review of other regulation |
| A2 | [Legal Services Act 2007, Schedule 2](https://www.legislation.gov.uk/ukpga/2007/29/schedule/2/data.html), paragraphs 3–8 | Reserved categories have specific scopes and exclusions | No activity-specific exemption opinion or later-case-law research was performed |
| A3 | [Legal Services Act 2007, s14](https://www.legislation.gov.uk/ukpga/2007/29/section/14/data.html), especially subsection (1) | Carrying on a reserved activity requires entitlement | This log does not determine whether any actual person is entitled |
| A4 | [LSB reserved-activities explanation](https://legalservicesboard.org.uk/enquiries/frequently-asked-questions/reserved-legal-activities), reserved activities, exemptions and other legal activity | Confirms the need to avoid treating all advice as reserved and to examine specific circumstances | Oversight-body explanation; no publication/update date displayed; not a substitute for the governing provisions |
| A5 | [SRA AI misuse warning](https://www.sra.org.uk/solicitors/guidance/misuse-ai/), published 17 August 2026; audience, hallucinations, accountability and confidentiality sections | Verification, human responsibility and information handling are material production concerns | Directed at regulated firms and individuals; the broader charter requirements are project policy. No independent analysis of the cited judgments or privilege doctrine was conducted |
| A6 | [ICO privacy-information guidance](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/individual-rights/the-right-to-be-informed/what-privacy-information-should-we-provide/), review notice and disclosure tables | Processing facts matter to disclosures; the page flags pending guidance changes following the Data (Use and Access) Act | No publication/update date displayed. Guidance under review is qualified seed evidence, not proof of every current disclosure requirement |
| A7 | [CMA fair-contract guide](https://www.gov.uk/guidance/writing-a-fair-contract-for-customers), scope, fairness and transparency sections; updated 22 July 2026 | Consumer document review must consider substance, context and presentation | Summary guidance, not a completed Consumer Rights Act analysis or finding about a real clause |
| A8 | [CMA37 publication page](https://www.gov.uk/government/publications/unfair-contract-terms-cma37), document listing and update history; updated 22 July 2026 | Confirms the bootstrap's reference to revised guidance and its current document entry point | The full guidance PDF and technical note were not examined in this stage |
| A9 | [UK IPO trade mark preparation guide](https://www.gov.uk/how-to-register-a-trade-mark/before-you-apply), classes, similar-mark checks and professional-help sections | Screening needs goods/services context; identified conflicts warrant professional advice | No publication/update date displayed; no registry search or actual mark-clearance analysis was performed |

The bootstrap's copyright-and-AI policy-report reference remains inherited seed material; it was not independently examined for this stage and supports no current copyright conclusion here. Broader legal methods, professional practice, confidentiality doctrine and specialist matters require the subsequent research stages. No professional user interviews, book extraction, tool evaluation or installed skill executions were performed.

## 14. Decisions and handoff to later stages

| Decision | Result | Reopening condition |
|---|---|---|
| D1: Owned discipline | Evidence-backed legal production tied to project decisions and behaviour | Later evidence shows a material responsibility is missing or belongs elsewhere |
| D2: Reusable responsibility scope | Include all nine Stage 1 responsibilities; keep substantive depth bounded | Stages 2–4 reveal unsupported methods, better boundaries or distinct specialist needs |
| D3: Initial proving jurisdictions | E&W positive proving; scoped UK-wide sources; explicit additional-jurisdiction routing | A defined matter justifies additional source, review and evaluation coverage |
| D4: Professional boundary | Human accountability, explicit reserved-activity exclusions and useful specialist handoffs | Verified legal change or properly researched expansion; user intent alone is not professional entitlement |
| D5: Human commitments | Proportionate review before material reliance; separate legal review from business adoption | Stage 9 provides evidence for more precise thresholds without removing required authority |
| D6: Knowledge and integration | Reusable methods here; matter state in the consumer; governance in Pactwright when selected | Independent cross-domain implementation evidence justifies a smaller shared contract |
| D7: Architecture restraint | No fixed skills, commands, templates, packs, providers or production directories | The designated later design stage supplies evidence and contracts |

Stage 2 must consume the charter, responsibility map, matter-depth limits, jurisdiction strategy, quality criteria and handoff needs. It should derive a coverage map broad enough to assess legal scoping, research, reasoning, drafting/review, professional judgement, product-counsel work and change impact, without forcing one book per topic or selecting books solely for substantive UK doctrine.

No book titles or files were supplied with this Stage 1 request, and no corpus is selected here. Stage 2 must inspect any materials supplied for that task, compare a broader candidate pool and select exactly five complementary books. Empty-slot selection follows the governing process; removal, replacement or demotion of supplied books requires explicit permission. Source availability and actual reading coverage must remain separate.

| Later stage | Work deliberately left to its completion gate |
|---|---|
| 2 | Knowledge-coverage map, candidate comparison, five-book selection, access register and any substitution decisions |
| 3 | Direct examination, traceable extraction and reconciliation of all five selected books |
| 4 | Professional-practice challenge, contrary evidence, uncovered responsibilities and an evidence-qualified domain model |
| 5–6 | Detailed jurisdiction, authority and temporal-validity model; matter and reasoning artefacts |
| 7–10 | Workflow design, legal-product traceability, operational review/escalation criteria and confidentiality/privilege research |
| 11–15 | Tool research, execution choice, gap analysis, skill/command design and evidence-led pack decisions |
| 16–18 | Selected progressive examples, complete Kakeibo/Worldstack stress tests and executable evaluation design |
| 19 onward | Canonical specs, public product surface, implementation scaffold, installation, validation and any supported maturity promotion |

These are scheduled design decisions, not unresolved prerequisites to this charter. Stage 1 has no outstanding source-access or user-permission blocker. Its recommendations remain revisable through recorded evidence rather than silently changing the boundary.

## 15. Stage 1 completion review

| Required Stage 1 output | Completion evidence |
|---|---|
| Project charter and owned legal outcomes | Sections 2–3 define the unit of work, useful outcomes and all nine responsibility dispositions |
| Intended-user map | Section 4 identifies users, inputs, useful results and retained accountability |
| Core matter classes | Section 5 distinguishes baseline production work from specialist depth |
| Professional-boundary map and practitioner handoffs | Section 6 separates statutory boundaries, project policy and external authority using directly examined sources |
| Initial jurisdiction strategy | Section 7 selects a proving baseline, limits broader claims and records rejected alternatives |
| Quality definition | Section 10 defines independent quality dimensions, failure conditions and proportionality |
| Human review and escalation points | Section 8 names decision owners, triggers, blocked outcomes and useful handoff content |
| Reusable/project-specific boundary and adjacent interfaces | Section 9 assigns knowledge, governance, execution and handoff responsibilities |
| Explicit non-goals | Section 12 excludes omnibus practice, autonomous commitments and premature infrastructure |
| Defensible boundary without fixed skills or templates | Sections 3, 5, 7 and 11 examine scope and counterexamples; sections 13–14 expose evidence limits and later research needs |

The review finds the Stage 1 exit criterion met: a defensible legal-production boundary exists. The hypothetical probes are design checks, not benchmark passes. Completion of this log does not establish legal accuracy in live use, complete any later stage, promote the family registry or make the repository a production scaffold.

---

**Version 1.0 — 12 September 2026.** Stage 1 charter and boundary completed against legal bootstrap v1.2. Next gate: Stage 2, complementary five-book corpus selection.
