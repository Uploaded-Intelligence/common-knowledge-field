# Contributing to Common Knowledge Field

Thank you for helping build infrastructure for lower-cost shared understanding.

## Start here

1. Read `docs/WINNING.md` and the milestone gate relevant to your change.
2. Check existing issues before proposing new scope.
3. For substantial changes, open an issue describing purpose, scope, acceptance evidence, and rollback.
4. Keep pull requests small enough to review against one coherent outcome.

## Privacy boundary

Do not commit or paste:

- real private-message transcripts or excerpts;
- participant names, handles, identifiers, or relationship metadata;
- screenshots containing conversation content;
- Beeper tokens, API keys, database keys, capability links, or other credentials;
- model logs, crash reports, or exports containing source text.

Tests and demonstrations must use synthetic data or material whose participants explicitly consented to public release. When in doubt, use synthetic data.

## Product invariants

- AI interpretations remain provisional until participant judgment.
- Joint ratification requires affirmative acts from every represented participant.
- Every visible semantic unit must resolve to evidence.
- Source-chat access is read-only in the MVP.
- No cloud-model fallback, hidden-personality inference, or automatic interpersonal intervention.
- Corrections append or supersede; they do not rewrite history.

## Development workflow

- Create a feature branch; Codex-authored branches use the `codex/` prefix.
- Develop production behaviour test-first.
- Preserve strict TypeScript and exact dependency pins.
- Run the verification commands documented in `docs/RUNBOOK.md`.
- Update canonical documentation when architecture, risk, progress, or decisions change.
- Explain which acceptance gate the pull request advances and include fresh evidence.

Pull requests require passing CI and review. A green test suite is not enough when the change affects UX, privacy, security, integration, performance, or accessibility.

## Licensing

By contributing, you agree that your contribution is licensed under AGPL-3.0-only. Record adapted third-party work in `THIRD_PARTY_NOTICES.md` and the research/licensing ledger before merging it.

## Security

Do not open a public issue for a vulnerability or suspected data exposure. Follow `SECURITY.md`.
