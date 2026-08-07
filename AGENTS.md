# Triangle Home Defense Website Agent Instructions

This repository is the canonical GitHub Pages production repository for `trianglehomedefense.com`.

## Required first step

Before changing website code, deployment configuration, branches, workflows, or the custom domain, read `DEPLOYMENT.md` in this repository and follow it as the deployment source of truth.

## Production rules

- Production repo: `trianglehomedefense/trianglehomedefense.github.io`
- Production branch: `main`
- Public domain: `trianglehomedefense.com`
- Only this production owner should contain a `CNAME` claiming `trianglehomedefense.com` unless ownership is intentionally migrated.
- Public business phone: `984-399-5003`
- Use `tel:+19843995003` and `sms:+19843995003`.
- Never publish the owner's personal number.

## Working mode

1. Confirm live domain -> Pages owner -> branch -> CNAME -> current commit before editing.
2. Make the smallest change that solves the requested problem.
3. Do not redesign or alter deployment architecture when the issue is only publishing, caching, or content.
4. If live output is stale, match the live HTML to repo history before changing code.
5. Do not add or change GitHub Actions workflows unless there is evidence the production Pages source actually uses Actions.
6. Preserve real THD field imagery; do not substitute generated wildlife, damage, or field-service imagery.
7. Verify mobile readability, public phone links, and absence of the personal phone before declaring production complete.
8. Stop once the requested live result is verified.

## Brand direction

- Primary identity: burgundy / 2003 Corvette 50th Anniversary Anniversary Red Metallic reference (RPO 94U / WA-820K), adapted for readable digital use.
- Supporting palette: warm cream, stone/rock neutrals, limited muted natural green.
- Do not drift into an all-green wildlife-company look.
- Maintain strong contrast and age-8-to-80 readability.

## Documentation rule

If the production architecture changes, update `DEPLOYMENT.md` and this file in the same change.
