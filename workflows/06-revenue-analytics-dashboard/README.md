# WF-06 — Revenue Analytics Dashboard

> Weekly AI-powered revenue report with Claude narrative insights for consórcio brokers.

## Overview

Every week, Claude analyzes your sales data and generates a comprehensive narrative report with performance insights, conversion analysis, and actionable recommendations — all in Portuguese.

## Trigger
- **Cron** — runs every Monday at 7am BRT

## What Claude Does
- Analyzes weekly sales metrics (leads, conversions, revenue)
- Identifies trends and anomalies
- Writes executive summary in Portuguese
- Generates 3 specific recommendations for the broker
- Compares performance against previous week

## Output
- Narrative report via WhatsApp or email
- JSON data for dashboard integration
- Recommended actions for the week

## Required Credentials
- Anthropic API Key (Claude)
- CRM / Google Sheets connection
- Email or WhatsApp API

## How to Import
1. Open n8n
2. Click **Import from file**
3. Select `workflow.json` from this folder
4. Configure credentials and data source
5. Activate the workflow

---
*Powered by [Claude AI](https://claude.ai) + [n8n](https://n8n.io)*
