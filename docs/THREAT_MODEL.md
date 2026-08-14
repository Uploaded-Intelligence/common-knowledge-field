# Threat Model

## Protected assets

- Message content and evidence excerpts.
- Participant identity and relationship topology.
- Beeper token, database key, model prompts, capability-link keys.
- Private judgments and unreleased field units.

## Adversaries and failures

- Malicious text attempting prompt injection.
- A leaked capability link.
- Relay or analytics operator inspecting payloads.
- WebView compromise reading privileged tokens.
- One participant coercing another to share or ratify.
- Accidental logging, crash dumps, exports, backups, or screenshots.
- Dependency compromise or upstream API drift.

## Controls

- Privileged secrets remain in the Tauri/Rust process and macOS Keychain.
- Model has no network, filesystem, messaging, or tool authority.
- Field proposals pass deterministic attribution, evidence, lifecycle, and visibility validation.
- Private and shared documents use different keys and storage.
- Capability keys remain in URL fragments and do not reach the relay.
- Relay stores opaque encrypted changes with retention limits and content-free metrics.
- Source content is sanitised before UI rendering.
- Release requires a preview and explicit action; jointness requires all parties.
- Local diagnostics are content-free; analytics are absent by default.

## Known residual risks

- Revocation cannot erase material already copied or downloaded.
- A private local analysis can still affect how one person perceives another.
- Exact relational safety cannot be guaranteed by technical controls; pilot feedback and conservative language remain required.

