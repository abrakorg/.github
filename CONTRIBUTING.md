# Abrak Contribution Workflow (Free-Plan Friendly)

This organization uses a local-first workflow because GitHub branch protections/rulesets may be unavailable on private repositories in the current plan.

## Core Rules
- Use feature branches. Do not work directly on `main`.
- Open a PR even if you are the only developer (keeps change history clean).
- Prefer squash merge.
- Do not commit secrets, tokens, passwords, or private keys.
- Update `.abrak/manifest.yml` and `.abrak/service-contract.yml` when contracts/ownership/runtime behavior change.
- If integration contracts change, update `ABRAK_CO_DATACENTER/registry/*`.

## Branch Naming
- `feat/<area>-<short-topic>`
- `fix/<area>-<short-topic>`
- `docs/<area>-<short-topic>`
- `chore/<area>-<short-topic>`
- `refactor/<area>-<short-topic>`

Examples:
- `feat/hub-license-events`
- `fix/odoo-auth-callback`
- `docs/registry-service-schema`

## Commit Message Format (recommended)
- First line (subject): `<type>(<scope>): <summary>`
- Keep subject concise (prefer <= 72 chars)

Examples:
- `feat(hub): add usage event ingestion endpoint`
- `fix(odoo): prevent duplicate license sync`
- `docs(registry): add connector service schema refs`

## Validation Before Merge
- Test the changed path
- Check logs/errors for regressions
- Record rollback path for risky changes
- Document any untested part explicitly

## Abrak Red Lines (Operational)
Never perform direct operational actions on:
- `PC.HAIDA.CO`
- `CRM.HAIDA.CO`

If a task might affect them, stop and separate the environment first.
