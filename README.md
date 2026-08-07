# Software Engineering Operating System (SEOS)

SEOS is a reusable, AI-friendly documentation and workflow baseline that lives inside a software repository. It governs work from project bootstrap through architecture evolution, incremental implementation, verification, release, operation, and historical baselines.

## What SEOS Solves

- Prevents AI or developers from coding before scope and acceptance criteria are ready
- Handles emergent work discovered during development
- Selects the right documentation depth for each change type and risk level
- Preserves current project truth separately from historical change records
- Makes completion claims evidence-based and traceable
- Controls architectural, security, data, dependency, and breaking changes through human gates

## Start Here

1. Read `AGENTS.md`.
2. Run the instructions in `docs/00-governance/AI-PROJECT-BOOTSTRAP-PROMPT.md`.
3. Fill baseline project documents without coding.
4. Register future work in `docs/07-work-items/WORK-ITEM-REGISTRY.md`.
5. Classify the change using `docs/00-governance/CHANGE-CLASSIFICATION.md`.
6. Copy the appropriate package from `docs/07-work-items/templates/`.
7. Satisfy Definition of Ready before coding and Definition of Done before completion.

## Work-Item Packages

- `feature`
- `architecture-change`
- `bug-fix`
- `refactoring`
- `integration`
- `data-migration`
- `dependency-upgrade`
- `security-change`
- `performance-improvement`
- `deprecation-removal`
- `incident-follow-up`

Each package includes pre-work, implementation planning, post-work validation, an AI context pack, deviation record, and evidence manifest.

## Emergent Architecture Example

When `AccessControl` is discovered during another task:

1. Stop at a valid repository state.
2. Register `ARC-ACL-001`.
3. Copy the `architecture-change` package.
4. Complete discovery, boundary proposal, impact assessment, and ADR.
5. Obtain the required human approval.
6. Create child module/feature tasks and implement vertical slices.
7. Validate dependency direction and public contracts.
8. Update the Boundary Registry, Module Catalog, contract documents, and evolution log.

## Baseline vs Work History

- `docs/01`–`06`, `08`–`09`, and architecture registries describe current truth.
- `docs/07-work-items` preserves why and how changes were made.
- `docs/11-baselines` preserves immutable release/milestone snapshots.

## Addy Osmani Agent Skills

SEOS routes compatible skills by lifecycle phase. Skills assist execution; repository documents remain the source of truth. Install and maintain external skills separately.
