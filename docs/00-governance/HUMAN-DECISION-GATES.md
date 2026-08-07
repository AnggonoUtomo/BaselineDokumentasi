# Human Decision Gates

AI may investigate, draft, compare options, and prepare evidence. AI must not self-approve the following:

- New or removed architectural boundary/module
- Breaking API or contract change
- Authentication, authorization, identity, secret, or cryptographic change
- Destructive or irreversible data migration
- Data ownership or retention change
- New production dependency, external vendor, paid service, or material cost increase
- Compliance, legal, privacy, or audit control change
- Production rollout with significant outage or rollback risk
- Relaxation of quality, security, or acceptance criteria

## Gate Record

Record:

```yaml
gate: architecture-approval
decision: approved | rejected | conditional
approver: <human name or role>
date: YYYY-MM-DD
conditions: []
evidence: []
```

Absence of approval means `not approved`.
