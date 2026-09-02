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

### Public-collaboration transition

- On 2026-09-02 the product owner explicitly authorised public repository visibility to enable outside contribution, superseding the earlier privacy-only repository decision.
- Pre-publication tracked-file inspection found no credential-like material or committed private transcript.
- Contributor and security-reporting guidance must be present before visibility changes; GitHub visibility and security settings require post-change verification.
- Public repository visibility does not authorise a public deployment or any publication of relational data.
