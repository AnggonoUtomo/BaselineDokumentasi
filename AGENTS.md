# AGENTS.md — SEOS AI Operating Rules

## Mission

Operate this repository through SEOS. Produce small, traceable, reviewable changes. Never substitute confident prose for evidence.

## Mandatory Reading Order

1. `docs/00-governance/SEOS-MANIFEST.md`
2. `docs/00-governance/CHANGE-CLASSIFICATION.md`
3. `docs/00-governance/WORK-ITEM-LIFECYCLE.md`
4. `docs/00-governance/HUMAN-DECISION-GATES.md`
5. Active work-item root and context pack
6. Relevant requirements, ADRs, boundaries, contracts, and engineering standards

## Source-of-Truth Priority

1. Approved active work item and task
2. Accepted ADRs and explicit contracts
3. Current baseline documents
4. Engineering/quality standards
5. Existing code
6. Historical work-item records

Conflicts require a deviation or decision record. Do not silently reconcile them.

## Mandatory Workflow

`DISCOVER → CLASSIFY → REGISTER → PROPOSE → APPROVE → READY → IMPLEMENT → VERIFY → REVIEW → COMPLETE → BASELINE-SYNC`

## Before Coding

- Classify the work as TRIVIAL, STANDARD, SIGNIFICANT, or CRITICAL.
- Register non-trivial work in `WORK-ITEM-REGISTRY.md`.
- Select and copy the correct package.
- Fill pre-work documents with facts, assumptions, risks, and acceptance criteria.
- Obtain human approval for protected decisions.
- Pass Definition of Ready.
- Create a task-specific `CONTEXT-PACK.md`.

## During Coding

- Work on one active task.
- Respect allowed/forbidden files and boundary rules.
- Implement the smallest vertical slice that can be tested.
- Run focused checks before expanding scope.
- Record unexpected architectural facts, behavior, or constraints.
- Never smuggle a feature into a refactor or a breaking change into a bug fix.

## Emergent Work

When new scope, module, boundary, contract, migration, security risk, or dependency is discovered:

1. Stop at a valid state.
2. Record discovery and link `discovered_by`.
3. Classify and register the new work.
4. Determine whether the current task is blocked, split, or safely continued.
5. Use the matching package; architecture discoveries use `architecture-change`.
6. Require ADR and human gate where applicable.
7. Resume only after the new work is Ready.

## After Coding

- Produce verification/review/completion documents required by the package.
- Complete `EVIDENCE-MANIFEST.md` with exact commands and results.
- Record deviations instead of rewriting history.
- Apply `DOCUMENTATION-SYNC-MATRIX.md`.
- Update current baseline documents and registries.
- Pass Definition of Done before status `completed`.

## Document Creation

AI may create an instance from an approved template. AI may not invent a new top-level category or reusable template without `DOCUMENT-PROPOSAL.md` and approval. Avoid duplicate sources of truth.

## Skill Routing

- Ambiguous idea: `idea-refine` / interview workflow
- Project or feature specification: `spec-driven-development`
- Task planning: `planning-and-task-breakdown`
- Context preparation: `context-engineering`
- Incremental coding: `incremental-implementation`
- Test-first behavior: `test-driven-development`
- Bugs/incidents: `debugging-and-error-recovery`
- API/contracts: `api-and-interface-design`
- Frontend: `frontend-ui-engineering`
- Architecture/ADR: `documentation-and-adrs`
- Review: `code-review-and-quality`
- Security: `security-and-hardening`
- Performance: `performance-optimization`
- Delivery: `ci-cd-and-automation`, `shipping-and-launch`

External skills support execution. They do not override SEOS documents or project decisions.

## Prohibited Claims

Do not say complete, secure, compatible, tested, or production-ready without corresponding evidence and named checks. Report skipped or unavailable checks explicitly.
