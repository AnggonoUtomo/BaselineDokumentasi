# Dependency Upgrade Package

Use this package for `dependency-upgrade` work. Copy the entire directory into the matching work-item collection and replace all placeholders.

## Required sequence

1. `01-UPGRADE-PROPOSAL.md` — Dependency, current/target versions, reason, support/security/license status.
2. `02-COMPATIBILITY-ASSESSMENT.md` — Breaking changes, transitive dependencies, platform/runtime and API impact.
3. `03-UPGRADE-PLAN.md` — Incremental steps, lockfile/config changes, test matrix and rollback.
4. `04-VALIDATION-REPORT.md` — Build, tests, security scan, performance and runtime observation.
5. `05-COMPLETION-REPORT.md` — Version adopted, changes, exceptions, follow-up and registry update.

Also add `CONTEXT-PACK.md`, `DEVIATION-RECORD.md` when needed, and `EVIDENCE-MANIFEST.md` before completion.
