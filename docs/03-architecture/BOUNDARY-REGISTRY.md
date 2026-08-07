# Boundary Registry

| ID | Boundary | Purpose | Owner | Status | Path | ADR |
|---|---|---|---|---|---|---|
| `<BC-ID>` | `<Name>` | `<Capability>` | `<Owner>` | candidate/active/stable/deprecated/retired | `boundaries/...` | `<ADR>` |

## Rules

- Every architectural boundary has a stable ID.
- Child modules are registered in the boundary's `MODULE-CATALOG.md`.
- Cross-boundary access must use an approved contract, event, or documented integration mechanism.
- A boundary may not expose internal database models as its public contract.
