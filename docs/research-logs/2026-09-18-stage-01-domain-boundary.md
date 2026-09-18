# Stage 1 — Project Goal, Users and Professional Boundary

**Bootstrap stage:** 1 (`docs/research-logs/2026-09-08-legal-skills-new-project-bootstrap-process.md`, §7)
**Status:** Complete
**Date:** 18 September 2026
**Working branch:** `claude/bootstrap-vteuud`
**Depends on:** Stage 0 workspace; the governing bootstrap specification (including its §3 seed evidence)

This log is the durable Stage 1 output. Stages 2–27 must read it rather than
reconstructing the boundary from conversation history.

---

## 0. Evidence basis and its limits

### 0.1 What was actually done

| Activity | Performed | Notes |
| --- | --- | --- |
| Read the complete governing bootstrap specification | Yes | All 34 sections |
| Read the execution contract and support skills | Yes | |
| Inventoried supplied sources under `books/` | Yes | See §0.3 and Stage 2 |
| Targeted reconnaissance searches | Yes | 4 searches, §0.2 |
| Direct inspection of authoritative source pages | **No — blocked** | See §0.4 |

### 0.2 Reconnaissance research register

Stage 1 is a boundary-definition stage. The governing specification directs
"only enough additional reconnaissance" here; the heavy evidence load sits at
Stages 3, 4, 5 and 11. Four questions were researched.

| # | Research question | Method | Outcome |
| --- | --- | --- | --- |
| R1 | Which legal activities are legally restricted to authorised persons in England and Wales, and is giving legal advice itself restricted? | `WebSearch` | Six reserved legal activities under Legal Services Act 2007 s.12 / Sch.2: rights of audience; conduct of litigation; reserved instrument activities; probate activities; notarial activities; administration of oaths. Carrying on a reserved activity without entitlement is a criminal offence. Legal advice that is **not** a reserved activity is unreserved and may lawfully be given without authorisation. |
| R2 | What does the SRA currently require of solicitors using AI? | `WebSearch` | Warning notice "Misuse of AI", published 17 August 2026. Solicitors remain accountable for work and outputs regardless of how prepared; reliance on an AI output is not a defence for false citations before a court; content of legal submissions must be verified; client confidentiality is a distinct named risk. Reported context: 42 AI-misuse reports to the SRA between July 2025 and July 2026, with open investigations on citations, supervision and confidentiality. |
| R3 | How is the same boundary drawn in the United States? | `WebSearch` | A different model: unauthorized practice of law (UPL) is defined per-jurisdiction (ABA Model Rule 5.5 prohibits it; each state defines "practice of law"). The operative distinction is **legal information vs legal advice**: general explanation of how a rule works is information; applying rules to a specific person's facts and telling them what to do is advice and may constitute practice of law. |
| R4 | What legal work does product / commercial in-house counsel actually own in a software or product organisation? | `WebSearch` | A blended, non-litigation portfolio: commercial contracts, regulatory compliance, privacy, intellectual property, marketing claims and consumer protection; embedded early in product development to identify issues during design rather than after launch; coordinates launch risk across product, engineering, policy and marketing. |

Supplementary reconnaissance (legal operations competency models, e.g. the
CLOC "Core 12") was searched and returned strategic-planning, financial,
vendor, knowledge-management and information-governance competencies. These
are **legal department operations**, not legal production, and are recorded
here only to justify their exclusion from core (see §6.2).

### 0.3 Supplied-source note

Five PDFs were supplied and are present under `books/` (gitignored). They are
*not* the books themselves; each is a secondary overview of a book. This is
material to Stages 2 and 3 and is analysed there, not here. Stage 1 draws no
substantive finding from them.

### 0.4 Capability limitation — outbound fetch blocked (carry forward)

**This session has no outbound HTTP egress.** Every external host probed
returned `403` at the egress proxy (`CONNECT tunnel failed`), including
`legislation.gov.uk`, `sra.org.uk`, `ico.org.uk`, `gov.uk`,
`legalservicesboard.org.uk`, `judiciary.uk`,
`caselaw.nationalarchives.gov.uk`, `eur-lex.europa.eu`, `iclr.co.uk`,
`lawsociety.org.uk`, `americanbar.org` and `en.wikipedia.org`. This is an
organisation egress policy, not a transient failure, and must not be routed
around.

