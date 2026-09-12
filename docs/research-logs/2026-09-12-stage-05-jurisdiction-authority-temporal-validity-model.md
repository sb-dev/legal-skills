# Stage 5 — Jurisdiction, Authority and Temporal-Validity Model

**Project:** `legal-skills`  
**Bootstrap stage:** 5 — Define Jurisdiction, Authority and Temporal-Validity Model  
**Status:** Complete  
**Date:** 12 September 2026  
**Stage 4 input:** `2026-09-12-stage-04-professional-practice-challenge.md`

## 1. Stage purpose

Stage 4 established that legal-production quality depends on jurisdiction fit, authority fidelity, source coverage and temporal validity being independently inspectable.

This stage defines the smallest reusable model needed to answer:

> For this proposition, which legal context applies, which authority actually supports it, and for what period can the proposition responsibly be treated as valid?

The model deliberately keeps three things separate:

```text
matter / issue legal context
≠
authority record
≠
legal proposition / interpretation
```

It also preserves the Stage 4 rule that legal research must distinguish source authority from source coverage. An official database may be authoritative for material it contains without being exhaustive for the question being asked.

This stage is a data and reasoning contract for later workflow and artefact design. It is **not** a universal conflict-of-laws engine, legal ontology, legal database schema or runtime implementation.

---

## 2. Governing inputs

This stage consumes:

- [`2026-09-08-legal-skills-new-project-bootstrap-process.md`](2026-09-08-legal-skills-new-project-bootstrap-process.md)
- [`2026-09-12-stage-01-project-goal-users-and-professional-boundary.md`](2026-09-12-stage-01-project-goal-users-and-professional-boundary.md)
- [`2026-09-12-stage-03-five-book-extraction.md`](2026-09-12-stage-03-five-book-extraction.md)
- [`2026-09-12-stage-04-professional-practice-challenge.md`](2026-09-12-stage-04-professional-practice-challenge.md)

Stage 4 capability `Q3 — Jurisdiction, temporal and source-scope framing` is the immediate design input.

The bootstrap requires the model to preserve at least:

```text
jurisdiction ≠ governing law ≠ forum
authority ≠ proposition ≠ interpretation
publication date ≠ effective date
regulator guidance ≠ legislation
registry search ≠ legal clearance
current source ≠ current law automatically
```

---

# 3. Current authoritative-source reconnaissance

The model was tested against source classes that expose different validity and coverage problems.

## 3.1 UK legislation — `legislation.gov.uk`

The National Archives' revised-legislation service exposes:

- original and revised text;
- provision-level extent information;
- commencement / in-force annotations;
- textual and non-textual modifications;
- outstanding changes and effects not yet applied editorially;
- point-in-time information.

Crucially, revised legislation may state that it is not fully up to date where known effects have not yet been applied to the displayed text.

Relevant sources:

- `https://www.legislation.gov.uk/`
- `https://www.legislation.gov.uk/pdfs/GuideToRevisedLegislation_Oct_2013.pdf`

### Design consequence

```text
official revised text
≠
proof that every known legal effect is already incorporated into displayed wording
```

A verifier must inspect outstanding effects where the page exposes them.

## 3.2 England and Wales case law — Find Case Law

The National Archives describes Find Case Law as the official public source for judgments and decisions from courts and tribunals in England and Wales.

Its coverage guidance also makes clear that the collection is not a complete record of every judgment or decision. Coverage varies by court and date. It also warns that a judgment may have been appealed even where the appeal judgment is not present in the service.

Relevant sources:

- `https://caselaw.nationalarchives.gov.uk/about-find-case-law`
- `https://caselaw.nationalarchives.gov.uk/courts-and-coverage`
- `https://caselaw.nationalarchives.gov.uk/how-to-search-find-case-law`

### Design consequence

```text
official judgment source
≠
complete case-law universe

no result in Find Case Law
≠
case does not exist

judgment found
≠
judgment has no later treatment / appeal
```

Neutral citation is a useful identity key where available, but proposition-level reliance still requires the actual supporting passage and context.

## 3.3 Assimilated law after Brexit

The Retained EU Law (Revocation and Reform) Act 2023 removed retained EU supremacy and retained general principles at the end of 2023 and renamed remaining retained EU law as assimilated law.

