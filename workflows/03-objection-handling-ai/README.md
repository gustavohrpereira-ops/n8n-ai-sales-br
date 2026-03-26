# WF-03 — Objection Handling with Claude AI

> Automatically handle common consórcio objections with intelligent, personalized responses.

## Overview

When a lead sends an objection via WhatsApp or CRM, this workflow captures it, analyzes the objection type with Claude, and generates a persuasive response addressing their specific concern.

## Trigger
- **Webhook** — triggered when a lead message contains objection keywords

## What Claude Does
- Classifies the objection (price, time, distrust, competition, urgency)
- Generates a tailored rebuttal in Brazilian Portuguese
- Includes specific consórcio benefits relevant to the objection
- Suggests next action for the broker

## Common Objections Handled
- "Consórcio é muito caro"
- "Prefiro financiamento"
- "Tenho medo de não ser contemplado"
- "Já tenho um consórcio"
- "Vou pensar melhor"

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
