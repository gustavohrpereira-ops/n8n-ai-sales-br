# WF-05 — Customer Segmentation with Claude AI

> Intelligently segment your consórcio leads into buyer personas using Claude AI analysis.

## Overview

Processes your lead database on a weekly schedule and uses Claude to classify each lead into a buyer persona based on their profile, behavior, and interactions — enabling more targeted and effective marketing.

## Trigger
- **Cron** — runs weekly to process and update lead segments

## What Claude Does
- Analyzes lead data (income, goals, behavior, source)
- Assigns buyer persona (Investor, First Home Buyer, Upgrader, etc.)
- Generates a segmentation rationale in Portuguese
- Recommends communication approach for each segment

## Output Segments
- 🔥 **Investidor** — high intent, multiple quotas
- 🏠 **Primeiro Imóvel** — emotional, needs education
- 🚗 **Auto Comprador** — vehicle-focused, price sensitive
- ❄️ **Frio** — needs long-term nurturing

## Required Credentials
- Anthropic API Key (Claude)
- Database/CRM connection

## How to Import
1. Open n8n
2. Click **Import from file**
3. Select `workflow.json` from this folder
4. Configure credentials
5. Activate the workflow

---
*Powered by [Claude AI](https://claude.ai) + [n8n](https://n8n.io)*
