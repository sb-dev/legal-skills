# Bootstrap Research and Execution Tooling

**Status:** Family-candidate prototype  
**Created:** 14 September 2026  
**Revised:** 17 September 2026  
**Branch:** `feat/bootstrap-3`

## Purpose

This branch prototypes reusable bootstrap-support skills for Production Skills projects while keeping domain-specific research rules in each project's governing bootstrap specification.

The original implementation placed research orchestration in a project-specific `legal-bootstrap-research` skill, then introduced a `.claude/bootstrap/` configuration layer. Cross-project comparison showed both were unnecessary: the reusable mechanics belong in shared skills, while Legal Skills already defines its authority, jurisdiction, temporal-validity, confidentiality, and direct-source rules in the bootstrap specification.

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
project repository
│
├── governing bootstrap specification
│   └── domain method / evidence rules / stage requirements / exit criteria
│
├── bootstrap execution contract under docs/research-logs/
│   └── branch / authorisation / commit / blocker rules
│
└── stage research logs
    └── durable evidence / decisions / verification
```

There is no `.claude/bootstrap/` convention. Claude-specific project files are limited to actual skills under `.claude/skills/`.

The three generic skills are temporarily co-located in this branch so the architecture can be exercised. They are candidates for extraction to the central `production-skills` bootstrap tooling after cross-project validation; they are not intended to become Legal Skills product skills.

## Shared project-support skills

### `bootstrap-research`

Location:

```text
.claude/skills/bootstrap-research/SKILL.md
```

Owns reusable research mechanics:

- stage-first evidence questions;
- multiple-query discovery where needed;
- inspected-source provenance;
- contradiction and gap research;
- native Claude `WebSearch` / `WebFetch` first;
- Firecrawl escalation for concrete retrieval problems;
- stop conditions tied to stage evidence rather than source count.

It derives domain-specific evidence requirements directly from the governing bootstrap specification rather than loading a duplicate project research profile.

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

## Domain-specific evidence rules

No separate `.claude` research profile is required.

For Legal Skills, the governing bootstrap already defines the relevant rules, including:

- authority before assertion;
- jurisdiction before rule application;
- temporal currency as part of correctness;
- books inform method while current authority governs legal propositions;
- confidentiality and privilege as design constraints;
- direct-source examination for the five-book corpus;
- authoritative-source challenge and tooling research stages.

The generic research skill must read those rules from the bootstrap rather than copying them into a second configuration file.

This same pattern should apply to other Production Skills projects: Game Development keeps player-evidence rules in its bootstrap, Software Engineering keeps repository/verification rules in its bootstrap, Business Building keeps empirical/professional-practice rules in its bootstrap, and so on.

## Lean execution contract

Location:

```text
docs/research-logs/2026-09-17-bootstrap-execution-contract.md
```

The execution contract contains run-specific mechanics only:

```text
repository / branch
governing bootstrap
accepted-state reconstruction
stage authorisation
one-stage / one-commit rule
repair-before-escalation behaviour
genuine-user-decision blockers
remote verification
final audit
```

It does not duplicate domain research policy.

The contract intentionally simplifies the earlier Game / Software execution contracts:

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

## Legal routing from the governing bootstrap

The Legal Skills bootstrap preserves the important distinction:

```text
foundational books
→ durable method / professional practice

authoritative current sources
→ applicable proposition for a defined jurisdiction and date
```

Stage 3 remains direct-source/local-first. Stage 4 challenges the corpus independently. Stage 5 makes authority and temporal validity explicit. Stage 11 may use developer/tooling evidence for tools and APIs but never as substantive legal authority.

These are bootstrap rules, not Claude configuration.

## Why this is preferable

The corrected structure separates:

```text
HOW research/execution works
→ reusable family candidate skills

WHAT evidence counts in this domain
→ governing project bootstrap

WHAT the stage must produce
→ governing project bootstrap

WHAT this run may execute
→ research-log execution contract
```

This avoids project-specific research skills, duplicate research profiles, and non-standard `.claude` configuration folders.

## Extraction status

The generic skills remain family candidates rather than being silently moved to `production-skills` from this branch. Central extraction should preserve the Production Skills rule that shared abstractions are promoted only after repeated cross-domain evidence is reviewed.

The current Game Development, Software Engineering, Business Building, and Legal bootstrap patterns provide strong evidence for the abstraction, but the central repository should own the actual promotion step.

## Verification

This branch is internally coherent when:

- `.claude/bootstrap/` does not exist;
- `legal-bootstrap-research` does not exist;
- the three generic support skills are discoverable under `.claude/skills/`;
- domain-specific legal evidence rules come from the governing bootstrap specification;
- the execution contract lives under `docs/research-logs/`;
- `.firecrawl/` remains ignored;
- the governing legal bootstrap remains authoritative.
