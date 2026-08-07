# Development Workflow

## Lifecycle

```text
DISCOVER → DEFINE → DESIGN → PLAN → BUILD → VERIFY → REVIEW → RELEASE → OPERATE
```

## Phase gates

### Discover

Outputs: repository inventory, stakeholders, problem statement, constraints, assumptions.

Exit gate: problem and context are understandable.

### Define

Outputs: PRD, scope, requirements, business rules, acceptance criteria.

Exit gate: requirements are approved and testable.

### Design

Outputs: system design, module boundaries, data/API design, ADRs, security implications.

Exit gate: implementation approach is coherent and risks are known.

### Plan

Outputs: implementation slices, dependencies, tasks, test plan, rollback plan.

Exit gate: Definition of Ready is satisfied.

### Build

Outputs: code and tests for one task/slice.

Exit gate: local task acceptance criteria pass.

### Verify

Outputs: automated checks, manual verification, evidence, regression results.

Exit gate: no unresolved critical failures.

### Review

Outputs: five-axis review, security/performance review where relevant, resolved findings.

Exit gate: merge/release recommendation exists.

### Release

Outputs: release notes, deployment and rollback evidence.

Exit gate: release is deployed or explicitly deferred.

### Operate

Outputs: monitoring, incidents, runbook updates, technical debt and follow-up tasks.

## Incremental rule

Every implementation slice must leave the repository in a valid, testable state and should be independently reviewable and revertible.

## Emergent work and architecture evolution

Development may reveal work that was not reasonably knowable during bootstrap. This is allowed, but it must not be hidden inside the active implementation task.

When a new boundary, submodule family, contract, integration, data owner, or architectural responsibility is discovered:

1. Pause the affected implementation slice at a safe state.
2. Create an Architecture Discovery Record.
3. Decide whether the current task can continue, must be blocked, or should be split.
4. If architecture changes, create the full Architecture Change Package.
5. Approve the proposal, impact assessment, and ADR.
6. Update baseline catalogs and traceability.
7. Create new ready tasks and resume incremental implementation.
8. Complete validation and completion reports after coding.

The discovery itself is not approval to implement.
