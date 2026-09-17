# Bootstrap Research and Execution Tooling

**Status:** Family-candidate prototype  
**Created:** 14 September 2026  
**Revised:** 17 September 2026  
**Branch:** `feat/bootstrap-3`

## Purpose

This branch prototypes a reusable bootstrap runtime for Production Skills projects. The operator should not need to restate stage numbers, ranges, research instructions, verification rules, or continuation prompts on every run.

The governing bootstrap specification remains authoritative for domain work and evidence requirements.

## Operator interface

The normal interface is one command:

```text
/bootstrap
```

With no arguments it means:

```text
inspect repository state
→ determine next incomplete stage
→ execute it completely
→ verify and repair
→ commit and push that stage
→ continue with the next incomplete stage
→ stop only for a genuine user decision
→ run the final audit after the last stage
```

The user does not need to repeat prompts such as `complete Stage 1`, `continue to Stage 4`, or `continue the next stage`.

## Architecture

```text
/bootstrap                       # public operator command
    ↓
bootstrap-stage-execution        # internal stage runner
    ├── bootstrap-research       # external research/retrieval
    └── direct-source-extraction # direct book/document examination
          ↓
governing bootstrap specification
+ accepted repository research logs
+ bootstrap execution contract
```

Claude-specific project files are actual skills under `.claude/skills/`. There is no `.claude/bootstrap/` configuration convention.

## `bootstrap`

Location:

```text
.claude/skills/bootstrap/SKILL.md
```

Owns orchestration only:

- locate the current execution contract;
- read the governing bootstrap;
- verify repository/branch state without discarding local work;
- reconstruct accepted progress from committed repository evidence;
- determine the next incomplete stage;
- authorise the remaining bootstrap by default;
- delegate each stage to `bootstrap-stage-execution`;
- continue automatically after successful stage completion;
- run the final/global audit.

## Internal support skills

### `bootstrap-stage-execution`

Executes one stage completely:

```text
read stage
→ read dependencies
→ execute
→ persist
→ verify
→ repair
→ commit
→ push
→ verify remote
→ return to /bootstrap
```

### `bootstrap-research`

Provides reusable research mechanics:

- derive evidence questions from the current stage;
- use Claude `WebSearch` / `WebFetch` first;
- inspect actual sources rather than search snippets;
- research contradictions and material gaps;
- preserve provenance and currency;
- escalate to Firecrawl only for concrete retrieval problems.

Domain-specific evidence rules come from the governing bootstrap specification.

### `direct-source-extraction`

Handles stages that require meaningful examination of books, standards, papers, or supplied documents rather than summaries or model memory. It records source access, reading coverage, traceable findings, applicability, conflicts, reconciliation, and unresolved claims.

## Execution contract

Location:

```text
docs/research-logs/2026-09-17-bootstrap-execution-contract.md
```

The contract now defines `/bootstrap` as the operator command and makes its default authorisation explicit:

```text
/bootstrap
→ next incomplete stage through final stage
```

Only an explicit user instruction narrows that range.

The contract retains:

```text
repository state is authoritative
one stage = one commit
stage number in commit message
verify before completion
repair before escalation
push + verify remote before continuation
never invent evidence
```

A failed search, test, command, extraction, implementation, or verification step is an execution problem to repair, not a reason to ask whether to continue.

## Research stack

Default retrieval remains native-first:

```text
Claude WebSearch
→ Claude WebFetch
→ evidence check
→ Firecrawl only when needed
```

Firecrawl roles:

| Capability | Role |
| --- | --- |
| search + scrape | retrieve several full results |
| scrape | fallback extraction for a known URL |
| map | discover site structure |
| crawl | bounded multi-page corpus |
| interact | forms, pagination, dynamic sites |
| parse | difficult local documents when external processing is acceptable |
| developer index | docs, READMEs, issues and merged PRs for tooling research |

Do not run `firecrawl setup defaults`; native Claude search/fetch remains the primary path. Do not add a generic deep-research workflow because the project bootstrap already defines the research process.

Large Firecrawl artefacts belong under `.firecrawl/`, which remains ignored by Git.

## Legal-specific behaviour

Legal-specific rules remain in the Legal Skills bootstrap, including:

- jurisdiction before rule application;
- authority before assertion;
- temporal currency as part of correctness;
- books inform method while current authority governs legal propositions;
- confidentiality and privilege constraints;
- direct-source examination of the five-book corpus.

The generic skills read those requirements from the bootstrap rather than duplicating them in Claude configuration.

## Family extraction candidate

The reusable candidate is now four skills with one public surface:

```text
public:
  bootstrap

internal:
  bootstrap-stage-execution
  bootstrap-research
  direct-source-extraction
```

The implementation is temporarily hosted in `legal-skills` for validation. If it proves useful across Legal, Software Engineering, Game Development, Business Building, and other Production Skills projects, the central `production-skills` repository should own the shared implementation.

## Verification

This branch is coherent when:

- `/bootstrap` is the only command the operator normally needs;
- `.claude/skills/bootstrap/SKILL.md` exists;
- the three support skills remain available internally;
- the execution contract authorises remaining stages by default;
- each stage is committed and pushed separately;
- domain evidence rules come from the governing bootstrap;
- `.claude/bootstrap/` and `legal-bootstrap-research` do not exist;
- `.firecrawl/` remains ignored.
