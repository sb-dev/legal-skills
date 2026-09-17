---
name: bootstrap-stage-execution
description: Internal stage-execution capability used by /bootstrap. It performs one bootstrap stage completely, persists evidence, verifies and repairs the result, commits and pushes the stage, and returns control for automatic continuation.
allowed-tools:
  - Read
  - Grep
  - Glob
  - Skill
  - Bash
---

# Bootstrap Stage Execution

This is an internal support capability for `/bootstrap`. It standardises execution mechanics; the project's bootstrap specification remains authoritative for domain work, required outputs, and exit criteria.

Read the applicable bootstrap execution contract under `docs/research-logs/` for repository, branch, commit, blocker, and remote-verification rules.

## Stage loop

For the current stage:

1. Read the complete stage in the governing bootstrap specification.
2. Read accepted prior-stage outputs that the stage depends on.
3. Derive a compact working checklist covering:
   - required inputs and prerequisites;
   - substantive research / design / implementation / evaluation;
   - required outputs;
   - exact counts or distributions where specified;
   - required execution, tests, comparisons, or installation evidence;
   - exit criteria.
4. Perform the complete substantive work.
5. Use `bootstrap-research` for external evidence work and `direct-source-extraction` when direct examination is required.
6. Persist the stage's durable outputs in the repository.
7. Re-read the original stage and verify actual outputs against every mandatory requirement and exit criterion.
8. Repair failures and re-run affected verification.
9. Commit only the completed stage, using the stage identifier in the commit message.
10. Push the commit to the working branch and verify that the remote branch points to the intended commit and contains the intended files.
11. Return control to `/bootstrap`, which continues with the next incomplete stage automatically.

Do not optimise for reaching the final stage. Complete the current stage properly first.

## Evidence rule

Never substitute:

```text
plan for execution
summary for required research
bibliography for direct-source examination
script for required script execution
prompt for required generated output
file existence for substantive validation
single favourable run for a required benchmark/comparison
model memory for required source evidence
```

Never invent research findings, test passes, benchmark results, installation results, telemetry, observations, tool executions, or repository state.

Synthetic fixtures must remain explicitly synthetic.

## Verification and repair

Verification must check substance, not filenames alone.

If a mandatory requirement fails:

```text
diagnose
→ repair the owning scope
→ re-run affected verification
→ continue
```

Do not weaken acceptance criteria, skip required work, or change validators merely to make incomplete work pass.

A separate exhaustive conformance table is not mandatory unless the bootstrap specification, execution contract, or stage risk requires one. Persist enough verification evidence to justify completion.

## Genuine blockers

Stop and return a user-decision blocker only when progress actually depends on the user, for example:

- explicit permission or approval is required;
- a supplied source may not be removed, replaced, or demoted without approval;
- materially different valid interpretations require a product/domain choice;
- mandatory evidence or capability is unavailable and cannot be repaired or substituted under the governing specification;
- continuing would reopen accepted scope or decisions without authority;
- proceeding would require discarding or overwriting unrelated local work.

Do not stop merely because a test, search, URL, tool invocation, extraction attempt, implementation, or verification step failed. Those are execution problems: diagnose, repair, retry, or use an allowed alternative.

## Commit discipline

Default to one commit per completed stage. Include the stage identifier, for example:

```text
stage 4: challenge professional practice
stage 12 P3: extract specialised corpus
```

Do not batch unrelated stages into one commit.

## Context rule

Reconstruct stage context from:

```text
governing bootstrap specification
+
accepted prior-stage outputs
+
applicable execution contract under docs/research-logs/
```

Do not depend on conversation memory for accepted project state.