The Act's savings preserve earlier interpretive effects for events or acts occurring before the end of 2023 where applicable. The Department for Business and Trade's REUL / assimilated-law dashboard received its final update in July 2026 and is intended to be decommissioned in January 2027, with a final downloadable dataset retained.

Relevant sources:

- `https://www.legislation.gov.uk/ukpga/2023/28`
- `https://www.legislation.gov.uk/ukpga/2023/28/notes/division/7/index.htm`
- `https://www.legislation.gov.uk/ukpga/2023/28/notes/division/12/index.htm`
- `https://www.gov.uk/government/publications/retained-eu-law-dashboard`

### Design consequence

A matter involving EU-derived UK law cannot be resolved from the label “EU law” or “retained EU law” alone.

At minimum resolve:

```text
relevant event / act date
which domestic / assimilated instrument applies
whether a pre-2024 saving is material
territorial scope
current amendments / revocation / restatement
```

The dashboard is useful inventory/history evidence but must not become the canonical live source of current law.

## 3.4 EU law — EUR-Lex

EUR-Lex distinguishes original legal acts from consolidated texts. Consolidated text combines an act with later amendments for convenience at a point in time, but EUR-Lex states that consolidated text has no legal effect. Authentic versions are the relevant acts published in the Official Journal.

EUR-Lex also distinguishes dates such as:

```text
date of document / adoption
date of entry into force
date of application
```

These may differ.

Relevant sources:

- `https://eur-lex.europa.eu/collection/eu-law/consleg.html`
- `https://eur-lex.europa.eu/EN/legal-content/glossary/consolidation.html`

### Design consequence

```text
consolidated EU text
→ excellent working representation
but
→ not itself the legal act with legal effect
```

A material proposition relying on a consolidated text should retain links to the authentic basic/amending acts where legal effect matters.

## 3.5 Regulator rules and guidance — FCA example

The FCA Handbook contains the complete record of FCA legal instruments and exposes a timeline that can show past, current and future versions and compare amendments.

Relevant sources:

- `https://handbook.fca.org.uk/`
- `https://handbook.fca.org.uk/guides/timeline-guide`

### Design consequence

A regulator source may provide its own temporal model. Legal Skills should use that model instead of replacing it with a generic “last updated” timestamp.

Rules and guidance inside one regulator system must still be distinguished by their legal status.

## 3.6 Trade-mark registries and search services

The UK IPO requires an applicant to choose relevant goods/services and check for identical or similar registered marks. It recommends professional advice when similar marks are found.

EUIPO states that availability searches reduce risk but do not rule it out; its similarity report is not exhaustive. TMview includes participating national, EU and other offices.

WIPO's Global Brand Database includes Madrid registrations and participating national/regional collections but does not guarantee accuracy or completeness of all data. Madrid Monitor provides more current international-registration transaction status and can show different protection states by designated territory.

Relevant sources:

- `https://www.gov.uk/how-to-register-a-trade-mark/before-you-apply`
- `https://www.gov.uk/guidance/how-to-classify-trade-marks`
- `https://www.euipo.europa.eu/en/trade-marks/before-applying/availability`
- `https://www.euipo.europa.eu/en/help-centre/tm/faq-search-availability`
- `https://www.wipo.int/en/web/global-brand-database`
- `https://www.wipo.int/en/web/global-brand-database/terms_and_conditions`
- `https://www3.wipo.int/madrid/monitor/en/`

### Design consequence

```text
registry search result
≠
complete rights search
≠
conflict conclusion
≠
clearance
```

Registry evidence must preserve territory, class/terms, search method, source coverage and retrieval time.

## 3.7 Corporate registries — Companies House example

Companies House exposes the public UK company register and real-time updates, but its current guidance warns that the service is not a complete source of company law/information and that occasional inaccuracies can occur. The search service itself states that Companies House does not check the accuracy of information filed.

Identity-verification requirements introduced from 2025 improve assurance about specified people but do not turn every registered company fact into independently verified truth.

Relevant sources:

- `https://www.gov.uk/guidance/searching-the-companies-house-register`
- `https://company-information.service.gov.uk/`
- `https://www.gov.uk/guidance/verifying-your-identity-for-companies-house`

