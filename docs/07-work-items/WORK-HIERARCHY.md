# Work Hierarchy

Recommended hierarchy:

```text
INITIATIVE
└── ARCHITECTURE / BOUNDARY CHANGE
    ├── MODULE
    │   ├── FEATURE
    │   │   ├── TASK
    │   │   └── BUG / REFACTOR
    │   └── FEATURE
    └── INTEGRATION / MIGRATION
```

## Relationship Rules

- Every task has exactly one parent work item.
- A work item may depend on multiple work items but must not create an undocumented cycle.
- Emergent work is linked to the task that discovered it using `discovered_by`.
- Deferred child modules remain documented as candidates; they are not silently implemented.
