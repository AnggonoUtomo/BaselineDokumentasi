# Change Classification

Classify every proposed change before planning or coding.

## Levels

| Level | Typical examples | Minimum documentation | Approval |
|---|---|---|---|
| `TRIVIAL` | Typo, comments, local rename, non-behavioral formatting | Task record, verification evidence | AI/self-review unless protected area |
| `STANDARD` | Small feature, isolated bug, bounded refactor | Work-item brief, tasks, tests, completion report | Work-item owner |
| `SIGNIFICANT` | New module, schema/API change, external integration, cross-boundary refactor | Full package, impact assessment, ADR when architectural | Human approval required |
| `CRITICAL` | Authentication/authorization, destructive migration, breaking API, compliance, high-cost infrastructure | Full package, threat/risk review, rollback, release gate | Named human approver required |

## Classification Questions

- Does it alter externally observable behavior?
- Does it cross module or boundary ownership?
- Does it modify persistent data or migration paths?
- Does it change public contracts, security, privacy, compliance, cost, or availability?
- Is rollback difficult, destructive, or time-sensitive?
- Does it introduce a new dependency or external vendor?

Choose the highest applicable level. Record the rationale in the work-item metadata.

## Escalation Rule

A work item may be escalated at any time. It may not be downgraded after implementation begins without a written rationale and human approval.
