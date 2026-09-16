---
name: direct-source-extraction
description: Shared direct-source examination and reconciliation procedure for bootstrap stages that require meaningful reading of supplied books, papers, standards, documents, or other source material. Use when summaries, bibliographies, publisher descriptions, or model memory are explicitly insufficient evidence.
allowed-tools:
  - Read
  - Grep
  - Glob
  - Bash
---

# Direct Source Extraction

Use this skill when a bootstrap stage requires direct examination of source material rather than source discovery alone.

The project bootstrap defines the required corpus, source permissions, minimum coverage, and exit criteria. This skill standardises how examination and reconciliation are recorded.

## Access before extraction

For each required source record:

```text
title / identifier
edition / version / publication year where relevant
provided or selected origin
source location or non-public identifier
access state
intended contribution
material actually examined
reading limitations
```

Useful access states are:

```text
full text available
relevant excerpts available
secondary material only
unavailable
```

Access is not reading. Do not mark a source examined because a file exists or because a table of contents, abstract, review, summary, or publisher description is available.

If the bootstrap requires direct examination and adequate source access is unavailable, record the gap as a blocker rather than inferring findings.

## Examine material meaningfully

Read the portions required to assess the source's intended contribution. Do not extract only famous passages or search hits if doing so would miss the source's argument, conditions, limitations, or counterexamples.

For each material finding capture:

| Field | Required content |
| --- | --- |
| Source location | Book/document, edition/version, chapter/section/page or other stable location actually examined |
| Problem / concept | Independently expressed principle, method, claim, model, or heuristic |
| Applicability | Context, assumptions, prerequisites, scope, and limitations |
| Production effect | Decision, workflow, artefact, behaviour, or responsibility affected |
| Evaluation | Evidence, metrics, checks, or acceptance implications |
| Failure / misuse | Failure conditions, misuse risks, and repair implications |
| Relationships | Support, overlap, tension, contradiction, or dependency with other sources |
| Disposition | Retain, merge, adapt, qualify, reject, or research further |

Use the project's domain terminology rather than forcing a universal schema beyond these evidence fields.

## Reconcile the corpus

After per-source extraction, analyse across sources:

```text
reinforcing findings
overlapping methods
competing assumptions
context-dependent alternatives
contradictions
important topics absent from the corpus
claims requiring broader professional / empirical / current-practice challenge
```

Repeated claims across several sources do not automatically constitute independent corroboration.

Do not force every selected source to contribute a core rule. A source may have a narrow contribution, be superseded by stronger evidence, or remain useful only as a challenge perspective.

## Copyright and publication boundary

Persist independently expressed synthesis and concise traceability, not substantial copied text, reconstructed chapters, proprietary examples, or private source material.

Do not commit supplied books or private source locations unless the user explicitly intends those files or locations to be published.

## Handoff to broader research

Produce explicit unresolved claims and gaps for the later challenge stage. Direct-source extraction establishes what the corpus contributes; it does not prove that the corpus is complete or current.

## Completion check

Before marking a direct-source stage complete, verify that:

- every required source has been meaningfully examined for its intended contribution;
- reading coverage is recorded honestly;
- material findings have stable source locations;
- synthesis is independently expressed;
- applicability and limitations are preserved;
- overlaps and conflicts are reconciled rather than hidden;
- unresolved claims and missing coverage are explicit;
- inadequate access has not been disguised with summaries or model memory;
- publication remains copyright-safe and does not expose private source material.
