# Testing Strategy

## Objectives

## Test levels

| Level | Purpose | Scope | Tool | Required in CI |
|---|---|---|---|---|

## Test selection rules

- Business rules require focused unit/domain tests where appropriate.
- Public behavior requires integration/feature tests.
- Bug fixes require a failing regression test before or alongside the fix.
- Critical user journeys require end-to-end coverage when feasible.

## Test data

## Isolation and external services

## Security testing

## Performance testing

## Quality gates

| Gate | Command/check | Blocking threshold |
|---|---|---|

## Flaky test policy

Do not retry away unexplained failures. Record owner, cause hypothesis, and corrective task.

## Evidence format

```text
Command:
Result:
Relevant output:
Environment:
Date:
```
