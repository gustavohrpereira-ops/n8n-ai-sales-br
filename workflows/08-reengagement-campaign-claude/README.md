# WF-08 — Re-engagement Campaign with Claude AI

> Automatically re-engage cold leads with AI-crafted personalized messages.

## Overview

Identifies leads that went cold (no response in 30+ days) and uses Claude to craft personalized re-engagement messages that reignite interest with a fresh angle.

## Trigger
- **Cron** — runs twice a week to identify and re-engage cold leads

## What Claude Does
- Analyzes why the lead went cold (last interaction context)
- Creates a new compelling re-engagement angle
- Writes a personalized message referencing their original interest
- Includes a new value hook or market insight
- Adjusts urgency based on how long the lead has been cold

## Output
- Re-engagement message via WhatsApp
- Lead status updated to "Re-engaged" or "Archived"
- Re-engagement analytics report

## Required Credentials
- Anthropic API Key (Claude)
- WhatsApp API
- CRM/Database connection

## How to Import
1. Open n8n
2. Click **Import from file**
3. Select `workflow.json` from this folder
4. Configure credentials
5. Activate the workflow

---
*Powered by [Claude AI](https://claude.ai) + [n8n](https://n8n.io)*
