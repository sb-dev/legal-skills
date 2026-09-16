# Legal Skills Bootstrap Execution Contract

**Repository:** `sb-dev/legal-skills`  
**Working branch:** `feat/bootstrap-3`  
**Governing bootstrap:** `docs/research-logs/2026-09-08-legal-skills-new-project-bootstrap-process.md`

This contract defines execution mechanics only. The bootstrap specification remains authoritative for substantive requirements and exit criteria.

## Current-stage rule

Determine accepted progress from repository state and persisted research logs on the working branch. Do not infer accepted stage completion from conversation memory.

Execute only the stage or stage range authorised by the current user instruction. If the user authorises a range or the remainder of the bootstrap, continue automatically stage by stage until that range is complete or a genuine user decision is required.

## Stage execution

For each authorised stage:

```text
read complete stage
→ read accepted dependencies
→ extract requirements and exit criteria
→ perform the substantive work
→ persist required outputs
→ verify actual outputs
→ repair failures
→ commit only that stage
→ verify remote commit
→ continue when authorised
```

Use the shared project support skills where applicable:

```text
bootstrap-stage-execution
bootstrap-research
direct-source-extraction
```

and apply `.claude/bootstrap/research-profile.md` for legal evidence rules.

## Non-negotiable evidence rules

Do not:

- substitute a summary for required substantive research;
- substitute a bibliography, publisher description, secondary summary, or model memory for required direct-source examination;
- describe expected execution when actual execution is required;
- claim tests, benchmarks, installations, comparisons, searches, or tool runs that did not occur;
- weaken a bootstrap exit criterion because the work is difficult;
- silently replace, remove, or demote a user-provided source where permission is required;
- batch several independently defined stages into one commit.

## Repair before escalation

A failed search, dead URL, failed command, test failure, extraction problem, or implementation defect is not by itself a reason to stop.

Use the smallest responsible repair or an allowed alternative path and continue.

## Stop only for genuine user decisions

Stop and ask when progress actually depends on the user, including:

- explicit permission or approval required by the bootstrap;
- supplied-source substitution/removal/demotion requiring approval;
- materially different valid interpretations that change project scope or accepted behaviour;
- unavailable mandatory evidence or capability that cannot be repaired or substituted within the bootstrap rules;
- a contradiction that would require reopening accepted prior work without authority.

Do not stop merely because work is difficult, a first attempt failed, or verification found defects.

## Verification

Before declaring a stage complete:

1. re-read its bootstrap section;
2. inspect the actual persisted outputs;
3. verify exact counts/distributions where specified;
4. run required tests, executions, comparisons, or installation checks;
5. repair every mandatory failure;
6. record enough verification evidence in the stage output to make completion auditable.

A separate exhaustive PASS/FAIL table is optional unless the stage or risk profile benefits from it.

## Commit convention

Use one commit per completed stage and include the stage identifier in the message, for example:

```text
stage 4: challenge professional legal practice
stage 12 P3: extract privacy pack corpus
```

Do not create an empty commit solely to mark progress.

## Completion reporting

After each completed stage, report compactly:

```text
Stage: <identifier>
Status: COMPLETE
Commit: <full SHA>
Verification: PASS
Blockers: none
```

When an authorised range continues, proceed to the next stage rather than waiting for another approval unless a genuine user decision is required.

## Final audit

At the end of the authorised bootstrap range, audit the repository against the bootstrap's global acceptance requirements that are applicable at that point.

Do not claim maturity, publication readiness, benchmark success, installation success, or completion without the corresponding persisted evidence.
