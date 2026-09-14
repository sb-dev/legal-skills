# Bootstrap Research Tooling

**Status:** Active bootstrap support  
**Date:** 14 September 2026  
**Branch:** `feat/bootstrap-3`

## Purpose

This note defines the web-research tooling used while executing the legal-skills bootstrap stages. It does not replace the bootstrap process, add a second research methodology, or make Firecrawl the default research engine.

The bootstrap remains authoritative for what each stage must investigate, persist and prove. This setup only improves how Claude Code discovers, retrieves and verifies external evidence.

## Decision

Use a native-first, Firecrawl-escalation model:

```text
bootstrap stage contract
        ↓
Claude Code WebSearch
        ↓
Claude Code WebFetch
        ↓
coverage / authority / currency check
        ↓
retrieval problem or material coverage gap?
        ├─ no  → continue native research
        └─ yes → Firecrawl escalation
                    ├─ search --scrape
                    ├─ scrape
                    ├─ map
                    ├─ crawl
                    ├─ interact
                    ├─ parse
                    └─ developer index (Stage 11/tooling work)
        ↓
challenge / reconcile
        ↓
persist stage evidence
        ↓
check stage exit criteria
```

Claude Code remains the researcher. Firecrawl extends retrieval when native tools are inadequate or materially less efficient.

## Project skill

The project-specific procedure lives at:

```text
.claude/skills/legal-bootstrap-research/SKILL.md
```

Claude Code project skills are discovered automatically from `.claude/skills/`. The skill encodes:

- stage-contract-first research;
- multiple-query evidence discovery;
- primary/authoritative source preference;
- native `WebSearch` / `WebFetch` as the default path;
- explicit Firecrawl escalation triggers;
- legal source provenance and temporal-validity capture;
- Stage 2, 3, 4, 5 and 11 routing rules;
- stop conditions tied to stage exit criteria rather than source count.

It is intentionally a bootstrap research skill, not a generic `deep-research` skill.

## Firecrawl setup

Install the CLI outside the repository:

```bash
npm install -g firecrawl-cli
firecrawl login --browser
firecrawl --status
```

For Claude Code, install only the core retrieval skills needed by this workflow rather than Firecrawl workflow skills:

```bash
npx skills add firecrawl/skills \
  --global \
  --agent claude-code \
  --skill \
    firecrawl-search \
    firecrawl-scrape \
    firecrawl-map \
    firecrawl-crawl \
    firecrawl-interact \
    firecrawl-parse \
    firecrawl-developer-index \
  --yes
```

The project skill does not require Firecrawl to be the default provider. Do **not** run:

```bash
firecrawl setup defaults
```

That mode is designed to route supported agents away from native web search/fetch. This bootstrap deliberately preserves Claude Code's native web tools as the first path.

Do not install or depend on Firecrawl workflow skills such as `firecrawl-deep-research` for this bootstrap. The legal bootstrap already defines the governing research process.

## Selected Firecrawl capabilities

### `firecrawl-search`

Use when native discovery needs richer retrieval, especially when several results need full-page content in one operation. Save large results under `.firecrawl/` rather than streaming them into context.

### `firecrawl-scrape`

Use as an extraction fallback for a known URL when `WebFetch` is incomplete or unsuitable.

### `firecrawl-map`

Use to discover the structure of an authoritative site before selecting the relevant guidance, registry, documentation or policy pages.

### `firecrawl-crawl`

Use only for a bounded authoritative site area when several related pages must be examined together. Avoid broad indiscriminate crawling.

### `firecrawl-interact`

Use for sites that require clicks, forms, pagination or other dynamic interaction. It is not the default way to fetch ordinary pages.

### `firecrawl-parse`

Use for difficult local PDF/DOCX/XLSX extraction when Claude Code's local document inspection is inadequate and external processing is acceptable. This is a fallback, not the default path for the five-book corpus.

### `firecrawl-developer-index`

Use primarily in Stage 11 for developer/tooling questions covering GitHub issues, merged pull requests, READMEs and documentation. It is not a legal-authority source.

## Deliberately excluded

### Firecrawl deep-research workflows

Excluded because they would introduce a second orchestration methodology alongside the legal bootstrap's own staged research model.

### Firecrawl research-paper index

Excluded from the legal research path. Its indexed literature is oriented toward biomedical/life-science literature and arXiv, not authoritative legal research.

### Firecrawl build skills

Excluded because the bootstrap is using Firecrawl as an operator tool, not integrating Firecrawl into the legal-skills product code.

### Firecrawl as default web provider

Excluded because native Claude Code search/fetch is adequate for ordinary discovery and straightforward authoritative pages. Firecrawl is an escalation path.

## Stage routing

| Bootstrap stage | Research-tooling expectation |
| --- | --- |
| Stage 2 — corpus selection | Native web search for candidate/edition/access reconnaissance; Firecrawl only if source discovery is difficult |
| Stage 3 — corpus extraction | Direct local book examination first; `firecrawl parse` only as a justified fallback |
| Stage 4 — professional-practice challenge | Multiple independent native searches; Firecrawl search/map/crawl when coverage or site structure warrants it |
| Stage 5 — authority/temporal model | Native search/fetch against authoritative sources; Firecrawl extraction only when necessary |
| Stage 11 — tools/databases/registries | Native search + official docs; developer index for implementation/API/GitHub evidence |

Other stages use the same routing rule whenever they require current external evidence.

## Evidence discipline

The retrieval stack must preserve the legal bootstrap's distinction:

```text
foundational books
→ durable method / professional practice

authoritative current sources
→ applicable legal proposition for a defined jurisdiction and date
```

For material external findings record, as applicable:

```text
research question
jurisdiction / territory
matter or validity date
proposition
source / authority type
stable URL or identifier
publication / judgment / made date
effective / commencement / update date
retrieved-at date
section / paragraph / page / location
applicability
limitations / contrary evidence
project implication
```

Search snippets are discovery aids, not evidence. Important claims must be based on inspected sources.

## Context and cost control

Firecrawl outputs can be large. Save them under `.firecrawl/` and inspect them incrementally. The repository ignores that directory.

Prefer the cheapest adequate retrieval operation:

```text
WebSearch before Firecrawl search
WebFetch before Firecrawl scrape
scrape before map/crawl
map before broad crawl
local Read before external document parsing
```

Escalation should solve a specific retrieval problem, not merely add more tools.

## Confidentiality boundary

Do not upload privileged, confidential, unpublished, personal or commercially sensitive material to Firecrawl without explicit approval. For supplied books and project-local documents, prefer local inspection. Apply the same care to any external web or AI service when matter confidentiality is material.

## Verification

A working local setup should satisfy:

```bash
firecrawl --status
```

and a small disposable extraction check may be used when needed:

```bash
mkdir -p .firecrawl
firecrawl scrape "https://firecrawl.dev" -o .firecrawl/install-check.md
```

Successful Firecrawl setup is useful but is not a bootstrap-stage completion criterion by itself. If Firecrawl is unavailable, continue with native Claude Code tools unless the stage genuinely depends on a retrieval capability that cannot otherwise be completed.