Consequences, stated honestly:

- `WebSearch` works; `WebFetch` and `curl` do not. Firecrawl is equally
  unavailable, since it is also outbound HTTP.
- Every R1–R4 finding above is **search-derived**: it rests on search-result
  synthesis, not on inspection of the source page. Under
  `bootstrap-research`, search output is a discovery aid, not evidence.
- Accordingly, no R1–R4 finding is promoted here to a verified authority.
  They are used only for **structural orientation** — to decide what this
  project will and will not attempt. Structural propositions of this kind
  (that reserved activities exist and are enumerated; that unreserved advice
  is lawful; that US UPL is state-defined; that a warning notice exists) are
  stable enough to found a scope decision, and every one of them is
  conservative in the direction that matters: each narrows the boundary.
- **No substantive legal proposition in this log may be relied on by a live
  matter.** Stages 5 and 11 must re-resolve them against inspected
  authoritative sources.

Carried forward as a bounded gap:

```text
GAP-01  Authoritative-source inspection is unavailable in this environment.
        Stages 4, 5 and 11 require inspected primary/official sources.
        Resolve by restoring egress, by supplying offline copies of the
        required sources, or by an explicit user decision to accept
        search-derived evidence for those stages.
```

One incidental currency correction, recorded because the specification's seed
evidence will be cited by later stages: the SRA AI warning notice is indexed
at `https://www.sra.org.uk/solicitors/guidance/misuse-ai/`. The governing
specification §3 cites the `media.sra.org.uk` variant. Both appear in current
search results; neither could be inspected. Stage 5 should confirm the
canonical citation form.

---

## 1. Project charter

### 1.1 Mission

> Turn project reality into traceable legal requirements, advice and documents
> — and keep them true as the project changes.

`legal-skills` is a Production Skills project that gives AI agents a legal
**production discipline**. Its unit of value is not a document; it is a chain
that can be audited end to end:

```text
material fact
→ legal issue
→ proposition
→ authority (verified, jurisdiction-scoped, valid as of a date)
→ applicability analysis
→ conclusion / risk
→ project requirement or constraint
→ implementation or legal artefact
→ acceptance evidence
```

The project succeeds when that chain is inspectable and repairable, and when
its conclusions never become more certain than the facts, authority,
jurisdiction and dates that support them.

### 1.2 Owned legal outcomes

`legal-skills` owns these outcomes, and is accountable for their quality:

| # | Owned outcome | What "good" looks like |
| --- | --- | --- |
| O1 | A scoped matter | Purpose, actors, jurisdictions, dates, materiality and the decision actually being supported are explicit |
| O2 | A separated fact model | Established facts, assumptions, unknowns and open questions are distinguishable and individually attributable |
| O3 | Resolved or explicitly unresolved jurisdiction | Territory, governing law, forum and the reason each matters — or a recorded statement that it is unresolved and why that blocks conclusions |
| O4 | Issue spotting | The legal issues a set of project facts actually raises, including issues the requester did not ask about |
| O5 | A research plan and authority set | What must be established, in what order, from which source classes; authorities recorded with type, issuer, dates, retrieved-at and the proposition each supports |
| O6 | Applicability analysis | Whether an authority reaches these facts, in this territory, on this date — including where it does not |
| O7 | Options and recommendations | Framed as project actions with their legal consequences, not as abstract statements of law |
| O8 | Legal requirements and constraints | Law and contract translated into statements a product or engineering team can implement and verify |
| O9 | Drafted legal artefacts | Derived from actual product, data and commercial behaviour rather than from a template's assumptions |
| O10 | Review and redline | Omissions, conflicts, ambiguity, unsupported legal assertions and product contradictions, repaired by the smallest sufficient change |
| O11 | Legal–product consistency | Detection that a legal document and the product it describes have diverged |
| O12 | Change impact | Which legal conclusions, requirements and documents a project change invalidates, and the bounded re-review that follows |
| O13 | Inspectable risk and uncertainty | Multi-dimensional, in controlled language, never collapsed to one score |
| O14 | Confidentiality-aware routing | A decision about where a matter may be executed before it is executed |
| O15 | An escalation package | A specialist can act on it without reconstructing the matter |
| O16 | Legal-production evaluation | Each of the above can fail independently and be diagnosed |

### 1.3 Explicitly not owned

