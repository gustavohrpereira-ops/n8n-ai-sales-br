# WF-02 — WhatsApp Follow-up Automation

> Send personalized WhatsApp follow-up messages crafted by Claude AI based on lead profile.

## Overview

This workflow runs on a cron schedule to identify leads that need follow-up and generates personalized WhatsApp messages using Claude AI. Each message is unique and tailored to the lead's profile, interest, and stage in the sales funnel.

## Trigger
- **Cron** — runs every 24 hours to check for pending follow-ups

## What Claude Does
- Analyzes lead profile and previous interactions
- Generates a personalized follow-up message in Brazilian Portuguese
- Adapts tone based on lead temperature (Hot/Warm/Cold)
- Creates urgency and value proposition specific to consórcio

## Output
- WhatsApp message ready to send (via Evolution API or Z-API)
- Follow-up scheduled for next touchpoint
- CRM status update

## Required Credentials
- Anthropic API Key (Claude)
- WhatsApp API credentials (Evolution API / Z-API / Twilio)
- CRM or database connection

## How to Import
1. Open n8n
2. Click **Import from file**
3. Select `workflow.json` from this folder
4. Configure credentials
5. Set cron schedule (default: daily at 9am BRT)
6. Activate the workflow

## Connected Workflows
- ← **WF-01** Lead Qualification (triggers this workflow for Hot leads)
- → **WF-03** Objection Handling

---
*Powered by [Claude AI](https://claude.ai) + [n8n](https://n8n.io)*
