# Security Policy

## Reporting a vulnerability

Please use GitHub's private vulnerability-reporting flow for this repository. Do not include sensitive findings, credentials, capability links, participant data, or real conversation content in a public issue or discussion.

Include the affected component and version or commit, impact, reproduction conditions using synthetic data, and any proposed mitigation. Maintainers will acknowledge the report through the private advisory thread and coordinate remediation there.

## Scope

Security-sensitive areas include:

- Beeper credentials and read-only source ingestion;
- encrypted local storage and key handling;
- evidence excerpts, participant identity, and relationship topology;
- model prompt injection and schema-validation boundaries;
- shared-field release grants, capability links, relay encryption, and revocation;
- logs, diagnostics, crash artefacts, exports, and deletion semantics.

The repository is public, but real conversation data and pilot environments are not public test targets. Do not attempt to access another person's messages, field, device, account, or relay data.
