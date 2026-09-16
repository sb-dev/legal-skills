# Bootstrap Research and Execution Tooling

**Status:** Family-candidate prototype  
**Created:** 14 September 2026  
**Revised:** 16 September 2026  
**Branch:** `feat/bootstrap-3`

## Purpose

This branch prototypes a reusable bootstrap-support architecture for Production Skills projects while retaining legal-specific evidence rules locally.

The original implementation placed research orchestration in a project-specific `legal-bootstrap-research` skill. Comparison with other Production Skills bootstraps showed that most research retrieval, direct-source extraction, and stage-execution mechanics are repeated across domains. Those mechanics are now separated from the legal evidence model.

The legal bootstrap remains authoritative for what each stage must investigate, persist, and prove.

## Architecture

```text
shared bootstrap mechanics
│
├── bootstrap-research
│   └── search / retrieval / challenge / provenance discipline
│
├── direct-source-extraction
│   └── books / documents / reading coverage / reconciliation
│
└── bootstrap-stage-execution
    └── stage loop / verification / repair / commit / continuation
          │
          ▼
legal-skills project profile
│
├── .claude/bootstrap/research-profile.md
│   └── legal authority / jurisdiction / temporal-validity rules
│
├── .claude/bootstrap/execution-contract.md
│   └── branch / authorisation / commit / blocker rules
│
└── governing bootstrap specification
    └── substantive legal stages and exit criteria
```

The three generic skills are temporarily co-located in this branch so the architecture can be exercised. They are candidates for extraction to the central `production-skills` bootstrap tooling after cross-project validation; they are not intended to become legal-domain product skills.

## Shared project-support skills

### `bootstrap-research`

Location:

```text
.claude/skills/bootstrap-research/SKILL.md
```

Owns only reusable research mechanics:

- stage-contract-first evidence questions;
- multiple-query discovery where needed;
- primary/authoritative/first-party source preference as specialised by the local profile;
- inspected-source provenance;
- contradiction and gap research;
- native Claude `WebSearch` / `WebFetch` first;
- Firecrawl escalation for concrete retrieval problems;
- stop conditions tied to actual stage evidence rather than source count.

It deliberately does not encode legal authority rules.

### `direct-source-extraction`

Location:

```text
.claude/skills/direct-source-extraction/SKILL.md
```

Owns the repeated direct-reading pattern used by Seed → Five → Challenge bootstraps:

- source-access register;
- reading coverage;
- stable source locations;
- independently expressed findings;
- applicability and limitations;
- overlap / conflict analysis;
- corpus reconciliation;
- unresolved claims for broader challenge;
- copyright-safe persistence.

It is used when a bootstrap explicitly requires meaningful source examination rather than summaries or model memory.

### `bootstrap-stage-execution`

Location:

```text
.claude/skills/bootstrap-stage-execution/SKILL.md
```

Owns the repeated stage loop:

```text
read stage
→ read accepted dependencies
→ extract requirements
→ execute
→ persist
→ verify
→ repair
→ commit stage
→ verify remote
→ continue when authorised
```

The skill keeps one-stage/one-commit discipline but removes unnecessary process stops. Failed searches, tests, commands, extraction attempts, or implementations are execution problems to repair. The process stops only when a genuine user decision is required.

## Legal project profile

Location:

```text
.claude/bootstrap/research-profile.md
```

This keeps domain-specific evidence rules local:

- legal authority source classes;
- books-versus-current-authority distinction;
- jurisdiction and matter-date capture;
- commencement / amendment / later-treatment / guidance currency;
- confidentiality and privilege constraints;
- legal-specific Stage 2 / 3 / 4 / 5 / 11 routing;
- legal limits on Firecrawl developer/research indexes.

The generic research skill reads this profile rather than containing legal-specific behaviour itself.

## Lean execution contract

Location:

```text
.claude/bootstrap/execution-contract.md
```

The contract is intentionally smaller than the earlier Game / Software execution contracts.

It retains:

```text
bootstrap specification is authoritative
repository state is authoritative
complete substantive stage work
verify before completion
repair failures
one stage per commit
stage number in commit message
never invent evidence
continue through an authorised range
```

It simplifies blocker behaviour:

```text
failed test/search/tool/implementation
→ repair and continue

permission / material ambiguity / unavailable mandatory evidence / reopening accepted scope
→ ask user
```

An exhaustive conformance table is optional unless the stage or risk justifies it; verification itself remains mandatory.

## Native-first research stack

The retrieval architecture remains:

```text
bootstrap stage
      ↓
Claude WebSearch
      ↓
Claude WebFetch
      ↓
coverage / evidence check
      ↓
retrieval problem?
      ├─ no  → continue native research
      └─ yes → Firecrawl escalation
                  ├─ search --scrape
                  ├─ scrape
                  ├─ map
                  ├─ crawl
                  ├─ interact
                  ├─ parse
                  └─ developer index for tooling research
```

Claude remains the researcher. Firecrawl extends retrieval; it does not replace the bootstrap methodology.

## Firecrawl setup

Install outside the repository:

```bash
npm install -g firecrawl-cli
firecrawl login --browser
firecrawl --status
```

For Claude Code, install only the core retrieval capabilities required by this workflow rather than generic deep-research workflows.

Do **not** run:

```bash
firecrawl setup defaults
```

Native Claude web search/fetch remains the primary path.

Do not make this bootstrap depend on `firecrawl-deep-research`. The project's own bootstrap defines the research process.

## Selected Firecrawl roles

| Capability | Role |
| --- | --- |
| search + scrape | richer multi-result retrieval |
| scrape | extraction fallback for a known URL |
| map | authoritative-site structure discovery |
| crawl | bounded multi-page corpus |
| interact | forms, pagination, dynamic sites |
| parse | difficult local documents when external processing is acceptable |
| developer index | implementation/tooling evidence such as docs, READMEs, issues and merged PRs |

Large retrieval artefacts belong under `.firecrawl/`, which remains ignored by Git.

## Legal-specific routing retained locally

The legal profile preserves the important domain split:

```text
foundational books
→ durable method / professional practice

authoritative current sources
→ applicable proposition for a defined jurisdiction and date
```

Stage 3 remains direct-source/local-first. Stage 4 challenges the corpus independently. Stage 5 makes authority and temporal validity explicit. Stage 11 may use developer-index evidence for tools and APIs but never as substantive legal authority.

## Why this is preferable

The previous structure implied that every Production Skills project should create its own research orchestration skill. The revised structure separates:

```text
HOW research/execution works
→ reusable family candidate

WHAT evidence counts in this domain
→ project-local profile

WHAT the stage must produce
→ project bootstrap specification

WHAT this run may execute
→ small execution contract
```

This reduces duplicated skills while keeping domain evidence rules and production intelligence local.

## Extraction status

The generic skills are intentionally marked as family candidates rather than silently moved to `production-skills` from this branch. Central extraction should preserve the Production Skills rule that shared abstractions are promoted only after repeated cross-domain evidence is reviewed.

The current Game Development, Software Engineering, Business Building, and Legal bootstrap patterns provide strong evidence for the abstraction, but the central repository should own the actual promotion step.

## Verification

This branch is internally coherent when:

- `legal-bootstrap-research` no longer exists;
- the three generic support skills are discoverable under `.claude/skills/`;
- legal-specific evidence rules exist only in the local research profile;
- the execution contract is lean and project-specific;
- `.firecrawl/` remains ignored;
- the governing legal bootstrap is unchanged and remains authoritative.
