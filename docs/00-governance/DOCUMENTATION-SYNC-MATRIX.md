# Documentation Sync Matrix

Use this matrix before marking any work item complete.

| Code/system change | Documents to inspect/update |
|---|---|
| New boundary | System Design, Boundary Registry, Module Catalog, dependency rules, ADR |
| New/changed module | Boundary docs, Module Catalog, contracts, lifecycle |
| Database/table/column | Database Design, data ownership, migration and rollback docs |
| Public API | API Spec, compatibility/deprecation, security and test plan |
| Domain/integration event | Event Catalog, producer/consumer contracts, observability |
| Role/permission/policy | Authorization Matrix, threat model, security tests |
| External integration | Integration Catalog, contract, failure modes, runbook |
| Dependency/library | Dependency Register, upgrade record, license/security notes |
| Deployment/config | Technical Spec, deployment/runbook, rollback procedure |
| Breaking change | ADR, compatibility plan, deprecation/removal package, release notes |
| Incident fix | Incident record, root cause, prevention actions, runbook/tests |
| Performance change | Performance baseline, benchmark report, capacity assumptions |

Completion reports must list every inspected document, including those confirmed as `no change required`.
