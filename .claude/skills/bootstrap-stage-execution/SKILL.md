---
name: bootstrap-stage-execution
description: Shared execution discipline for staged Production Skills bootstraps. Use when a repository bootstrap is executed stage by stage and requires durable outputs, verification, repair, stage-scoped commits, and continuation across an authorised range.
allowed-tools:
  - Read
  - Grep
  - Glob
  - Skill
  - Bash
---

# Bootstrap Stage Execution

This skill standardises execution mechanics. It does not define the domain work. The project's bootstrap specification remains authoritative.

When the current run has a bootstrap execution contract under `docs/research-logs/`, use it for repository, branch, stage-authorisation, commit, and blocker rules. Do not require a private `.claude` configuration surface.

## Stage loop

For each authorised stage:

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
5. Persist the stage's durable outputs in the repository.
6. Re-read the stage requirements and verify the actual outputs against them.
7. Repair failures and re-run affected verification.
8. Commit only that completed stage unless the project contract explicitly defines another boundary.
9. Verify the remote branch points to the intended commit and intended files are present.
10. If the current task or execution contract authorises further stages, continue immediately to the next stage unless a genuine user decision is required.

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

## Verification

Verification should be proportionate to the stage but must check substance, not filenames alone.

If a mandatory requirement fails:

```text
diagnose
→ repair the owning scope
→ re-run affected verification
→ continue
```

Do not weaken acceptance criteria, skip required work, or rewrite validators to make incomplete work pass.

A separate exhaustive conformance table is not mandatory unless the bootstrap specification, execution contract, or risk of the stage requires one. A concise verification record is sufficient when it clearly demonstrates the exit criteria.

## Blockers and user decisions

Stop and ask the user only when progress genuinely depends on a user decision, for example:

- explicit permission or approval is required;
- a supplied source may not be removed, replaced, or demoted without approval;
- materially different valid interpretations require a product/domain choice;
- mandatory evidence or capability is unavailable and cannot be repaired or substituted under the governing specification;
- continuing would reopen accepted scope or decisions without authority.

Do **not** stop merely because:

- a test fails;
- research is incomplete;
- a search query is poor;
- a URL is dead;
- a tool invocation fails;
- implementation has a defect;
- verification finds a failure;
- an alternative supported retrieval or execution path is needed.

Those are execution problems: diagnose, repair, retry, or use an allowed alternative.

## Commit discipline

Default to one commit per completed stage.

Include the stage identifier in the commit message, for example:

```text
stage 4: challenge professional practice
stage 12 P3: extract specialised corpus
```

Do not batch unrelated stages into one commit.

If a stage produces no repository change, do not create an empty commit merely for symmetry; record completion only when the governing process permits a no-change stage.

## Context rule

Reconstruct stage context from repository state:

```text
governing bootstrap specification
+
accepted prior-stage outputs
+
applicable execution contract under docs/research-logs/
```

Do not depend on conversation memory for accepted project state.

## Authorised continuation

If the user has authorised a stage range or the remainder of the bootstrap, continue stage by stage without asking for permission between successfully completed stages.

Stop at the last fully verified stage only when a genuine blocker or user decision prevents the next stage.

## Final audit

When the authorised bootstrap range reaches its final stage, audit the resulting repository against any global acceptance gates in the bootstrap specification. Do not claim maturity, benchmark success, installation success, publication readiness, or completion without the corresponding evidence.
