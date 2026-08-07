# Triangle Home Defense Website Deployment Protocol

Last updated: 2026-08-07

## Purpose

Keep website publishing fast, safe, and predictable. This file is the deployment source of truth. If the production setup changes, update this file in the same change.

## Current Production Model

- Public domain: `trianglehomedefense.com`
- Canonical GitHub Pages repo: `trianglehomedefense/trianglehomedefense.github.io`
- Production branch: `main`
- Custom domain file: `CNAME`
- `CNAME` must contain exactly: `trianglehomedefense.com`
- Only ONE repository may claim the custom domain at a time.
- `trianglehomedefense/trianglehomedefense.com` may hold source/assets, but it must not also claim the custom domain unless production ownership is intentionally moved.

## Non-Negotiable Public Contact Rule

- Public business phone: `984-399-5003`
- Phone links: `tel:+19843995003`
- Text links: `sms:+19843995003`
- Never publish the owner's personal number.

## Fast Preflight Before Any Website Change

1. Confirm which repo currently owns the live domain.
2. Confirm only that repo contains `CNAME` for `trianglehomedefense.com`.
3. Confirm production branch is `main`.
4. Fetch live HTML and match it to the expected repo/commit before editing.
5. Search production source for the personal phone number and confirm zero occurrences.
6. Do not redesign, add workflows, or change deployment architecture unless the problem actually requires it.

## Publish Sequence

1. Make the smallest necessary change.
2. Commit intentionally to the production path.
3. Verify the live site title and visible layout.
4. Verify `984-399-5003` is visible and clickable.
5. Verify the personal phone number is absent from live output.
6. Stop once the live site is correct.

## If the Live Site Shows an Old Build

Treat it first as a deployment-source problem, not a browser-cache problem.

- Compare live HTML to repository history.
- Identify the exact old commit if possible.
- Check repo ownership, branch, CNAME, and Pages source before changing code.
- Avoid branch churn and repeated blind rebuild commits.

## If the Site 404s

- Check whether `CNAME` was removed, moved, or duplicated.
- Restore the last known working single-owner CNAME configuration first.
- Verify Pages is publishing from the intended repo/branch.
- Do not make unrelated content/design changes while restoring service.

## Deployment Principle

**Live domain -> Pages owner -> branch -> CNAME -> current commit -> edit -> verify.**

That order should be followed every time.
