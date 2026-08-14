# Review

## Required checkpoint reviews

Each milestone requires:

1. Spec-compliance review against `docs/WINNING.md`.
2. Code-quality and risk review.
3. Fresh automated verification.
4. Domain evidence where tests are insufficient.

Blocking findings remain open here until fixed and reverified.

## Findings

### M0 external-platform limitation

- GitHub returned HTTP 403 for branch protection and HTTP 422 for secret scanning on the current private-repository tier.
- Resolution: retain privacy; use mandatory worktrees, clean-branch checks, local secret scanning, CI, and PR review discipline. This does not block M1 but remains open before external collaboration.
