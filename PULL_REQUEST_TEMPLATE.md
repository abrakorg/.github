# Abrak Pull Request Template / قالب درخواست ادغام ابرک

## Summary | خلاصه
- What changed?
- چرا این تغییر لازم بود؟

## Scope | دامنه اثر
- Repo / Module:
- Environment target: `dev` / `stage` / `prod` (if applicable)
- Related issue / task / ADR:

## Change Type | نوع تغییر
- [ ] Feature
- [ ] Bug fix
- [ ] Refactor
- [ ] Docs
- [ ] Infra/Config
- [ ] Security hardening

## Validation | اعتبارسنجی
- [ ] I tested the changed flow locally / on target dev environment
- [ ] I checked logs / errors for regressions
- [ ] I verified existing behavior still works (critical path)
- [ ] I documented any validation gap explicitly

## Risk & Rollback | ریسک و بازگشت
- Risk level: `low` / `medium` / `high`
- Rollback plan:
- User-facing impact / downtime (if any):

## Abrak Safety Checklist | چک‌لیست ایمنی ابرک
- [ ] No secrets/tokens/passwords committed
- [ ] No direct push to `main` (branch + PR workflow used)
- [ ] `.abrak/manifest.yml` updated (if repo metadata changed)
- [ ] `.abrak/service-contract.yml` updated (if service contract changed)
- [ ] Registry/docs updated in `ABRAK_CO_DATACENTER` (if integration changed)
- [ ] No operational action touched `PC.HAIDA.CO`
- [ ] No operational action touched `CRM.HAIDA.CO`

## Notes | توضیحات تکمیلی
- Anything reviewers/operators must know before merge
