# ARC-ACL-001 — Menambahkan Boundary AccessControl

```yaml
id: ARC-ACL-001
kind: architecture-change
classification: CRITICAL
status: proposed
parent: null
discovered_by: FTR-USR-004
depends_on: []
related_adrs: [ADR-0012]
```

## Kandidat Module Turunan

- `MOD-ACL-IDN` — Identity
- `MOD-ACL-AUT` — Authentication
- `MOD-ACL-AZR` — Authorization
- `MOD-ACL-RLM` — Role Management
- `MOD-ACL-PRM` — Permission Management
- `MOD-ACL-SES` — Session Management
- `MOD-ACL-AUD` — Access Audit

Semua module di atas masih berstatus kandidat dan tidak otomatis menjadi scope implementasi. Proposal wajib menentukan mana yang diterima, ditunda, digabung, atau ditolak.
