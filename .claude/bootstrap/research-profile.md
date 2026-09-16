# Legal Bootstrap Research Profile

This profile specialises the shared `bootstrap-research` and `direct-source-extraction` skills for `legal-skills`.

It defines legal evidence priorities and domain-specific constraints. It does not replace the governing bootstrap specification.

## Governing bootstrap

```text
docs/research-logs/2026-09-08-legal-skills-new-project-bootstrap-process.md
```

## Legal evidence hierarchy

Prefer the strongest source appropriate to the proposition and jurisdiction. Typical source classes include:

```text
enacted legislation / official legislative repositories
judgments / official court and tribunal sources
regulator rules, decisions, notices and guidance
official registries and filing systems
treaties / official supranational material
government guidance and consultations
recognised professional-body material for professional-practice evidence
official product / database / API documentation for tooling claims
high-quality practitioner or academic commentary for interpretation, disagreement and practice discovery
```

Binding effect and persuasive value vary by jurisdiction and matter. Do not turn this list into a universal numeric ranking.

Secondary sources may identify issues and authorities. They do not replace appropriate current authority for a material substantive-law proposition.

## Books versus legal authority

Keep this distinction explicit:

```text
foundational books
→ durable legal-production method / professional practice

authoritative current sources
→ what law, guidance, registry evidence, or other authority establishes
  for a defined jurisdiction, matter, and date
```

A book is not current legal authority merely because it accurately explains doctrine or practice.

## Required legal provenance

For material legal findings capture as applicable:

```text
research question
jurisdiction / territory
matter date or temporal context
proposition supported
authority / source type
source title
stable URL or identifier
publication / judgment / made date
effective / commencement / update date
retrieved-at date
section / paragraph / page / stable location
applicability
limitations / contrary authority
confidence or unresolved uncertainty
dependent conclusion / project implication
```

A conclusion must not become more certain than its facts, authority, jurisdiction, temporal analysis, or unresolved interpretive questions justify.

## Currency and temporal validity

Where material, distinguish:

```text
law made
law commenced / effective
law amended / repealed
judgment date
appeal / later treatment
guidance publication / update date
retrieved-at date
analysis valid-as-of date
```

Search for amendments, commencement, later treatment, superseding guidance, and current regulator material when these could change the conclusion.

## Confidentiality and privilege

Do not send privileged, confidential, unpublished, personal, or commercially sensitive material to external retrieval services without explicit approval.

Prefer local inspection for supplied books and project-local documents. Apply the same care to any external AI, search, parsing, or crawling service when matter confidentiality is material.

## Stage-specific research routing

### Stage 2 — five-book corpus selection

Use bounded reconnaissance only far enough to compare candidate books, editions, source access, and complementary coverage. Do not collapse selection into direct extraction.

### Stage 3 — five-book extraction

Use `direct-source-extraction` and inspect the supplied books directly. Prefer local `Read`/`Grep`/`Glob` access. External parsing is a fallback only when local inspection is inadequate and external processing is acceptable.

Publisher descriptions, reviews, web summaries, and model memory do not satisfy direct-source examination.

### Stage 4 — professional-practice challenge

Research independently across the legal-production boundary rather than searching only for confirmation of book-derived methods.

Actively investigate omitted responsibilities, competing methods, failure conditions, contrary evidence, and current professional practice across the areas named by the bootstrap.

### Stage 5 — jurisdiction, authority and temporal validity

Prefer authoritative legal sources. Preserve jurisdiction, authority status, dates, and validity explicitly. Do not collapse research evidence and legal application into one undifferentiated conclusion.

### Stage 11 — AI skills, databases, registries and tools

Use native web search plus official provider documentation for the capability landscape. Firecrawl's developer-index capability may be useful for READMEs, API docs, GitHub issues, and merged PRs.

Developer-index evidence is tooling evidence, not substantive legal authority.

## Firecrawl policy

Use Claude Code `WebSearch` and `WebFetch` first.

Escalate to Firecrawl only for a concrete retrieval need such as:

```text
richer extraction
multiple full results
site structure discovery
bounded crawling
dynamic interaction
difficult document parsing
developer/tooling evidence
```

Do not use Firecrawl deep-research workflows as a second research methodology. The legal bootstrap already defines the research process.

Do not use Firecrawl's research-paper index as a legal-research database.

Do not run `firecrawl setup defaults`; native Claude web tools remain the normal first path.

## Completion discipline

Before a research-heavy legal stage completes, verify that:

- every material research question has evidence or an explicit bounded gap;
- legally material propositions are traceable to inspected sources;
- jurisdiction and temporal validity are recorded where material;
- stronger authority was preferred where appropriate;
- contrary evidence and meaningful interpretive uncertainty were not silently discarded;
- book-derived methods remain distinguishable from current legal propositions;
- confidentiality constraints were respected;
- the bootstrap stage's actual exit criteria are met.
