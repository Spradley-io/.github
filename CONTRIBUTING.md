# Contributing to Spradley

These are the org-wide defaults. Individual repositories may add their own
`README.md` and `CONTRIBUTING.md` with stack-specific setup; those take
precedence.

## Workflow

1. Branch off the repo's default branch.
2. Make surgical, focused changes. Match the existing style.
3. Run the repo's checks locally before opening a PR (lint, type-check, tests).
4. Open a PR using the template. Keep PRs small and reviewable.
5. Squash-merge once CI is green.

## House rules

- **No em dashes** in code, comments, commits, or docs. Use a period, comma,
  colon, parentheses, or semicolon instead.
- **Privacy first.** No PII into AI processing or logs. Employee answers are
  scrubbed before any AI step.
- **No GDPR shortcuts.** Consent, audit logs, and data export/deletion are real
  requirements.
- **Security by default.** Respect Row-Level Security and least-privilege
  access on every new query path.

## Reporting security issues

Do not open a public issue. See [SECURITY.md](./SECURITY.md).
