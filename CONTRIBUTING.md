# Contributing to Spradley

These are the org-wide defaults. A repository's own `README.md`,
`CONTRIBUTING.md` or `AGENTS.md` takes precedence, including its branch rules
(in `spradley-app`, for example, work branches off `dev`, and `lab` is never
merged back).

## Workflow

1. Branch off the repo's default branch.
2. Make surgical, focused changes. Match the existing style.
3. Run the repo's checks locally before opening a PR (lint, type-check, tests).
4. Open a PR using the template. Keep PRs small and reviewable.
5. Squash-merge once CI is green.

## House rules

- **No em dashes** in code, comments, commits, or docs. Use a period, comma,
  colon, parentheses, or semicolon instead.
- **Privacy first.** No PII in logs. Reporting, quotes and analysis read the
  redacted answer only and fail closed when it is missing; never add a path that
  falls back to the raw answer. The live interviewer is the one deliberate
  exception: it hears answers unredacted, because it has to follow the
  conversation.
- **No GDPR shortcuts.** Consent, audit logs, and data export and deletion are
  real requirements.
- **Tenant isolation lives in code.** The app's database role bypasses
  Row-Level Security, so RLS protects nothing. Every query on a company's data
  goes through the repository layer's company scope, never a raw query.

## Reporting security issues

Do not open a public issue. See [SECURITY.md](./SECURITY.md).
