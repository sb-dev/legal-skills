---
name: bootstrap-research
description: Shared evidence-first research procedure for Production Skills bootstrap stages. Use when a stage requires external research, current verification, professional-practice challenge, capability-landscape research, or other source-based investigation. The project bootstrap and local research profile define what evidence is required; this skill defines how to acquire and qualify it.
allowed-tools:
  - WebSearch
  - WebFetch
  - Read
  - Grep
  - Glob
  - Skill
  - Bash(firecrawl *)
  - Bash(npx firecrawl-cli *)
---

# Bootstrap Research

This is a reusable bootstrap-support skill. It does not define a domain methodology and must not replace a project's bootstrap specification, stage requirements, exit criteria, or domain-specific evidence rules.

## Inputs

Before researching, read:

1. the current stage in the project's authoritative bootstrap specification;
2. accepted prior-stage outputs that the stage depends on;
3. `.claude/bootstrap/research-profile.md` when present;
4. `.claude/bootstrap/execution-contract.md` when present.

The bootstrap says **what must be proved**. The research profile says **what counts as strong evidence in this domain**. This skill says **how to obtain and challenge that evidence**.

## Research loop

For each substantive stage:

1. Convert stage requirements and exit criteria into distinct evidence questions.
2. Search each material question from more than one genuinely different angle when one query is unlikely to establish adequate coverage.
3. Prefer the source classes defined by the local research profile; otherwise prefer primary, authoritative, official, empirical, or first-party sources appropriate to the claim.
4. Inspect the source itself. Search snippets, model memory, summaries, and generated prose are discovery aids, not evidence.
5. Capture enough provenance to trace every material finding to an inspected source.
6. Look for missing responsibilities, counterexamples, contrary evidence, temporal changes, scope limits, and implementation constraints.
7. Run targeted follow-up research for material gaps rather than broad repetitive searches.
8. Keep unresolved or weakly supported claims explicit instead of promoting them into unconditional project rules.
9. Persist detailed findings in the stage's durable research output.
10. Stop when the stage's evidence requirements and exit criteria are satisfied or remaining uncertainty is explicitly bounded — not when an arbitrary source count is reached.

## Native-first retrieval

Use Claude Code's native tools first:

| Need | Default |
| --- | --- |
| Discover current sources | `WebSearch` |
| Read a straightforward web source | `WebFetch` |
| Inspect local supplied material | `Read`, `Grep`, `Glob` |
| Challenge coverage | another targeted `WebSearch` |

Escalate to Firecrawl only when it solves a concrete retrieval problem:

| Retrieval problem | Escalation |
| --- | --- |
| Need several full search results together | `firecrawl search ... --scrape` |
| Native fetch cannot extract a known page adequately | `firecrawl scrape` |
| Need to discover an authoritative site's structure | `firecrawl map` |
| Need a bounded multi-page corpus | `firecrawl crawl` |
| Dynamic interaction, forms, pagination, or click paths are required | `firecrawl interact` |
| Difficult local document needs clean extraction and external processing is allowed | `firecrawl parse` |
| Tooling research needs READMEs, docs, GitHub issues, or merged PRs | Firecrawl developer-index capability |

Do not run `firecrawl setup defaults`; native Claude web search remains the normal first path.

Save large Firecrawl results under `.firecrawl/` and inspect them incrementally rather than flooding the main context.

Check the installed CLI help when command syntax differs instead of guessing.

## Evidence record

For each material finding capture, as applicable:

```text
research question
claim / proposition / practice
source type
source title
stable URL or identifier
publication / effective / update date
retrieved-at date
section / paragraph / page / stable location
scope / applicability
limitations / contrary evidence
evidential standing
project implication
```

The local research profile may require additional domain fields.

## Direct-source stages

When a stage explicitly requires direct examination of supplied books, papers, standards, files, or other source material, use the `direct-source-extraction` skill rather than treating web summaries as a substitute.

Source access is not source examination.

## Cost and context discipline

Use the cheapest adequate operation:

```text
WebSearch before Firecrawl search
WebFetch before Firecrawl scrape
scrape before site-wide operations
map before broad crawl
local Read before external document parsing
```

Do not add providers merely to create redundant coverage. Cross-provider verification is justified only when a material gap, contradiction, or discovery-risk remains.

## Completion check

Before research-dependent stage completion, verify that:

- each material research question has evidence or an explicit bounded gap;
- material findings are traceable to inspected sources;
- the local domain evidence hierarchy was followed;
- contrary evidence and material limitations were investigated;
- change-sensitive claims were checked for currency where relevant;
- direct-source requirements were actually satisfied where required;
- detailed evidence is persisted in the repository;
- the stage's actual exit criteria are met.
