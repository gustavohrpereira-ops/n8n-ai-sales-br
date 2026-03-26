# WF-01 — Lead Qualification with Claude AI

> Automatically qualify and score incoming leads using Claude as the intelligence engine.

## 🇧🇷 PT-BR | 🇺🇸 EN

---

## Overview

This workflow receives leads via webhook, analyzes them with Claude AI, and assigns a qualification score (0-100) based on consórcio sales criteria. High-scoring leads are immediately routed for priority follow-up.

## Trigger
- **Webhook** — receives lead data from landing pages, CRM, or WhatsApp forms

## What Claude Does
- Analyzes lead intent, budget signals, and urgency
- Scores lead 0-100 based on consórcio-specific criteria
- Generates a qualification summary in Portuguese
- Recommends next action (call now / nurture / discard)

## Output
- Lead score + category (Hot / Warm / Cold)
- Qualification notes for the broker
- Automatic routing to appropriate follow-up workflow

## Required Credentials
- Anthropic API Key (Claude)
- Webhook URL configuration

## How to Import
1. Open n8n
2. Click **Import from file**
3. Select `workflow.json` from this folder
4. Configure your Anthropic API credentials
5. Activate the workflow

## Input Payload Example
```json
{
  "name": "João Silva",
  "phone": "+55 31 99999-0000",
  "interest": "consórcio imóvel 500k",
  "source": "instagram",
  "message": "Quero saber mais sobre consórcio"
}
```

## Connected Workflows
- → **WF-02** WhatsApp Follow-up (for Hot leads)
- → **WF-05** Customer Segmentation

---
*Powered by [Claude AI](https://claude.ai) + [n8n](https://n8n.io)*