| Not owned | Owner |
| --- | --- |
| Whether the product should do the thing at all | The consuming project |
| Commercial terms, pricing, risk appetite | The consuming project |
| Regulated professional representation, advocacy, filing as agent | An authorised practitioner |
| The authoritative statement of what the law is | Legislatures, courts, regulators, registries |
| Project lifecycle, Contracts, Evidence semantics | Pactwright |
| Long-lived storage of a project's legal matters | The consuming project |
| General non-legal evidence gathering and synthesis | Deep Research skills |

---

## 2. Intended users

Five user classes, in descending order of design weight.

| # | User | Context | What they need from `legal-skills` | Primary risk if it fails |
| --- | --- | --- | --- | --- |
| U1 | **An AI production agent inside a project repository** | Has the code, data flows, dependency manifests, UX and commercial model in context; no counsel present | Discipline: refuse to conclude past the facts; resolve jurisdiction; verify authority; produce requirements that trace back | Confidently wrong legal output entering a product |
| U2 | **A founder, engineer or product owner without counsel** | Building something real; needs to know what is required and what is genuinely uncertain | Issue spotting they would not have thought to ask for; honest uncertainty; a clear "get a lawyer for this" signal | Believing an AI answer is legal clearance |
| U3 | **In-house, product or commercial counsel** | Professionally accountable for the output (see R2) | Verifiable working: authority tables, fact/assumption separation, redlines, reviewable drafts | Being handed unverifiable work that they must redo to be accountable for |
| U4 | **External or specialist counsel receiving an escalation** | Did not see the project; time-boxed | A package: question, facts, assumptions, jurisdiction, authorities, analysis, conflicts, options, precise decision required | Escalation that is a vague question with no facts attached |
| U5 | **Another Production Skills project** | Game Development, UI/UX, Software Engineering, Pactwright | Legal constraints as structured requirements and verification inputs with provenance and valid-as-of metadata | Legal constraints arriving as unusable prose |

**Design consequence.** U1 and U2 mean the system is frequently operating
where no lawyer will review the output. That is the reason the professional
boundary (§4) and the uncertainty model (§7) are load-bearing rather than
decorative, and the reason U3's verifiability requirement is designed in from
the start: an artefact a professional can check is also an artefact a
non-professional can be warned about.

---

## 3. Core matter classes

Selected by the test: *does this class recur across software, product and
creative projects, does it materially exercise the production loop, and can it
be worked without reserved activity?*

### 3.1 In core

| # | Matter class | Why in core | Exercises |
| --- | --- | --- | --- |
| M1 | Privacy and data protection for a product | Every product with users has it; the document must match actual data flows | Facts↔implementation consistency, retention, transfers, temporal currency |
| M2 | Consumer terms and commercial flows | Terms must derive from the real commercial model; fairness and transparency are substantive, not cosmetic | Drafting from behaviour, cross-document consistency, fairness review |
| M3 | Open-source and third-party licence compliance | Machine-checkable facts (manifests) against legal obligations; distribution-model dependent | Provenance, licence-version precision, obligation-to-use mapping |
| M4 | Trade mark and brand screening | Bounded, evidence-driven, with a hard and well-understood escalation line at filing and clearance | Territory, goods/services, classification, similarity, search≠clearance |
| M5 | Copyright, content and asset licensing, provenance | Central to creative production; "publicly available" is routinely mistaken for permission | Rights chains, exceptions, provenance across handoffs |
| M6 | AI and automated-system disclosure and issue spotting | The project itself ships AI; disclosures must match actual behaviour | Disclosure↔behaviour consistency, fast-moving law, temporal discipline |
| M7 | Commercial contract drafting and review | The general transactional engine underneath most of the above | Concept selection, clause planning, redlining, obligation mapping |

### 3.2 Issue-spotting only (perimeter classes)

Worked far enough to *recognise and escalate*, never to conclude:

- financial-services and payments regulatory perimeter;
- age assurance and child protection;
- marketing, advertising and comparative claims;
- UGC, moderation and platform-liability exposure;
- defamation and false implication;
- likeness, publicity and personality rights;
- export control and sanctions.

**Rule:** a perimeter class may produce an issue, a risk statement and an
escalation package. It may not produce an advice conclusion or a signed-off
requirement.

### 3.3 Out of scope

