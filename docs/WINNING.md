# Winning: Common Knowledge Field MVP

## Purpose

CKF reduces the cognitive and relational cost of maintaining shared reality in text conversations. It continuously turns a linear message stream into a living, plural, evidence-bound field showing what matters, what each participant expressed, where interpretations differ, what remains unresolved, what changed, and what was actually agreed or committed to.

AI performs the primary mapping work automatically. Humans retain meaning, veto, correction, release, and consent.

## Terminal Goal-State

On an Apple-Silicon Mac, a person chats through Beeper while a docked CKF field:

1. Receives a pinned DM automatically and read-only.
2. Updates incrementally without spatial or semantic resets.
3. Surfaces at most three useful developments without a command or manual node authoring.
4. Grounds every interpretation in exact message evidence and keeps perspectives distinct.
5. Remains useful as a deterministic raw structure when local inference is unavailable.
6. Starts privately and can release a reviewed subset into a consented shared field.
7. Allows both participants to affirm, contest, correct, or resolve shared units.
8. Never sends a message or shares field content without explicit human action.

The causal loop is:

`Messages -> grounded provisional field -> perceptible feedback -> improved noticing/repair/coordination -> new messages -> revised field`

## Acceptance Criteria

### M0 — Control plane

- Purpose, non-goals, architecture, risks, research dispositions, threat model, runbook, and roadmap contain no placeholders.
- Global foundation and winning-definition audits pass.
- Every selected upstream dependency has a licence and reuse disposition.
- The private GitHub-ready repository contains no private transcript or secret.

### M1 — Replayable living field

- A fixture player replays at least 100 messages at conversational cadence.
- Now, Differences, Open loops, and Evolution lenses work without AI.
- Every visible node and edge resolves to valid evidence.
- At least 95% of unaffected nodes preserve identity and position across updates.
- Provisional, stable, contested, superseded, resolved, and retracted lifecycles are represented.
- The field is fully usable through keyboard-accessible outline mode.
- A browser verification records screenshots, interaction evidence, accessibility results, and console state.

### M2 — Semantic engine

- At least 90% evidence-supported semantic units.
- At least 95% correct speaker attribution.
- Zero automatic `jointly_ratified` classifications.
- Under 5% false-agreement errors.
- P95 semantic update below 10 seconds and peak total memory below 12 GB on the reference M4/16 GB Mac.

### M3 — Live private Beeper field

- New raw events appear within P95 1.5 seconds of receipt; semantic updates within P95 10 seconds.
- WebSocket disconnect, polling reconciliation, duplication, edits, deletion, and restart recovery pass.
- Beeper tokens and database keys never enter WebView state or logs.
- No per-message or per-turn mapping action is required.

### M4 — Energetic viability

- Nine real sessions across three consenting dyads.
- At least seven sessions surface one participant-rated useful development without a command.
- Median correction burden is no more than one gesture per 20 messages.
- No high-confidence unsupported interpretation reaches Now.
- Participants report reduced effort regaining conversational context.

### M5 — Consented sharing

- Desktop and two browser replicas converge after concurrent offline edits.
- Normal shared updates propagate within P95 two seconds.
- Relay inspection reveals no readable field or transcript text.
- Raw source content is absent unless covered by a release grant.
- Joint ratification requires both participants.

### M6 — MVP hardening

- Accessibility, security, recovery, export, deletion, performance, review, and packaging gates pass together in a fresh run.
- Public release remains a distinct explicit approval decision.

## Non-negotiable constraints

- Local-first; offline-capable private field; no cloud-model fallback.
- AI proposals remain visibly provisional and evidence-bound.
- Attention, understanding, agreement, and commitment remain distinct.
- No personality, diagnosis, hidden emotion, motive, or intent inference.
- Raw DM content never reaches a relay.
- No advertising, engagement manipulation, behavioural scoring, or automatic interpersonal action.
- Accessible outline representation accompanies the spatial map.
- Deleted source content is tombstoned and evidence-invalidated, not silently retained.

## Non-goals

- Replacing chat applications, autonomous mediation, generic mind-mapping, or truth adjudication.
- Group/channel deliberation, mobile-native clients, Windows/Linux, public publishing, or foundation-model training in MVP.

## Verification Evidence

The repository-wide command is `pnpm verify`. Milestone-specific evidence is recorded in `docs/REVIEW.md` and `docs/PROGRESS.md`; browser evidence is required for M1 and later UX gates. No milestone advances on tests alone when its acceptance criteria include behaviour, privacy, performance, accessibility, or real participant outcomes.

## Failure Modes

- A persuasive but unstable graph increases cognitive load.
- AI collapses perspectives or hallucinates agreement.
- Salience becomes intrusive or banal.
- A source message leaks into shared state.
- Beeper's experimental WebSocket changes or drops events.
- Local inference exceeds the latency or memory envelope.
- Sharing creates coercion or implies revocation can erase prior downloads.
- The team expands to groups before the dyadic loop is useful.

## Open decisions

No product decisions block M0 or M1. The local model and semantic pipeline are selected mechanically by the M2 bake-off. Public release, production hosting, signing credentials, and real-pilot recruitment remain explicit later gates.
