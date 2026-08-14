# Common Knowledge Field MVP Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use `superpowers:subagent-driven-development` or `superpowers:executing-plans` task-by-task. Use test-driven development and fresh checkpoint review.

**Goal:** Deliver a verified local-first macOS companion that automatically turns a pinned Beeper DM into a stable, evidence-bound private field and can release a consented subset into a mutually governed shared field.

**Architecture:** A trusted Tauri/Rust host owns chat credentials, encrypted source storage, model execution, and OS integration. Shared TypeScript packages own the semantic contract, append-only field engine, Automerge document model, React Flow projection, PWA, fixtures, and evaluation. Raw source content never enters shared documents or the relay.

**Tech stack:** Tauri 2.11.4, Rust stable, React 19, strict TypeScript, pnpm monorepo, React Flow 12.11.3, Automerge Repo 2.5.6, Vitest, Playwright, SQLCipher, and a managed `llama.cpp`-compatible runner.

## Global constraints

- `docs/WINNING.md` is the acceptance contract.
- Production behaviour is test-first.
- AI proposals are untrusted, provisional, evidence-bound patches.
- Joint ratification is impossible without every participant's affirmative judgment.
- Beeper integration is read-only.
- Raw messages never enter shared state, relay payload plaintext, or logs.
- No cloud inference or public deployment.

## Task sequence

### Task 1 — M0 control plane

Create and verify the private GitHub-ready repository, canonical documents, licence ledger, threat model, CI, and implementation issue sequence. Commit only after foundation and winning checks pass.

### Task 2 — M1 field schema and replay contract

Write failing tests for evidence validation, lifecycle transitions, participant judgments, patch idempotency, and fixture replay. Implement the smallest canonical schema and a consent-safe 100-message fixture.

### Task 3 — M1 stable projection and lenses

Write browser/component tests for stable identity/position, the four lenses, maximum-three Now items, evidence navigation, and outline keyboard access. Implement a narrow docked UI and expanded view.

### Task 4 — M1 verification

Run unit, property, type, lint, build, browser, accessibility, performance, and visual checks. Record screenshots and results. Run spec and code-quality checkpoint reviews; resolve all blockers.

### Task 5 — M2 semantic bake-off

Build one shared evaluation interface and adapters for direct structured output, T3C-derived logic, LangExtract, and Graphiti. Evaluate the fixed local-model candidates against evidence, speaker, lifecycle, agreement, latency, and memory gates. Record a mechanical keep/reject decision.

### Task 6 — M3 trusted host and Beeper adapter

Create the Tauri host, Keychain secret boundary, SQLCipher append-only event ledger, generated/contract-tested Beeper read adapter, WebSocket ingestion, and polling reconciler. Verify duplicate, edit, delete, disconnect, and restart behaviour before connecting UI state.

### Task 7 — M3 managed inference and docked app

Package the winning local model behind a constrained host command. Add first-run model management, feature-gated semantic degradation, side-window behaviour, content-free diagnostics, performance traces, and recovery tests.

### Task 8 — M4 private pilot

Prepare consent materials and local-only pilot instrumentation. Run nine sessions across three dyads, score every M4 gate, and fix energetic-viability failures before sharing work begins.

### Task 9 — M5 release bundle and shared field

Write tests for release grants, evidence minimisation, `FieldBundleV1`, participant judgments, joint ratification, capability rotation, revocation, and export/delete. Implement the field PWA and encrypted opaque Automerge relay only after private usefulness is proven.

### Task 10 — M6 hardening and completion

Run the full security, accessibility, privacy, recovery, performance, packaging, PR-review, and end-to-end acceptance matrix. Produce a signed internal build only after credential approval. Public release remains separately gated.

## Checkpoint rule

Each task is complete only when its acceptance evidence is fresh, documented, reviewed, and traceable to `docs/WINNING.md`. A later task may not compensate for an earlier failed gate.

