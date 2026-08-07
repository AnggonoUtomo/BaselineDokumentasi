# Module Catalog

| Module | Purpose | Owns data | Public contracts | Publishes events | Consumes | Forbidden dependencies | Owner |
|---|---|---|---|---|---|---|---|

## Boundary rules

- A module must not query another module's private tables directly unless explicitly approved.
- Cross-module synchronous behavior uses an explicit public contract.
- Cross-module asynchronous behavior uses documented events/messages.
- Shared code must be minimal and must not contain module-specific business rules.

## Per-module template

### `<Module name>`

- Purpose:
- In scope:
- Out of scope:
- Entities/aggregates:
- Public application contracts:
- Events published:
- Events consumed:
- Data ownership:
- Authorization boundary:
- Dependencies:
- Invariants:
