# Document Creation and Evolution Policy

## Purpose

This policy controls when AI or developers may create new documents during development. The baseline documentation is extensible, but its structure must evolve deliberately and traceably.

## Core rule

AI may create a new project document only when an existing approved template cannot represent a newly discovered concern without becoming ambiguous, overloaded, or untraceable.

AI must not invent a parallel documentation system, rename baseline directories, or create arbitrary top-level folders.

## Permitted cases

A new document is permitted when at least one condition applies:

1. A new bounded context, module boundary, submodule, integration, security model, migration, or operational responsibility is discovered.
2. An approved feature exposes a missing architectural decision or cross-module contract.
3. The work needs separate pre-implementation and post-implementation evidence.
4. A document would otherwise mix unrelated lifecycle states or responsibilities.
5. A recurring document type appears in at least two work items and deserves a reusable template.

## Required process

Before creating a new document type or structure:

1. Search the baseline templates and existing project documents.
2. Record why the existing templates are insufficient.
3. Classify the change as project-specific document or reusable template.
4. Create a `DOC-PROPOSAL` using `docs/07-work-items/templates/DOCUMENT-PROPOSAL.md`.
5. For architecture changes, create an Architecture Change Package.
6. Update `DOCUMENTATION-STANDARD.md` and relevant indexes if the proposal is approved.
7. Preserve stable IDs and links from impacted documents.

## Project-specific document

A project-specific document describes one concrete concern, for example:

```text
docs/03-architecture/boundaries/BC-ACL-001-access-control/
```

It does not automatically become a reusable template.

## Reusable template

A new reusable template may be added only when:

- the structure is expected to be reused;
- its purpose does not overlap an existing template;
- required lifecycle inputs and outputs are defined;
- its creation rule is documented;
- it has a stable location under `docs/07-work-items/templates/`.

## Required metadata

Every new governed document must include:

```yaml
id:
title:
document_type:
status: draft
version: 0.1.0
owner:
created:
updated:
source_work_item:
related: []
```

## Prohibited behavior

- Creating a new architecture folder while coding without pausing the task.
- Treating an implementation discovery as an approved requirement.
- Hiding scope growth inside an existing task.
- Creating duplicate catalogs or competing sources of truth.
- Updating code first and documenting the decision afterward, except emergency repair explicitly recorded as a deviation.
