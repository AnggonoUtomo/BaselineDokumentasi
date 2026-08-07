# Work Item Lifecycle

## States

`discovered → proposed → approved → ready → in_progress → implemented → verified → completed → archived`

Optional states: `blocked`, `deferred`, `rejected`, `cancelled`, `superseded`.

## Transition Rules

| From | To | Required evidence |
|---|---|---|
| discovered | proposed | Discovery/problem record |
| proposed | approved | Scope, impact, decision owner |
| approved | ready | Definition of Ready satisfied |
| ready | in_progress | Active task selected and context pack prepared |
| in_progress | implemented | Code/config/docs produced; no completion claim yet |
| implemented | verified | Required tests/checks pass |
| verified | completed | Review, completion report, baseline sync |
| completed | archived | Release/reference recorded |

Forbidden shortcuts include `proposed → in_progress`, `implemented → completed`, and `blocked → completed`.

## Metadata

Every work-item root document must contain:

```yaml
id: WI-AREA-NNN
kind: feature
classification: STANDARD
status: proposed
owner: unassigned
created_at: YYYY-MM-DD
updated_at: YYYY-MM-DD
parent: null
depends_on: []
blocks: []
related_adrs: []
```