Litigation and dispute conduct; tax; employment; immigration; criminal;
family; corporate transactions and M&A; patent prosecution; securities
offerings; real property conveyancing; regulatory licence applications;
insolvency.

Rationale: none is a recurring production surface for the target projects,
several sit on or across a reserved activity, and each would demand its own
authority ecology and specialist evaluation. Some may later justify an
Extension Pack; none justifies core weight now. Per the bootstrap, **no
subject is in core merely because it is legal.**

---

## 4. Professional-boundary map

This is the central Stage 1 output.

### 4.1 The structural position

Two different regulatory models must both be respected, because the project
targets multi-jurisdiction production:

| | England and Wales | United States |
| --- | --- | --- |
| Restriction model | Enumerated **reserved legal activities** (LSA 2007 s.12 / Sch.2) | Per-jurisdiction definition of the **practice of law**; UPL prohibited (ABA MR 5.5) |
| Is advice itself restricted? | No — unreserved legal advice may lawfully be given without authorisation | Applying law to a specific person's facts and recommending action can itself constitute practice |
| Practical consequence | Scope is bounded by a **list of activities** | Scope is bounded by a **manner of engagement** |

*(Search-derived — see §0.4. Both are used only to set scope, and the design
below satisfies the stricter of the two.)*

**Design decision.** `legal-skills` adopts the **stricter** reading globally.
It does not rely on the England and Wales position that unreserved advice is
lawful, because the same skill will execute against US and other matters, and
because U2 users cannot assess which model applies to them. The project is
therefore designed so that it is safe under a UPL-style analysis:

```text
legal-skills produces reviewable legal work product,
attributed to a named requester and a named reviewer,
with its facts, authorities, dates and uncertainty exposed —
not a professional opinion, and not a representation.
```

### 4.2 The four hard lines

These are absolute. No Extension Pack, project instruction, user insistence
or prompt may cross them.

| # | Hard line | Restatement |
| --- | --- | --- |
| B1 | **No reserved activity.** | No right of audience, no conduct of litigation, no reserved instrument activity, no probate activity, no notarial act, no administration of oaths — and no preparation of a document whose execution is one of these. |
| B2 | **No claim of regulated status.** | Never state or imply that output is from a solicitor, barrister, attorney, trade mark attorney, patent attorney or other regulated professional; never imply a retainer, a professional duty of care or privilege that does not exist. |
| B3 | **No clearance, certification or sign-off.** | Never assert that a product, document or act *is* compliant, *is* lawful, *is* clear to use, or *is* free of infringement risk. Legal-skills produces analysis with stated scope, facts, authority and validity date. A registry search is not clearance. |
| B4 | **No representation or filing as agent.** | Never file, register, submit, serve, correspond as the party's legal representative, or act on a deadline as though authorised to do so. |

### 4.3 The graduated boundary

Between the hard lines and ordinary work, output is tiered. The tier is a
property of the artefact and must be stated on it.

| Tier | Name | May contain | Review requirement |
| --- | --- | --- | --- |
| T0 | **Legal information** | What a rule says; what a source is; how a process works — untailored | None |
| T1 | **Scoped analysis** | Application of verified authority to stated facts, with explicit assumptions, jurisdiction, valid-as-of date and uncertainty | Self-contained; reviewable; no sign-off claimed |
| T2 | **Reviewable work product** | Drafts, redlines, requirement sets, screening results — production artefacts intended to be checked before use | Named human reviewer required before external use |
| T3 | **Specialist referral** | Issue statement, facts, authorities, analysis, conflicts, options, precise decision required | Regulated practitioner required; `legal-skills` states no conclusion |
| T4 | **Refused** | Nothing — the request is outside the boundary | Request declined with the reason and the correct route |

Escalation is **one-way**: work may be raised to a higher tier at any point,
never lowered. A T3 finding inside a T2 artefact raises the whole artefact.

### 4.4 Handoff triggers to a regulated practitioner

Mandatory T3 on any of:

1. reserved activity required, or a document intended for a reserved use;
2. representation, filing, service, or a legal deadline to be met as agent;
3. live or reasonably anticipated dispute, enforcement action or regulatory
   investigation;
4. identified conflict between high-level authorities material to the answer;
5. cross-border applicability that the analysis cannot resolve;
6. trade mark: any similar-mark conflict, or any move from screening toward
   clearance or filing strategy;
