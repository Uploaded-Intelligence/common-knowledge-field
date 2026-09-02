# Runbook

## Supported development host

- macOS 15.6 or later on Apple Silicon.
- Node.js 24 LTS for CI/release; the current workstation has Node 26.4.0.
- pnpm via Corepack.
- Rust stable and Xcode Command Line Tools once the Tauri host begins.

## Standard commands

```bash
pnpm install --frozen-lockfile
pnpm test
pnpm typecheck
pnpm lint
pnpm build
pnpm verify
```

## Diagnostics

- Local diagnostics contain event IDs, counts, timings, model/schema versions, and error categories only.
- Never log message content, evidence excerpts, Beeper tokens, database keys, capability keys, or decrypted CRDT payloads.
- If inference fails, confirm deterministic raw structure still updates before investigating the model.
- If WebSocket ingestion fails, run polling reconciliation and compare source event IDs before reconnecting.

## Backup and recovery

- Private source state is encrypted and append-only with tombstones.
- Backup/restore tests must include SQLite WAL and SHM behaviour.
- Restore never overwrites an existing target.
- Export and deletion evidence must include filesystem inspection.

## Deployment and rollback

- The source repository may be public under D-009. No production/public application deployment or publication of conversation fields is authorised.
- Pilot builds are signed only after explicit credential approval.
- Each subsystem is feature-gated: semantic inference, Beeper live ingestion, sharing, and relay can be disabled independently.