### Design consequence

Registry evidence should preserve:

```text
what the registry says
≠
what has independently been proven true
```

---

# 4. Design principles

## P1 — Legal context is issue-specific

A matter may involve several legal contexts at once.

Example:

```text
UK company
selling digital service into UK and EU
processing EU and UK personal data
using US supplier
contract choosing English law
EU trade mark registration
```

There is no responsible single value for:

```text
jurisdiction = "UK"
```

Instead, legal context should be resolved for the issue being analysed.

## P2 — Unknown is a valid state

If governing law, forum, territorial scope or material date is unresolved, record it as unresolved.

Do not silently select the user's location, the company's incorporation country or the governing-law clause as a universal substitute.

## P3 — Facts that establish legal context need provenance

Actor location, place of establishment, contract terms, consumer location, asset location and processing territory are factual inputs. They must inherit the Stage 4 fact-status discipline:

```text
verified
asserted
inferred
assumed
disputed
unknown
```

## P4 — Authority type and force are separate

A court judgment is an `authority_type`.

Whether it is binding, persuasive or merely informative is a **contextual relationship** between that authority, proposition and decision-maker.

Likewise regulator guidance is guidance by type, but its practical/legal relevance varies by regime.

## P5 — Temporal validity is interval- and event-aware

Do not represent legal currency only as:

```text
last_updated = 2026-09-12
```

The relevant questions are:

```text
when did the rule / version become effective?
when did it cease or change?
for which event / act / transaction date is it being applied?
are there transitional / saving rules?
```

## P6 — Source freshness does not prove legal currency

A page retrieved today may display:

- historical law;
- prospective law;
- consolidated but legally non-operative text;
- guidance under review;
- a judgment later appealed;
- a registry record later changed.

## P7 — Negative research needs a coverage record

A finding such as:

```text
no conflicting mark found
no case found
no registration found
```

is only as strong as:

```text
sources searched
coverage of those sources
query / filters
relevant date
known blind spots
```

## P8 — Preserve source-native identifiers

Where available, retain stable legal identifiers rather than relying on display titles alone:

```text
UK legislation URI / year + chapter / SI number
neutral citation
CELEX / ELI / ECLI
trade-mark application / registration number
company number
regulator rule identifier
```

## P9 — Current-law and historical-law questions are different tasks

The system must ask whether the proposition is needed:

```text
as law stands now
or
as law stood when a past event occurred
```

A present-day consolidated source is not enough for a historical question.

## P10 — No universal legal source ranking

A primary statute, regulator rule, case, registry record and official guidance answer different questions.

The correct source is proposition-specific.

---

# 5. Jurisdiction-context contract

The smallest useful jurisdiction model has **matter facts** and **issue-specific legal context**.

## 5.1 Matter-level jurisdiction facts

Record only fields relevant to the matter:

```text
matter_territories[]
actors[]
  role
  entity / person
  location / establishment
  fact_status
  provenance
consumer_or_user_locations[]
places_of_offering[]
data_subject_locations[]
asset_or_right_territories[]
contract_choice_of_law_terms[]
material_dates[]
cross_border_questions[]
```

These are factual/legal-context inputs, not conclusions that one jurisdiction governs everything.

## 5.2 Issue-specific legal context

Each material issue may resolve:

```text
issue_id / issue_description
legal_system_or_jurisdiction
territorial_application
governing_law
forum / court
regulator
registry
relevant_actor_nexus
relevant_material_date
analysis_as_of
context_status
context_basis / evidence
unresolved_cross_border_questions[]
```

### `context_status`

Use a simple controlled state:

```text
resolved
provisional
contested
unknown
```

No numerical jurisdiction confidence is justified.

## 5.3 Jurisdiction vs governing law vs forum

Preserve the distinction explicitly.

### Jurisdiction / legal system

Which body of law is potentially relevant to the issue.

### Governing law

Which law governs a contract, obligation or question under an applicable choice/conflict rule.

### Forum

Which court, tribunal, regulator, arbitrator or other decision-maker has authority to hear or determine the matter.

These can diverge.

Example:

```text
English governing law
+ arbitration seated in Paris
+ EU competition issue
+ UK company
```

