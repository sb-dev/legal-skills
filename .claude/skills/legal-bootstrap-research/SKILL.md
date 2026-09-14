---
name: legal-bootstrap-research
description: Evidence-first web research procedure for executing legal-skills bootstrap stages. Use whenever a bootstrap stage requires external research, authoritative-source verification, professional-practice challenge, current legal or regulatory evidence, registry/database research, or tooling landscape research. Use Claude Code WebSearch/WebFetch first and escalate to Firecrawl only when richer extraction, site discovery, bounded crawling, document parsing, dynamic interaction, or developer-index search is needed.
allowed-tools:
  - WebSearch
  - WebFetch
  - Read
  - Grep
  - Glob
  - Bash(firecrawl *)
  - Bash(npx firecrawl-cli *)
---

# Legal Bootstrap Research

Use this skill to execute the research requirements already defined by the legal-skills bootstrap process. It is a retrieval and evidence-discipline layer, not a replacement research methodology.

## Non-goals

Do not:

- replace the bootstrap stage instructions or exit criteria;
- invoke a generic deep-research workflow merely because a stage requires research;
- use Firecrawl as the default web provider;
- use Firecrawl's research-paper index as a legal-research database;
- treat search snippets, summaries, LLM output, or secondary commentary as authority for a material legal proposition;
- send privileged, confidential, unpublished, personal, or commercially sensitive material to an external retrieval service without explicit approval.

## Start from the stage contract

Before researching:

1. Read the current bootstrap stage in `docs/research-logs/2026-09-08-legal-skills-new-project-bootstrap-process.md`.
2. Read the prior stage logs that the current stage depends on.
3. Extract the stage's research questions, required durable outputs, and exit criteria.
4. Turn those requirements into distinct evidence questions before searching.

The stage exit criteria determine when research is sufficient. Finding several sources does not.

## Default research loop

For each evidence question:

1. Search from more than one genuinely different angle with Claude Code `WebSearch`.
2. Prefer primary or authoritative sources appropriate to the proposition being established.
3. Use `WebFetch` to inspect promising sources; do not rely on search-result snippets as evidence.
4. Record material source provenance and the proposition it supports.
5. Identify contradictions, missing responsibilities, jurisdictional differences, temporal changes, or weakly supported claims.
6. Run targeted follow-up searches for those gaps.
7. Stop only when the evidence required by the stage exit criteria is covered or the remaining uncertainty is explicitly bounded.
8. Persist the detailed evidence and decisions in the stage research log before dependent work proceeds.

## Source selection

Prefer the strongest source for the proposition, recognising that authority varies by jurisdiction and task.

Typical priority classes include:

- enacted legislation and official legislative repositories;
- judgments and official court or tribunal sources;
- regulator rules, decisions, notices and guidance;
- official registries and filing systems;
- treaties and official supranational material;
- government guidance and consultations;
- recognised professional-body material where it is evidence of professional practice rather than binding law;
- official product, API, database and tool documentation for tooling claims;
- high-quality practitioner or academic commentary for interpretation, context, disagreement and practice discovery.

Secondary sources may identify issues or authorities. They do not replace appropriate current authority for a material substantive-law proposition.

## Native-first tool routing

Use Claude Code's built-in web tools first.

| Need | Default tool |
| --- | --- |
| Discover current sources | `WebSearch` |
| Read straightforward authoritative HTML | `WebFetch` |
| Challenge coverage from another query angle | another `WebSearch` |
| Inspect local supplied books or documents | `Read`, `Grep`, `Glob` |

Escalate to Firecrawl only when it adds a concrete retrieval capability.

| Retrieval problem | Firecrawl escalation |
| --- | --- |
| Search plus several full-page results are needed | `firecrawl search ... --scrape` |
| `WebFetch` cannot extract a known page adequately | `firecrawl scrape` |
| Need to discover an authoritative site's structure | `firecrawl map` |
| Need a bounded corpus from part of a site | `firecrawl crawl` |
| A page requires clicks, forms, pagination or dynamic interaction | `firecrawl interact` |
| A difficult local PDF/DOCX/XLSX needs clean Markdown | `firecrawl parse` |
| Stage 11 needs GitHub issues, merged PRs, READMEs or developer docs | `firecrawl developer` / developer category search |

Do not run `firecrawl setup defaults`: the project deliberately retains Claude Code's native `WebSearch` and `WebFetch` as the default path.

## Firecrawl operating rules

Keep large retrieval outputs out of the main context window.

```bash
mkdir -p .firecrawl

firecrawl search "<query>" -o .firecrawl/search.json --json
firecrawl search "<query>" --scrape -o .firecrawl/search-scraped.json --json
firecrawl scrape "<url>" -o .firecrawl/source.md
firecrawl map "<url>" -o .firecrawl/map.json --json
firecrawl crawl "<url>" -o .firecrawl/crawl.json --json
firecrawl parse "<local-file>" -o .firecrawl/document.md
firecrawl developer "<developer/tooling query>" -o .firecrawl/developer.json --json
```

Read saved results incrementally with `Read`/`Grep`; do not dump large retrieval files into conversation context.

Check `firecrawl --help` or the relevant subcommand help when syntax has changed instead of guessing.

## Legal evidence record

For every material proposition preserve enough information to audit it later. Capture as applicable:

```text
research question
jurisdiction / territory
matter date or temporal context
proposition supported
authority / source type
source title
source URL or stable identifier
publication / judgment / made date
effective / commencement / update date when relevant
retrieved-at date
relevant section / paragraph / page / stable location
applicability
limitations / contrary authority
confidence or unresolved uncertainty
dependent conclusion / project implication
```

A conclusion must not become more certain than its facts, authority, jurisdiction or temporal analysis justify.

## Stage-specific routing

### Stage 2 — five-book corpus selection

Use web research only for enough reconnaissance to choose the complementary five-book corpus and verify editions, scope, source access and coverage. Do not turn selection into the direct-extraction stage.

### Stage 3 — five-book extraction

Directly examine the supplied books. Prefer local `Read`/`Grep` against the source files. Use `firecrawl parse` only when native local-document inspection is inadequate and external processing is acceptable. Publisher descriptions, reviews and web summaries do not satisfy direct-source extraction.

### Stage 4 — professional-practice challenge

Search independently across the legal-production boundary, not merely for confirmation of book-derived methods. Use multiple query angles across the professional practices named by the bootstrap and actively seek contradictory or omitted responsibilities.

### Stage 5 — jurisdiction, authority and temporal validity

Prefer authoritative legal sources. Preserve dates and authority status explicitly. Search for amendments, commencement, later treatment and current regulator guidance where material.

### Stage 11 — AI skills, databases, registries and tools

Use normal web search for the landscape and official product documentation. Use Firecrawl's developer index for implementation/documentation questions, GitHub issues, merged PRs and API behaviour. Do not confuse developer-index evidence with substantive legal authority.

## Completion check

Before declaring a research-heavy stage complete, verify:

- every stage research question has evidence or an explicit bounded gap;
- material claims can be traced to inspected sources;
- primary/authoritative sources were preferred where appropriate;
- jurisdiction and temporal validity are recorded where material;
- contradictory evidence was investigated rather than silently discarded;
- book-derived claims and current legal propositions remain distinguishable;
- Firecrawl was used only where native tools were inadequate or materially less efficient;
- detailed findings are persisted in the repository research log;
- the stage's stated exit criteria are actually met.
