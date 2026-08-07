# Definition of Ready

A feature/task is ready only when all applicable items are checked.

## Feature readiness

- [ ] Problem and desired outcome are explicit.
- [ ] Scope and non-scope are defined.
- [ ] Stakeholders and users are identified.
- [ ] Functional and non-functional requirements have IDs.
- [ ] Business rules and edge cases are documented.
- [ ] Acceptance criteria are testable.
- [ ] Dependencies and module impacts are known.
- [ ] Data, API, security, privacy, and authorization impacts are reviewed.
- [ ] Architecture decisions are approved or not required.
- [ ] Risks, assumptions, and open questions are resolved enough to proceed.
- [ ] Rollout and rollback expectations are defined.

## Task readiness

- [ ] Task has one bounded objective.
- [ ] References point to approved specifications.
- [ ] Allowed and forbidden change areas are identified.
- [ ] Expected files/components are listed when known.
- [ ] Acceptance criteria and verification commands are present.
- [ ] Required tests are named.
- [ ] Dependencies are completed or explicitly available.
- [ ] Task can be completed without inventing missing requirements.

## Verdict

```yaml
readiness: READY | NOT_READY
approved_by: <human>
date: YYYY-MM-DD
notes: <text>
```
