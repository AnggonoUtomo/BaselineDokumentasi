# Data Migration Package

Use this package for `data-migration` work. Copy the entire directory into the matching work-item collection and replace all placeholders.

## Required sequence

1. `01-MIGRATION-PROPOSAL.md` — Business reason, source/target, volume, downtime, risk and ownership.
2. `02-SOURCE-TARGET-MAPPING.md` — Field/entity mapping, transformation, defaults, rejected records and lineage.
3. `03-DATA-QUALITY-ASSESSMENT.md` — Completeness, validity, duplicates, referential integrity and remediation.
4. `04-MIGRATION-PLAN.md` — Phases, rehearsal, backup, batching, idempotency, freeze window and cutover.
5. `05-ROLLBACK-PLAN.md` — Trigger, restore path, reverse transform, time limit and data-loss boundary.
6. `06-RECONCILIATION-REPORT.md` — Counts, totals, hashes/samples, exceptions and sign-off.
7. `07-POST-MIGRATION-REPORT.md` — Outcome, residual issues, monitoring, cleanup and lessons.

Also add `CONTEXT-PACK.md`, `DEVIATION-RECORD.md` when needed, and `EVIDENCE-MANIFEST.md` before completion.
