# Module Lifecycle

States: `candidate → accepted → active → stable → deprecated → retired`.

| State | Meaning | Allowed implementation |
|---|---|---|
| candidate | Investigated, not approved | No production implementation |
| accepted | Boundary placement approved | Skeleton/planning allowed |
| active | Under development | Incremental tasks allowed |
| stable | Supported contract and ownership | Normal maintenance |
| deprecated | Replacement and deadline announced | Compatibility fixes only |
| retired | Removed from active system | Historical docs retained |

Transitions that split, merge, move, deprecate, or retire a module require an architecture-change or deprecation package.
