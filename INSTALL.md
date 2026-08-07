# Install SEOS into a Project

## New Project

Copy all files from this package into the repository root. Keep the repository's existing `.gitignore`; use `.gitignore.template-notes` only as guidance.

Then instruct the AI:

```text
Read AGENTS.md and execute docs/00-governance/AI-PROJECT-BOOTSTRAP-PROMPT.md.
Do not code during bootstrap. Inspect the repository, separate verified facts from assumptions, fill baseline documents in order, and finish with a readiness verdict.
```

## Existing Project

1. Copy `docs/`, `AGENTS.md`, and `SEOS-VERSION`.
2. Merge rather than overwrite project-specific `README.md` or existing agent instructions.
3. Bootstrap from repository evidence.
4. Register known active work and architecture decisions.
5. Do not retroactively fabricate evidence for completed work; label reconstructed history clearly.

## Starting a Work Item

```bash
cp -R docs/07-work-items/templates/<package>   docs/07-work-items/<collection>/<WORK-ID>-<slug>
```

Update `WORK-ITEM-REGISTRY.md`, metadata, and package documents before coding.
