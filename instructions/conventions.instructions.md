---
description: "iosys organization conventions and standards"
---

# Organization Conventions

Follow these conventions when working in iosys repositories.

## Repository Naming
- Client projects: `client-{clientname}-{project}` (e.g., `client-acme-webshop`)
- Internal projects: `{product-name}` (e.g., `invoicing-saas`)

## Labels
Use these labels on issues:
- **Priority**: `priority: critical`, `priority: high`, `priority: medium`, `priority: low`
- **Type**: `type: bug`, `type: feature`, `type: process`, `type: other`
- **Size**: `size: xs` (<1h), `size: s` (<1d), `size: m` (1-3d), `size: l` (>3d)
- **Workflow**: `ready`, `blocked`, `help-wanted`

## Definition of Ready
An issue is ready to work on when it has:
- Type label
- Size label
- Priority label
- Clear requirements

## Branching
- **Trunk-based development**: Work on `main`
- **Dev deployment**: Push to `main` → deploys to dev
- **Prod deployment**: Create tag `v{MAJOR}.{MINOR}.{PATCH}` → deploys to prod
- **Versioning**: Semantic versioning (semver)

## Creating Issues
```bash
# Bug
gh issue create --title "[Bug]: description" --label "type: bug"

# Feature
gh issue create --title "[Feature]: description" --label "type: feature"
```

## Tech Stack
- **Cloud**: Azure (IoT Hub, Databricks, Functions)
- **Languages**: Python, TypeScript, C#
- **Data**: Time series, OPC-UA, MQTT
- **Frontend**: React, Next.js

See `CONVENTIONS.yaml` for full machine-readable specifications.
