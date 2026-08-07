# Documentation Standard

## Purpose

Define how project documentation is created, identified, approved, changed, and connected to code.

## Required metadata

Each governed document begins with:

```yaml
---
id: <DOC-ID>
title: <Title>
status: draft
version: 0.1.0
owner: <role-or-name>
reviewers: []
created: YYYY-MM-DD
updated: YYYY-MM-DD
related: []
---
```

## Status definitions

- `draft` — incomplete and not authoritative.
- `in-review` — ready for stakeholder review.
- `approved` — accepted as source of truth.
- `ready` — approved and all entry criteria for execution are met.
- `in-progress` — currently being implemented.
- `blocked` — cannot proceed; blocker is documented.
- `completed` — acceptance criteria and evidence are complete.
- `superseded` — replaced by a newer document or decision.

## Writing rules

- Use explicit, testable statements.
- Use `MUST`, `SHOULD`, and `MAY` intentionally.
- Separate facts, decisions, assumptions, and questions.
- Assign stable IDs to requirements, rules, decisions, features, tasks, and tests.
- Avoid terms such as “fast”, “secure”, or “user-friendly” without measurable criteria.
- Reference repository paths instead of copying large code sections.
- Do not remove a required section; use `Not applicable — <reason>`.

## Change control

When scope or behavior changes:

1. Update the governing requirement/specification.
2. Record the reason and impact.
3. Create or update an ADR when architecture is affected.
4. Update affected tasks and acceptance criteria.
5. Update traceability.
6. Resume implementation only after approval/readiness is restored.

## Review cadence

Review project baseline documents at each major release and feature documents before implementation and before closure.

## Controlled extensibility

This documentation baseline may evolve through `DOCUMENT-CREATION-POLICY.md`. New project-specific documents must fit an existing governed category. New reusable templates require an approved `DOCUMENT-PROPOSAL.md`. Architecture evolution uses the standard Architecture Change Package.