must not be flattened into one field.

## 5.4 Territory and legal-right scope

Some issues are intrinsically territorial.

Examples:

```text
trade mark → protected / applied-for territory + goods/services
copyright → territorial right / use / distribution context
privacy → establishment / data-subject / processing / offering nexus
consumer → market / consumer location / trader establishment
regulatory → authorised entity + activity + market / regulator perimeter
```

The core model should carry the necessary facts and unresolved questions without embedding every specialist conflict rule.

---

# 6. Temporal-validity contract

## 6.1 Matter dates

A matter may require several dates:

```text
event_date
contract_or_transaction_date
product_launch_or_change_date
processing_start_date
filing_or_application_date
infringement_or_use_date
decision_or_approval_date
requested_historical_date
```

Do not invent a universal `matter_date` if several dates affect different issues.

## 6.2 Analysis dates

Record:

```text
retrieved_at
analysis_as_of
last_verified_at
```

### `retrieved_at`

When the source was fetched.

### `analysis_as_of`

The date for which the work claims legal currency.

### `last_verified_at`

When identity/status/currency was last actively checked.

These dates answer different questions.

## 6.3 Authority lifecycle dates

Depending on source type, record relevant fields from:

```text
made / enacted / adopted
publication
judgment / decision
entry_into_force / commencement
application
amendment_effective
repeal / revocation / expiry
future_effective_change
```

Not every authority has every date.

## 6.4 Effective interval

Where knowable, represent applicability as one or more intervals:

```text
effective_from
effective_until
territorial_scope
purpose / provision qualification
source_of_effective_date
```

This accommodates provisions that commence:

- on different dates;
- for different purposes;
- in different territories.

## 6.5 Transitional and saving rules

Record explicitly when current law changes do not apply straightforwardly to earlier events.

Candidate field:

```text
transitional_or_saving_effect:
  present | absent | unknown
  description
  authority
```

The assimilated-law transition is a clear example: post-2023 interpretation cannot automatically be projected backward to earlier acts/events.

## 6.6 Prospective law

Future law can be relevant without being current law.

Use a distinct state:

```text
prospective
```

and retain the future effective date / commencement dependency.

Do not describe Royal Assent, publication or adoption as equivalent to operative applicability where commencement/application occurs later.

---

# 7. Authority-record contract

The authority record describes the source. It does not contain the whole legal conclusion.

## 7.1 Identity

```text
authority_id
canonical_identifier
short_title
authority_type
source_url
issuing_body / court / regulator / registry
jurisdiction_or_system
language
```

Examples of canonical identifiers:

```text
2026 c. 18
S.I. 2026/123
[2026] UKSC 32
CELEX: 32026R1315
ECLI:EU:C:2026:...
UK00004123456
EUTM application / registration number
Companies House company number
FCA rule identifier
```

## 7.2 Authority type

Do not force all sources into primary/secondary alone.

Candidate types:

```text
primary_legislation
secondary_or_delegated_legislation
treaty_or_international_instrument
court_judgment
tribunal_decision
regulator_rule
regulator_guidance
official_government_guidance
official_registry_record
official_notice_or_gazette
contract_or_private_instrument
professional_guidance
secondary_commentary
other
```

`contract_or_private_instrument` can be legally operative between parties but is not public legal authority in the same sense as legislation or precedent.

## 7.3 Source representation

Record what was actually read:

```text
representation_type
  original / as_enacted
  revised
  consolidated
  authentic_official_publication
  judgment_text
  report
  registry_record
  guidance_version
  summary / headnote
representation_date_or_version
```

This prevents a consolidated or summary representation being silently treated as the legal source itself.

## 7.4 Contextual legal force

Do not store a universal `binding=true` on the authority.

Instead, when authority is linked to a proposition / issue, record a contextual force such as:

```text
controlling
binding
persuasive
guidance
official_evidence
informative
unknown
```

and record:

```text
force_basis
```

Examples:

- court hierarchy;
- statute / delegated power;
- regulator rulebook status;
- contractual choice;
- registry evidential role.

## 7.5 Temporal fields

As relevant:

```text
document_date
publication_date
judgment_or_decision_date
effective_from
effective_until
application_from
amendment_status
repeal_or_revocation_status
future_change_status
```