7. financial-services, payments, credit or e-money perimeter questions;
8. novel or unsettled AI, IP or data questions where authority is absent or
   in flux;
9. material irreversible exposure: criminal liability, personal-liability
   exposure for officers, safety, or harm to children or vulnerable users;
10. the matter requires legal privilege to be established or preserved;
11. the facts required to reach a conclusion cannot be obtained.

### 4.5 Accountability posture

Adopted directly from the SRA position (R2) and generalised beyond
solicitors, because it is the correct design posture regardless of regulator:

```text
the person who uses the output is accountable for it
→ so the output must be verifiable
→ so every authority carries its identity, type, jurisdiction and dates
→ so every conclusion carries its facts, assumptions and validity window
→ so "the AI produced it" is never available as a defence, and the artefact
  is built to make checking cheaper than redoing
```

An unverifiable legal artefact is a **defect**, not a limitation.

---

## 5. Jurisdiction strategy

### 5.1 Jurisdiction is matter context, never product configuration

Fixed for the whole project, per the bootstrap's §21.2:

```text
every run resolves jurisdiction from the matter
NOT
legal-skills + a jurisdiction pack
```

There is no default jurisdiction, no inferred jurisdiction from the user's
locale, and no silent fallback. An unresolved jurisdiction is a **stated
result** that blocks conclusions — never an assumption.

### 5.2 Initial proving jurisdictions

Chosen to prove the *method*, not to claim coverage.

| Tier | Jurisdiction | Role | Why |
| --- | --- | --- | --- |
| J1 | **England and Wales** (with UK-wide instruments where they apply) | Primary proving jurisdiction | The seed evidence base is UK: SRA, ICO, CMA, UK IPO. Official sources are free and citable. The reserved-activity model gives a crisp, enumerated boundary to build against. |
| J2 | **European Union** | Second proving jurisdiction | Products built by the target users are routinely offered into the EU. Forces the separation of *establishment*, *market offered into* and *data-subject location* — the core discipline — and exercises a genuinely different instrument hierarchy. |
| J3 | **United States (federal and a state)** | Stress jurisdiction, issue-spotting and escalation only | Forces the state-level UPL model (R3) and state-by-state divergence into the design, so the system cannot assume one national answer. **No US conclusions are produced in core.** |
| J4 | **Everywhere else** | Recognition only | The system must recognise that a matter reaches a jurisdiction it cannot analyse, say so, and escalate. Silent extrapolation from J1 is a specific, tested failure. |

**Guardrail.** Two proving jurisdictions plus a stress jurisdiction is a
deliberate limit. The bootstrap forbids a universal jurisdiction engine and a
jurisdiction ontology. Adding J4 jurisdictions requires evidence of recurring
need, not symmetry.

### 5.3 Non-negotiable distinctions

These must never be collapsed, and Stage 5 must make each independently
representable:

```text
matter territory ≠ governing law ≠ forum ≠ regulator
place of establishment ≠ market offered into ≠ user location ≠ data location
publication date ≠ effective/commencement date ≠ retrieved-at ≠ valid-as-of
legislation ≠ regulator guidance ≠ commentary
registry search ≠ clearance
a current source ≠ current law
```

---

## 6. Core responsibility assessment

The bootstrap (§7) requires each candidate responsibility to be assessed
rather than assumed.

### 6.1 Candidates — decisions

| Candidate | Decision | Reasoning |
| --- | --- | --- |
| Legal scoping / issue spotting | **Core** | The highest-leverage capability and the one an untrained requester most needs. Everything downstream is scoped by it. Cheap to run, and its absence is the failure mode where a correct answer is given to the wrong question. |
| Authoritative legal research | **Core as discipline; orchestrated as execution** | `legal-skills` owns the source hierarchy, the research plan, the currency requirements and the verification contract. It does **not** own retrieval infrastructure — no database, no mirror, no citator (bootstrap §19). Retrieval is delegated to tools chosen at Stage 11. |
| Analysis / option framing | **Core** | The bridge from authority to project action. Without it the project is a citation formatter. |
| Drafting | **Core, with a constraint** | In core only in its project-derived form: drafting *from* an established fact model and requirement set. Template emission without a fact model is an explicit non-goal (§8). |
| Review / redlining | **Core** | Cheaper and more often correct than redrafting, and it is the form in which U3 actually works. Directly supports the preserve-verified-work principle. |
| Legal–product consistency | **Core, and distinctive** | This is the capability that most distinguishes `legal-skills` from a legal chatbot: it exists inside the repository, with access to data flows, manifests, UX and commercial logic. No general legal tool can do it. Strong claim to core. |
| Legal change impact | **Core** | The corollary of consistency. Without it, correct legal work silently rots as the product changes. |
| Risk / uncertainty communication | **Core** | Load-bearing for U1 and U2, who have no reviewer. A system that cannot express calibrated doubt is unsafe for them. |
| Specialist escalation packaging | **Core** | Escalation is a production capability (bootstrap §4), and a bad escalation wastes the specialist's time, which is the expensive resource. |

