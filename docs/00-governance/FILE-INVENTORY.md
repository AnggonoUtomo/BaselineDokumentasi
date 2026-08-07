# SEOS File Inventory

Version: `2.0.0`

This repository contains the complete SEOS baseline: root operating instructions, governance, product and requirements templates, architecture and boundary records, design catalogs, engineering standards, implementation planning, quality gates, operations, decisions, immutable baseline snapshots, active task registries, worked examples, and eleven reusable work-item packages.

## Canonical roots

- `AGENTS.md`, `README.md`, `INSTALL.md`, `SEOS-VERSION`
- `docs/00-governance` through `docs/11-baselines`
- `docs/07-work-items/templates`
- `tasks`
- `examples`

## Reusable packages

- architecture-change
- bug-fix
- data-migration
- dependency-upgrade
- deprecation-removal
- feature
- incident-follow-up
- integration
- performance-improvement
- refactoring
- security-change
- shared execution records

## Verification

Use the repository tree or run:

```bash
git ls-files
find docs -type f | sort
```

Empty work-item collections are retained with `.gitkeep` files. This inventory is intentionally category-based so it remains readable; Git is the authoritative per-file inventory.
