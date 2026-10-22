---
description: "iosys organization conventions and standards"
---

# Organization Conventions

Follow these conventions when working in iosys repositories.

## Repository Naming
- Client projects: `client-{clientname}-{project}` (e.g., `client-acme-webshop`)
- Internal projects: `{product-name}` (e.g., `invoicing-saas`)

## Labels
Work is tracked in Linear. Labels and fields come from the existing Linear taxonomy in `linear_taxonomy` (see `CONVENTIONS.yaml`).
- **Category** (one per implementation ticket): `Bug`, `Feature`, `Improvement`, `Research`
- **Priority**: native Linear priority 0-4 (0 = No priority, Backlog only; Ready needs 1-4), not a label
- **Estimate**: native Linear points, not a label
- **Other existing labels**: `Blocked`; `Task`, `follow-up`, `agent-authored` only where the target team has them. Availability differs by team: verify before applying.

Do not create, rename, or retire labels. Team availability varies: verify a label exists on the team before applying it.

## Definition of Ready
An implementation ticket is ready when it has exactly one Category label, a native priority set to 1-4, a native estimate when the team scale is verified, and clear requirements. Meeting follow-up tasks (no Category label) are exempt and are not Ready until triaged.

## Branching
- **Trunk-based development**: Work on `main`
- **Dev deployment**: Push to `main` → deploys to dev
- **Prod deployment**: Create tag `v{MAJOR}.{MINOR}.{PATCH}` → deploys to prod
- **Versioning**: Semantic versioning (semver)

## Creating Issues
Create work items in Linear, not GitHub. The `gh issue create` examples with `type:` labels in `issue_templates` in `CONVENTIONS.yaml` are GitHub-only, use GitHub-side labels (`github_labels`), and are not Linear labels.

## Tech Stack
- **Cloud**: Azure (IoT Hub, Databricks, Functions)
- **Languages**: Python, TypeScript, C#
- **Data**: Time series, OPC-UA, MQTT
- **Frontend**: React, Next.js

See `CONVENTIONS.yaml` for full machine-readable specifications.
