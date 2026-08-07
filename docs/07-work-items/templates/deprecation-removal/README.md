# Deprecation Removal Package

Use this package for `deprecation-removal` work. Copy the entire directory into the matching work-item collection and replace all placeholders.

## Required sequence

1. `01-DEPRECATION-PROPOSAL.md` — Deprecated surface, reason, consumers, replacement and compatibility window.
2. `02-CONSUMER-IMPACT.md` — Known consumers, usage evidence, migration effort and owner.
3. `03-TRANSITION-PLAN.md` — Announcement, dual-run/shim, migration steps, telemetry and deadline.
4. `04-REMOVAL-READINESS.md` — Usage zero/approved, backups, rollback, docs/tests and gate approval.
5. `05-REMOVAL-REPORT.md` — Removed artifacts, consumer status, incidents, cleanup and release.

Also add `CONTEXT-PACK.md`, `DEVIATION-RECORD.md` when needed, and `EVIDENCE-MANIFEST.md` before completion.