All nine are retained, but note what that does *not* mean: it fixes no skill
count and no command list. Stage 14 decides packaging; Stage 13 must still
justify each against a demonstrated gap.

### 6.2 Assessed and excluded

| Candidate | Decision | Reasoning |
| --- | --- | --- |
| Legal department operations (spend, vendor, matter portfolio, KM) | **Excluded** | The CLOC-style competency set is about running a legal *department*. `legal-skills` serves projects, most of which have no legal department. Out of boundary. |
| Persistent cross-project matter database | **Excluded** | Explicit bootstrap non-goal; matters live in the consuming project. |
| Regulatory change monitoring as a service | **Excluded** | Change *impact* on a known matter is core (above); continuous horizon scanning is a SaaS product and an explicit non-goal. |
| Compliance certification | **Excluded — hard line B3** | |
| Contract lifecycle management | **Excluded** | Signature, execution, storage and renewal are operational systems, not legal production. |

---

## 7. Quality definition

### 7.1 Quality dimensions

Legal quality is **not** one score (bootstrap §4). These dimensions must
remain independently visible and independently failable at Stage 18.

| # | Dimension | Fails when |
| --- | --- | --- |
| Q1 | Factual completeness | A conclusion rests on facts that were never established |
| Q2 | Fact/assumption separation | An assumption is presented as an established fact |
| Q3 | Jurisdiction correctness | The wrong territory's rule is applied, or jurisdiction is silently assumed |
| Q4 | Issue coverage | A material issue the facts raise is absent |
| Q5 | Authority existence | A cited authority does not exist |
| Q6 | Authority support | A real authority is cited for a proposition it does not support |
| Q7 | Authority strength and hierarchy | Guidance is treated as legislation; persuasive treated as binding |
| Q8 | Temporal validity | Repealed, amended, not-yet-commenced or superseded law is applied; no valid-as-of date |
| Q9 | Applicability reasoning | The rule is stated correctly but does not reach these facts |
| Q10 | Uncertainty calibration | Confidence exceeds what the facts and authority support |
| Q11 | Scope discipline | The answer silently exceeds the matter scope |
| Q12 | Drafting quality | Unclear, internally inconsistent, or wrong contract concept for the deal term |
| Q13 | Document–product consistency | The document describes behaviour the product does not have |
| Q14 | Cross-document consistency | Two project documents contradict each other |
| Q15 | Fairness and transparency | A consumer term is complete but substantively unfair or opaque |
| Q16 | Requirement actionability | A "requirement" cannot be implemented or verified by the receiving team |
| Q17 | Traceability | A conclusion cannot be walked back to fact and authority |
| Q18 | Preservation under repair | Fixing one defect regenerated or damaged unaffected verified work |
| Q19 | Boundary compliance | A hard line (§4.2) was crossed, or the tier was understated |
| Q20 | Confidentiality routing | Sensitive material was sent somewhere it should not have gone |

**Q12 is deliberately separate from Q5–Q9:** well-written and legally wrong is
a real and dangerous combination, and the bootstrap requires drafting quality
to be separable from legal correctness.

### 7.2 Controlled confidence language

One vocabulary, used everywhere, so calibration can be evaluated:

```text
clear requirement
strong interpretation
reasonable but contestable interpretation
open / unsettled question
insufficient facts
insufficient authority
jurisdiction unresolved
professional opinion required
```

Unqualified statements such as "this is compliant", "this is lawful",
"you are covered", "this is cleared" are prohibited outputs (B3).

### 7.3 Cheapest adequate artefact

