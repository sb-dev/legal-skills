# Legal Skills — Bootstrap Execution Contract

**Repository:** `sb-dev/legal-skills`  
**Working branch:** `feat/bootstrap-3`  
**Governing bootstrap:** `docs/research-logs/2026-09-08-legal-skills-new-project-bootstrap-process.md`
**Operator command:** `/bootstrap`

This contract defines execution mechanics only. The bootstrap specification remains authoritative for substantive requirements, domain evidence rules, and exit criteria.

## Default authorisation

Invoking `/bootstrap` authorises execution from the next incomplete stage through the final bootstrap stage.

The user does not need to restate the current stage, repeat the execution instructions, or provide a stage range on each run. An explicit user instruction may narrow or stop that range.

Determine accepted progress from repository state and persisted research logs on `feat/bootstrap-3`. Do not infer accepted completion from conversation memory.

## Stage execution

For every remaining stage:

```text
read complete stage
→ read accepted dependencies
→ extract requirements and exit criteria
→ perform substantive work
→ persist required outputs
→ verify actual outputs
→ repair failures
→ commit only that stage
→ push commit
→ verify remote commit
→ continue automatically
```

`/bootstrap` is the public entry point. It uses these internal support skills as applicable:

```text
bootstrap-stage-execution
bootstrap-research
direct-source-extraction
```

Domain-specific legal evidence rules come directly from the governing legal bootstrap specification.

## Evidence rules

Do not:

- substitute a summary for required substantive research;
- substitute a bibliography, publisher description, secondary summary, or model memory for required direct-source examination;
- describe expected execution when actual execution is required;
- claim tests, benchmarks, installations, comparisons, searches, or tool runs that did not occur;
- weaken a bootstrap exit criterion because the work is difficult;
- silently replace, remove, or demote a user-provided source where permission is required;
- batch independently defined stages into one commit.

## Repair before escalation

A failed search, dead URL, failed command, test failure, extraction problem, implementation defect, or verification failure is not by itself a blocker.

Use the smallest responsible repair or an allowed alternative path and continue.

## Stop only for genuine user decisions

Stop when progress actually depends on the user, including:

- explicit permission or approval required by the bootstrap;
- supplied-source substitution/removal/demotion requiring approval;
- materially different valid interpretations that change project scope or accepted behaviour;
- unavailable mandatory evidence or capability that cannot be repaired or substituted within the bootstrap rules;
- a contradiction that would require reopening accepted prior work without authority;
- unrelated local changes would have to be discarded or overwritten.

Do not stop merely because work is difficult, a first attempt failed, or verification found defects.

## Verification

Before completing each stage:

1. re-read the original stage requirements and exit criteria;
2. inspect the actual repository outputs;
3. run required tests, execution, comparisons, or installation checks;
4. repair every mandatory failure;
5. persist enough verification evidence to justify completion.

An exhaustive conformance table is optional unless the stage, bootstrap, or risk level requires one.

## Commit and remote rule

Use one commit per completed stage and include the stage identifier in the commit message, for example:

```text
stage 4: challenge professional practice
stage 12 P3: extract specialised corpus
```

Push every completed stage commit to `origin/feat/bootstrap-3`, verify the remote branch points to that commit, then continue automatically.

## Context rule

Reconstruct every stage from:

```text
governing bootstrap specification
+
accepted prior-stage outputs on feat/bootstrap-3
+
this execution contract
```

Do not rely on conversation memory for accepted state.

## Final audit

After the final stage, audit the resulting repository against the bootstrap's global acceptance requirements. Do not claim maturity, publication readiness, benchmark success, installation success, or completion without the required evidence.