## 7.6 Later treatment and relationship state

For cases or instruments where material:

```text
appeal_status
later_treatment[]
amends[]
amended_by[]
repeals[]
repealed_by[]
implements[]
implemented_by[]
related_authorities[]
```

Do not require all relationships for every source. Capture only those needed to support the proposition or currency determination.

## 7.7 Source coverage

A source record used for search should carry:

```text
coverage_status
  sufficient_for_question
  partial
  unknown
coverage_note
```

Examples:

- Find Case Law does not cover every judgment;
- WIPO Global Brand Database depends on participating sources and cannot guarantee completeness;
- Companies House is an official registry but not an independently verified statement of every filed fact;
- a licensed database may have publisher-specific coverage.

## 7.8 Retrieval and verification

Record:

```text
retrieved_at
last_verified_at
```

Do not use one opaque verification score.

---

# 8. Verification-state contract

A material proposition should only be described as verified to the extent the necessary checks were completed.

Use independent flags / states:

```text
identity_verified
source_text_verified
jurisdiction_verified
temporal_status_verified
later_treatment_checked
source_coverage_checked
proposition_support_verified
```

Each can be:

```text
yes
no
not_applicable
unknown
```

## 8.1 Why not one `verification_status`?

Because these failures are materially different:

```text
real source, wrong jurisdiction
real source, stale version
current source, wrong proposition
valid proposition, later overruled case
correct database, incomplete search coverage
```

A single “verified” badge would hide the repair path.

## 8.2 Minimum for a material current-law proposition

Normally require:

```text
identity_verified = yes
source_text_verified = yes
jurisdiction_verified = yes
temporal_status_verified = yes
proposition_support_verified = yes
```

and where relevant:

```text
later_treatment_checked = yes
source_coverage_checked = yes
```

If a required check remains unknown, the proposition must remain qualified.

---

# 9. Proposition-to-authority contract

Authority and proposition are many-to-many.

One authority can support several propositions. One proposition may require several authorities.

## 9.1 Proposition record

Stage 6 will define the durable artefact, but Stage 5 requires the following semantic contract:

```text
proposition_text
issue_context
jurisdiction_context
temporal_scope
proposition_status
authority_links[]
interpretation_note
limitations / conditions
contrary_or_limiting_authority[]
```

## 9.2 Proposition status

Use evidence-qualified states such as:

```text
supported
qualified
disputed
unresolved
superseded
```

Do not infer certainty from the number of citations.

## 9.3 Authority link

Each link should preserve:

```text
authority_id
relationship
  supports
  limits
  contradicts
  explains
  historical_context
pinpoint_reference
supporting_passage_verified
contextual_force
contextual_force_basis
```

## 9.4 Pinpoints

Where the source permits, preserve the smallest stable location adequate for verification:

```text
section / regulation / article
paragraph
page
judgment paragraph
registry field / event
rule identifier
```

A broad home-page citation is insufficient when a material proposition depends on a specific provision.

## 9.5 Interpretation remains separate

The authority link establishes what source text supports the proposition.

It does not eliminate interpretive work.

Keep distinct:

```text
source text
→ extracted proposition
→ interpretation / status
→ application to facts
→ conclusion / risk
```

---

# 10. Negative-search evidence contract

Stage 4 showed that negative findings are unusually easy to overstate.

For a material negative result, record:

```text
negative_claim
sources_searched[]
search_date
query / identifiers / filters
territory
class / category where relevant
coverage_note
known_blind_spots
result
residual_uncertainty
```

Examples:

```text
no case found
no similar registered mark found
no company filing found
no regulator instrument found
```

A negative claim should default to wording such as:

```text
"No result was found in the searched sources within the recorded scope"
```

unless broader absence has genuinely been established.

---

# 11. Source-specific verification profiles

The core model should support source-specific checks without hard-coding one workflow for every authority class.

## 11.1 UK legislation profile

For a material provision:

```text
resolve Act / SI identity
→ select original or revised representation appropriate to question
→ inspect provision text
→ inspect commencement / I-notes where material
→ inspect extent / territorial application
→ inspect amendments / modifications
→ inspect outstanding effects not yet applied
→ resolve relevant point in time
→ preserve pinpoint
```