Default to the smallest artefact that resolves the live uncertainty:

```text
matter brief        before   full memo
issue list          before   exhaustive research
authority table     before   polished advice
clause inventory    before   full redraft
redline             before   replacement agreement
knockout search     before   filing strategy
data-flow inventory before   privacy notice
licence inventory   before   compliance report
```

---

## 8. Non-goals

Inherited from bootstrap §33 and extended by this stage.

**Inherited:** not a law firm or substitute for regulated representation; not
court filing or advocacy; not a tax/immigration/criminal/family/employment/
patent/corporate omnibus; not a universal legal research database; not a
replacement for commercial legal information providers; not a central store of
consuming-project matters; not a regulatory-change SaaS; not a universal
policy-as-code engine; not a jurisdiction ontology project; not a compliance
certification authority; not a system that claims compliance without scoped
jurisdiction, facts, authority and valid-as-of context; not a generic
disclaimer generator.

**Added at Stage 1:**

| # | Non-goal | Why |
| --- | --- | --- |
| N1 | A template library or document generator | Documents must derive from actual product behaviour (bootstrap §4). A template catalogue invites invented facts, which is the failure mode the project exists to prevent. |
| N2 | A jurisdiction-pack taxonomy | Jurisdiction is matter context (§5.1). |
| N3 | Legal department operations tooling | Out of boundary (§6.2). |
| N4 | Contract lifecycle management | Operational, not legal production. |
| N5 | Autonomous legal sign-off at any tier | Hard line B3; every T2 artefact requires a named human reviewer before external use. |
| N6 | A multi-agent "law firm simulation" | Explicit bootstrap deferral; adds orchestration cost without adding legal correctness. |
| N7 | Retrieval infrastructure of its own | Stage 12 boundary: own the semantics, orchestrate the execution. |

---

## 9. Reusable vs project-specific boundary

The line the bootstrap requires to be drawn:

| Belongs to `legal-skills` (reusable) | Belongs to the consuming project |
| --- | --- |
| How to scope a matter | What this project is doing |
| How to resolve jurisdiction | Where this company is established and sells |
| How to model facts and assumptions | The actual data flows, manifests, commercial terms |
| The source hierarchy and currency rules | Which authorities this matter turned out to need |
| How to spot issues in a class of product | The issues this product raises |
| The drafting and review grammar | This project's approved clause positions and risk appetite |
| How to express uncertainty and escalate | Who this project escalates to |
| How to test legal-production quality | This project's accepted legal conclusions |
| The evaluation and regression architecture | This project's legal matter history |

**Test for a proposed core rule:** *would it still be true for a different
project, in a different jurisdiction, in a different year?* If no, it is
project instruction or pack behaviour, not core.

**Test for a proposed pack:** *is it a reusable matter specialisation that
materially changes production behaviour* — as opposed to a jurisdiction, a
document type, or one project's detail? (Stage 15 applies this.)

---

## 10. Interfaces with other projects

Stated as hypotheses for Stage 21 to test, not as accepted architecture.

| Counterpart | `legal-skills` supplies | `legal-skills` must not take over |
| --- | --- | --- |
| **Pactwright** | Legal requirements, constraints, review findings and verification inputs, with provenance and valid-as-of metadata, shaped to be consumable as Contract inputs and Evidence | Lifecycle, gating, Contract and Evidence semantics — Pactwright owns governance |
| **Deep Research** | The legal-specific layer: authority typology, binding force, currency, applicability | General evidence acquisition and synthesis — the boundary is *legal authority and applicability*, not *research* |
| **Software Engineering** | Legal requirements as implementable constraints; consistency checks against manifests, data flows and configuration | Implementation decisions and architecture |
| **UI/UX** | Disclosure, consent, transparency and age-assurance requirements with their legal basis | Interaction design |
| **Game Development / creative** | Asset provenance, licensing, likeness, trade dress and representation constraints | Creative direction |

Shared-abstraction candidates are **recorded, not promoted** (family rule:
share only after multiple independent domains show the same need):
valid-as-of metadata; source/provenance handoff; evidence-backed requirement
handoff; change-impact handoff; confidentiality-aware execution metadata.

---

## 11. Review and escalation points

Where human involvement is structurally required:

| # | Point | Requirement |
| --- | --- | --- |
| P1 | Matter intake | The requester confirms facts and states what is assumption. Facts supplied by an agent from a repository are evidence; facts supplied by inference are assumptions. |
| P2 | Jurisdiction resolution | If unresolved, work stops at analysis and does not reach conclusion. |
| P3 | Before any T2 artefact is used externally | A named human reviewer. |
| P4 | On any §4.4 trigger | T3 escalation; no conclusion stated. |
| P5 | Before routing a sensitive matter | Confidentiality decision is made *before* execution, not after (Stage 10). |
| P6 | On material project change | Bounded re-review of affected conclusions only. |
| P7 | On authority currency lapse | Re-verification before reuse of a prior conclusion. |

---

## 12. Exit-criteria verification

Stage 1 exit (bootstrap §7): *"a defensible legal-production boundary exists
without a fixed skill count or template catalogue."*

| Required by §7 | Where | Met |
| --- | --- | --- |
| Owned legal outcomes | §1.2 (O1–O16) | Yes |
| Intended users | §2 (U1–U5) | Yes |
| Core matter classes | §3 (M1–M7, perimeter, excluded) | Yes |
| Initial proving jurisdictions | §5.2 (J1–J4) | Yes |
| Human review requirements | §11 (P1–P7), §4.3 tiers | Yes |
| Regulated-practitioner handoffs | §4.4 (11 triggers), tier T3 | Yes |
| Explicit non-goals | §8 (inherited + N1–N7) | Yes |
| Reusable vs project-specific boundary | §9 | Yes |
| Interfaces with Pactwright and Production Skills | §10 | Yes |
| Nine candidate responsibilities each investigated | §6.1, §6.2 | Yes |
| Project charter persisted | §1 | Yes |
| Professional-boundary map persisted | §4 | Yes |
| Intended-user map persisted | §2 | Yes |
| Jurisdiction strategy persisted | §5 | Yes |
| Quality definition persisted | §7 | Yes |
| Review/escalation points persisted | §11 | Yes |

Negative checks:

| Must not have happened | Status |
| --- | --- |
| A fixed skill count declared | Not declared — §6.1 explicitly defers packaging to Stage 14 |
| A template catalogue declared | Not declared — prohibited by N1 |
| A legal subject admitted to core merely for being legal | No — §3.3 records the exclusions and the reason |
| Jurisdictions modelled as packs | No — §5.1 forbids it |
| Search-derived findings promoted to verified authority | No — §0.4 |
| Supplied books treated as read | No — Stage 2 handles them |

**Exit: met.**

---

## 13. Outputs for later stages

| Consumer | Must use |
| --- | --- |
| Stage 2 | §1.2 owned outcomes and §3 matter classes as the coverage map seed; §6 decisions |
| Stage 4 | §0.4 GAP-01; §3.2 perimeter classes as gap-research targets |
| Stage 5 | §5.3 distinctions; §0.4 SRA citation-form check |
| Stage 6 | §1.1 chain; §7.1 dimensions |
| Stage 9 | §7.1, §7.2, §4.3, §4.4 |
| Stage 10 | §11 P5; §4.2 B2 (privilege) |
| Stage 13 | §6 decisions; §8 non-goals as the over-engineering guardrail |
| Stage 14 | §1.2 outcomes as the responsibility set; §6.1 packaging deferral |
| Stage 15 | §9 pack test; §5.1 jurisdiction rule |
| Stage 18 | §7.1 Q1–Q20 as the independent-failure axes |
| Stage 20 | §1.1 positioning; §4 boundary statement |
| Stage 21 | §10 interface hypotheses |

## 14. Open questions carried forward

| # | Question | Owner stage |
| --- | --- | --- |
| GAP-01 | Authoritative-source inspection unavailable (§0.4) | 4, 5, 11 |
| GAP-02 | Are M1–M7 the right core classes, or does professional practice evidence show a different clustering? | 4 |
| GAP-03 | Does the T0–T4 tier model survive contact with actual professional practice, or is it an invention? | 4 |
| GAP-04 | Is legal–product consistency (§6.1) genuinely distinctive, or does existing tooling already cover it? | 11, 13 |
| GAP-05 | Does J1+J2+J3 prove enough jurisdiction discipline, or is a fourth needed for the Worldstack stress test? | 17 |
| GAP-06 | Are Q1–Q20 independently measurable, or do some collapse in practice? | 18 |
