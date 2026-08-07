# AI Context Policy

## Goal

Give an AI enough verified context to complete one task without loading the entire project or inventing missing facts.

## Required Context Pack

- Active task and parent work item
- Classification and current lifecycle state
- Relevant requirements and acceptance criteria
- Relevant ADRs, boundary contracts, and dependency rules
- Allowed and forbidden files/areas
- Existing patterns to preserve
- Verification commands
- Known assumptions, open questions, and risks

## Rules

- One active implementation task per AI execution unless explicitly approved.
- Prefer exact document sections and file paths over broad repository summaries.
- Mark repository facts, assumptions, and recommendations separately.
- Never hide discovered scope expansion; create a discovery/deviation record.
- Context packs are disposable execution artifacts, not new sources of truth.