### Guardrail

If `legislation.gov.uk` states that effects remain unapplied editorially, do not treat displayed revised wording alone as conclusively current.

## 11.2 England and Wales case profile

```text
resolve neutral citation / case identity
→ retrieve official judgment where available
→ identify court / date / judgment
→ locate supporting paragraphs
→ determine contextual precedential force
→ check appeal / later treatment where material
→ record Find Case Law coverage limitation for negative research
```

### Citation representation

Where litigation/court-document practice matters, preserve neutral citation and appropriate report reference according to the applicable practice direction. Do not make court-bundle citation rules a universal runtime requirement for every internal research note.

## 11.3 EU act profile

```text
resolve CELEX / ELI
→ identify authentic basic act
→ identify amendments / corrigenda
→ use consolidated text for working readability where useful
→ verify authentic source(s) for legal effect
→ distinguish adoption / publication / entry into force / application
→ resolve territorial / personal / temporal scope
→ preserve applicable version date
```

### Guardrail

`consolidated_text = true` must never imply `has_legal_effect = true` merely because the consolidated wording is current.

## 11.4 Assimilated-law profile

```text
identify UK domestic / assimilated instrument
→ determine event / act date
→ determine whether pre-2024 savings matter
→ inspect current legislation.gov.uk status
→ identify reform / revocation / restatement
→ use REUL dashboard only as supporting inventory/history
→ apply current domestic interpretive framework for post-2023 matters unless a saving/special rule changes that result
```

## 11.5 Regulator rulebook profile

Where the regulator provides a timeline:

```text
resolve rule identifier
→ select matter date
→ retrieve version in force on that date
→ distinguish rule / guidance / evidential provision
→ inspect scheduled future changes if relevant
→ preserve regulator-specific version metadata
```

FCA Handbook is the proving example; other regulators need equivalent source-specific research.

## 11.6 Regulator / government guidance profile

```text
resolve publisher and page/document identity
→ publication / update date
→ scope and audience
→ legal status
→ whether guidance is current / under review / withdrawn
→ supporting passage
```

### Guardrail

Do not label guidance as legislation or binding law merely because it comes from an official body.

## 11.7 Trade-mark registry profile

```text
candidate sign
→ territory / registry
→ goods / services + class / terms
→ search strategy
→ applications + registrations + status
→ similar / identical results
→ data-source coverage
→ retrieval date
→ residual unregistered / non-database rights risk
→ clearance / filing escalation where required
```

### Guardrail

`registry_search_complete = yes` is not a synonym for `mark_cleared = yes`.

## 11.8 Corporate-registry profile

```text
company identifier
→ official registry record
→ filing / officer / status field relied on
→ retrieval date
→ filing date / effective date where relevant
→ registry caveat / verification status
→ corroborating evidence if consequence requires
```

### Guardrail

A registered filing is evidence of what was filed and recorded; it is not automatically proof that every underlying factual assertion is true.

---

# 12. Current-law verification algorithm

For a material proposition intended to represent current law:

```text
1. define the proposition question
2. resolve issue-specific jurisdiction / governing-law / forum context
3. set analysis_as_of
4. identify appropriate authority class
5. retrieve authoritative source representation
6. verify authority identity
7. verify territorial / personal scope
8. verify commencement / effective / application status
9. inspect amendments / repeal / revocation / outstanding effects
10. inspect appeal / later treatment where material
11. locate the supporting passage
12. classify contextual legal force
13. record source coverage / negative-search limits where material
14. link authority to independently expressed proposition
15. record qualifications / contrary authority / uncertainty
```

This algorithm is deliberately source-sensitive. Steps can be `not_applicable` where a source type does not require them.

---

# 13. Historical-law verification algorithm

For a proposition about law at a past date:

```text
1. identify the legally relevant event / transaction date
2. identify all potentially relevant legal systems / territories
3. retrieve the authority version effective at that date
4. inspect transitional / saving provisions
5. distinguish later amendments from law then in force
6. identify case law / guidance available and operative as of that date where material
7. preserve later developments separately as subsequent context
8. state analysis valid-for date explicitly
```

Do not back-project current law simply because today's source page is easier to find.

---

