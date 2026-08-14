# Architecture

## Trust boundaries

```text
Beeper Desktop --local HTTP/WS--> trusted Tauri host --> encrypted source ledger
                                              |
                                              v
                                    validated field patches
                                              |
                                   private Automerge document
                                              |
                            explicit release grant + bundle preview
                                              |
                                 encrypted shared document
                                              |
                                    opaque sync relay
```

The Tauri host owns Beeper credentials, database keys, source content, model execution, exports, and OS integration. Web UIs receive only narrowly scoped data. The relay receives encrypted Automerge changes and presence metadata, never source messages or decryption keys.

## Monorepo units

- `apps/desktop`: React UI and Tauri host.
- `apps/field-web`: shared-field PWA.
- `apps/relay`: opaque Automerge WebSocket relay.
- `packages/field-schema`: canonical types, validation, lifecycle, visibility, release grants.
- `packages/field-engine`: incremental identity, patch application, evidence validation, salience.
- `packages/field-ui`: stable React Flow projection and accessible outline.
- `packages/fixtures`: consent-safe replay corpus and player.
- `packages/evaluation`: semantic and performance scoring.

## State separation

1. `SourceEvent`: immutable local message event with edit/delete lineage.
2. `FieldPatchProposal`: untrusted machine proposal.
3. `AcceptedFieldRevision`: validator-approved append-only transition.
4. `PrivateField`: local Automerge projection.
5. `FieldBundleV1`: explicitly released subset and evidence excerpts.
6. `SharedField`: encrypted participant-governed Automerge document.

## Runtime degradation

- Model absent: deterministic topics/replies/questions and replay remain available.
- Beeper absent: fixture/import mode remains available.
- WebSocket absent: bounded polling reconciles.
- Relay absent: shared edits queue locally and encrypted bundle export remains available.

