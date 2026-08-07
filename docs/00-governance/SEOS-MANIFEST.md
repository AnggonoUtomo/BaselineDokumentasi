# SEOS Manifest

## Identity

- Name: Software Engineering Operating System (SEOS)
- Version: 2.0.0
- Purpose: AI-friendly, repository-local operating system for planning, implementing, validating, releasing, and evolving software.

## Core Principles

1. Documentation is executable guidance, not decoration.
2. Every material code change maps to a classified work item.
3. Work proceeds through explicit pre-work, implementation, and post-work evidence.
4. Baseline documents describe the current truth; work-item documents preserve change history.
5. AI may propose change, but human gates protect high-impact decisions.
6. One active task, bounded context, measurable acceptance criteria, verifiable evidence.

## Canonical Lifecycle

`DISCOVER → CLASSIFY → PROPOSE → APPROVE → READY → IMPLEMENT → VERIFY → REVIEW → COMPLETE → BASELINE-SYNC → ARCHIVE`

## Source-of-Truth Priority

1. Approved active work item and task
2. Accepted ADRs and boundary contracts
3. Current baseline architecture/design documents
4. Engineering and quality standards
5. Existing implementation
6. Historical work-item documents

When these disagree, stop and create a deviation or decision record. Do not silently choose.
