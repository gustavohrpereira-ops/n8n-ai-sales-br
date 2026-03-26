# WF-04 — Proposal Generator with Claude AI

> Generate personalized consórcio proposals using Claude AI based on lead profile and goals.

## Overview

Receives lead data and automatically generates a complete, personalized consórcio proposal with the right product, parcel value, and investment justification — all written by Claude in professional Brazilian Portuguese.

## Trigger
- **Webhook** — triggered when lead is marked as ready for proposal

## What Claude Does
- Selects the most suitable consórcio product (imóvel/auto/serviço)
- Calculates recommended credit value based on lead's goals
- Writes a personalized proposal with compelling copy
- Includes ROI comparison vs financing
- Formats output as WhatsApp message or PDF-ready text

## Required Credentials
- Anthropic API Key (Claude)
- Webhook configuration

## How to Import
1. Open n8n
2. Click **Import from file**
3. Select `workflow.json` from this folder
4. Configure credentials
5. Activate the workflow

---
*Powered by [Claude AI](https://claude.ai) + [n8n](https://n8n.io)*
