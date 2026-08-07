# Dependency Rules

## Global Rules

- Dependencies point toward stable abstractions and explicit contracts.
- A module must not query another boundary's private tables directly.
- Internal classes are not public APIs.
- Cyclic boundary dependencies are forbidden unless an ADR documents a temporary migration state.
- Shared Kernel additions require impact review because they increase coupling.

## Rule Registry

| Rule ID | Source | Allowed target | Forbidden target/access | Enforcement |
|---|---|---|---|---|
| `DEP-001` | `<boundary/module>` | `<contract>` | `<internal model/table>` | architecture test / review |

## Automated Enforcement

Document architecture tests, static checks, forbidden imports, namespace rules, or dependency graph checks here.