# 14. Temporal-state vocabulary

For later artefacts, use a small vocabulary where helpful:

```text
not_yet_in_force
in_force
partially_in_force
prospective
expired
repealed
revoked
superseded
historical_version
status_unknown
```

These states describe the authority/provision, not whether the proposition is legally correct.

---

# 15. Change triggers

A legal proposition or dependent project requirement should be considered for re-review when its dependency chain records a trigger such as:

```text
new amendment / repeal / revocation
commencement or application date reached
new court decision or appeal
later treatment changes case reliance
regulator rule / guidance update
registry application / registration status change
new market / territory
new actor / establishment location
contract governing-law / forum change
new material event date or factual correction
source coverage changes materially
```

The trigger should identify affected dependencies. It does not require re-running the whole matter by default.

---

# 16. Failure taxonomy for Stage 5

## J1 — Jurisdiction flattening

**Failure:** one `jurisdiction=UK` value is applied to privacy, consumer, contract, IP and regulatory issues.

**Repair:** restore issue-specific context and re-run only affected propositions.

## J2 — Governing-law / forum conflation

**Failure:** chosen law is assumed to determine forum or regulator.

**Repair:** resolve each relationship separately.

## J3 — Location laundering

**Failure:** user's current location or company incorporation is silently treated as controlling law.

**Repair:** restore provenance and analyse the legally relevant nexus.

## T1 — Publication / effect conflation

**Failure:** published or enacted law is treated as operative before commencement/application.

**Repair:** resolve operative date and qualify prospective rules.

## T2 — Current-source / current-law conflation

**Failure:** recently retrieved page is assumed legally current.

**Repair:** inspect source-native version, amendments and status metadata.

## T3 — Historical back-projection

**Failure:** current law is used for an earlier event without transition analysis.

**Repair:** retrieve historical version and savings/transitional rules.

## A1 — Consolidation laundering

**Failure:** EUR-Lex consolidated text is represented as the authentic legal act.

**Repair:** link working consolidated text to authentic Official Journal acts and verify effect.

## A2 — Revised-text lag ignored

**Failure:** displayed `legislation.gov.uk` wording is relied on despite outstanding unapplied effects.

**Repair:** inspect the outstanding effects and relevant amending instrument.

## A3 — Case found / later treatment ignored

**Failure:** real judgment is relied on without checking material appeal or later treatment.

**Repair:** update status and dependent proposition.

## A4 — Negative-search overclaim

**Failure:** one source returns no result and the system concludes legal absence.

**Repair:** inspect collection coverage, search additional appropriate source and qualify residual uncertainty.

## A5 — Guidance-to-law promotion

**Failure:** regulator or government guidance is described as legislation or binding rule without basis.

**Repair:** restore authority type and contextual legal force.

## R1 — Registry-to-clearance promotion

**Failure:** trade-mark registry search becomes categorical clearance.

**Repair:** restore search scope, classes, territory, coverage and professional/clearance boundary.

## R2 — Registry-to-truth promotion

**Failure:** Companies House filing is treated as independently verified factual truth.

**Repair:** distinguish registry evidence from underlying factual proof and corroborate where consequence requires.

## P1 — Citation without proposition support

**Failure:** real authority is attached to a proposition it does not actually support.

**Repair:** locate supporting passage or remove/qualify proposition.

---

# 17. Candidate evaluation dimensions introduced by Stage 5

Later benchmarks should add explicit tests for:

1. **issue-specific jurisdiction fit** — no matter-level jurisdiction flattening;
2. **governing-law / forum separation** — distinct when legally different;
3. **jurisdiction fact provenance** — relevant location / choice terms are sourced, not assumed;
4. **authority identity integrity** — canonical source is real and correctly identified;
5. **authority-type classification** — legislation, judgment, guidance, registry evidence remain distinct;
6. **representation integrity** — original/revised/consolidated/summary status is explicit;
7. **contextual force correctness** — binding/persuasive/guidance status is issue-specific;
8. **commencement / application correctness** — operative dates are not inferred from publication alone;
9. **historical-version correctness** — past events use the law applicable at the relevant time;
10. **later-treatment completeness** — material appeal / amendment / repeal checked;
11. **source-coverage awareness** — negative results respect source limitations;
12. **proposition-to-pinpoint traceability** — material proposition maps to the actual supporting source location;
13. **registry-scope discipline** — search evidence is not promoted to legal clearance;
14. **change-trigger completeness** — dependency-invalidating events are identifiable;
15. **valid-as-of clarity** — the legal conclusion has an explicit analysis date / period.

---

# 18. Minimal implementation shape for later stages

Stage 5 does not require a database.

Markdown or structured YAML-like records are sufficient during bootstrap.

A future minimal representation could resemble:

```yaml
legal_context:
  issue: "consumer cancellation"
  legal_system: "England and Wales"
  governing_law: null
  forum: null
  regulator: "CMA"
  territory: ["England", "Wales"]
  material_date: "2026-09-12"
  analysis_as_of: "2026-09-12"
  status: "provisional"
  unresolved:
    - "confirm whether service is offered into Northern Ireland"

authority:
  id: "example-authority-id"
  type: "official_government_guidance"
  source_url: "..."
  issuing_body: "CMA"
  publication_date: "..."
  retrieved_at: "2026-09-12"
  representation_type: "guidance_version"
  coverage_status: "sufficient_for_question"
  verification:
    identity_verified: yes
    source_text_verified: yes
    jurisdiction_verified: yes
    temporal_status_verified: yes
    proposition_support_verified: yes

proposition_link:
  proposition: "..."
  relationship: "supports"
  pinpoint: "section / paragraph"
  contextual_force: "guidance"
  limitations: "..."
```

This is illustrative only. Stage 6 owns the durable matter / fact / issue / proposition artefacts and should simplify further where possible.

---

# 19. Explicit non-goals

Stage 5 does **not** introduce:

```text
universal conflict-of-laws engine
universal hierarchy of every legal source
legal knowledge graph
automatic precedent citator replacement
automatic trade-mark clearance engine
central registry mirror
universal risk score
provider-specific database dependency
full temporal database for all legislation
```

Those would be over-engineering without implementation evidence.

The reusable core is the reasoning and evidence contract.

---

# 20. Decisions carried into Stage 6

Stage 6 should treat the following as settled inputs unless new evidence overturns them:

1. legal context is issue-specific, not one matter-level jurisdiction string;
2. jurisdiction, governing law, forum, regulator and registry are separate concepts;
3. relevant jurisdiction facts need fact-status and provenance;
4. authority records describe sources, not conclusions;
5. legal force is contextual to authority + proposition + decision-maker;
6. publication, commencement/effect, application and analysis dates are distinct;
7. current and historical legal questions require different version-selection behaviour;
8. source coverage must be explicit when negative research is material;
9. material propositions need a verified supporting passage / pinpoint where available;
10. verification dimensions remain separate rather than collapsed into one confidence score;
11. registry searches are evidence within a bounded search, not categorical clearance;
12. change triggers should invalidate dependent work rather than force full-matter regeneration.

---

# 21. Stage completion assessment

## Required: smallest useful jurisdiction context

**Satisfied.** Sections 5 and 18 define a bounded, issue-specific context without building a conflict-of-laws engine.

## Required: authority record

**Satisfied.** Sections 7 and 8 define identity, type, representation, force, temporal state, coverage and verification.

## Required: temporal-validity contract

**Satisfied.** Section 6 distinguishes matter dates, source dates, commencement/application, effective intervals, transitional rules and analysis dates.

## Required: current authoritative-source research

**Satisfied.** The model was challenged against UK legislation, Find Case Law, assimilated-law sources, EUR-Lex, FCA rule timelines, trade-mark registries and Companies House.

## Required: proposition tied to verified authority and context

**Satisfied.** Section 9 defines the proposition-authority relationship and Section 12 defines the current-law verification sequence.

## Exit decision

**Stage 5 is complete.**

A material proposition can now be represented with:

```text
issue-specific legal context
+
verified authority identity / source representation
+
contextual legal force
+
source coverage
+
temporal validity
+
supporting pinpoint
+
verification state
+
valid-as-of scope
```

without pretending that authority retrieval itself resolves legal interpretation or application.

The next required stage is **Stage 6 — Define Matter, Fact, Issue and Legal-Reasoning Artifacts**.