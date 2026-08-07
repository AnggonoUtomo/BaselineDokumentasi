# AI Project Bootstrap Prompt

Use this prompt once after copying the template into a project.

---

You are initializing the project's engineering documentation system.

## Mandatory instructions

1. Read `AGENTS.md` and all files in `docs/00-governance/`.
2. Inspect the repository before writing project facts:
   - languages and frameworks;
   - package/dependency manifests;
   - source directories;
   - modules or bounded contexts;
   - database and migration structure;
   - API/routes;
   - tests and quality tools;
   - CI/CD and deployment files;
   - existing documentation;
   - current Git state when available.
3. Separate findings into:
   - **Verified facts** — directly supported by repository evidence;
   - **Assumptions** — plausible but unverified;
   - **Open questions** — needed decisions or missing information.
4. Do not generate architecture merely from preference. Preserve established project patterns unless a change is explicitly approved.
5. Fill baseline documents in this order:
   1. `docs/01-product/PROJECT-BRIEF.md`
   2. `docs/01-product/SCOPE.md`
   3. `docs/01-product/PRD.md`
   4. `docs/02-requirements/REQUIREMENTS.md`
   5. `docs/03-architecture/SYSTEM-DESIGN.md`
   6. `docs/03-architecture/MODULE-CATALOG.md`
   7. `docs/04-design/DATABASE-DESIGN.md`
   8. `docs/04-design/API-SPEC.md`
   9. `docs/05-engineering/TECHNICAL-SPEC.md`
   10. `docs/05-engineering/TESTING-STRATEGY.md`
   11. `docs/06-planning/IMPLEMENTATION-PLAN.md`
   12. `docs/02-requirements/TRACEABILITY-MATRIX.md`
6. Use stable IDs from `docs/00-governance/ID-CONVENTIONS.md`.
7. Preserve every heading in each template. Write `Not applicable` with a reason rather than deleting a section.
8. Add source references as repository paths and line ranges where practical.
9. Do not start coding.

## Final bootstrap output

Produce:

- repository inventory;
- documents completed;
- assumptions made;
- unresolved decisions;
- documentation inconsistencies found;
- recommended first feature package;
- readiness verdict: `NOT READY`, `CONDITIONALLY READY`, or `READY FOR FEATURE PLANNING`.

---
