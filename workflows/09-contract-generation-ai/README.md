# WF-09 — Contract Generation with Claude AI

> Automatically draft consórcio contracts using Claude AI based on approved proposals.

## Overview

Once a lead accepts a proposal, this workflow generates a complete, legally-formatted consórcio contract draft using Claude, pre-populated with all client and product information.

## Trigger
- **Webhook** — triggered when lead status changes to "Proposal Accepted"

## What Claude Does
- Fills in contract template with client and product data
- Drafts the terms and conditions summary in plain Portuguese
- Generates a personalized cover letter
- Flags any missing required information
- Creates both formal (legal) and simplified (client-friendly) versions

## Output
- Contract draft (PDF-ready text or Google Doc)
- Client cover letter
- Internal checklist for broker
- Notification sent to client via WhatsApp

## Required Credentials
- Anthropic API Key (Claude)
- Webhook configuration
- Google Drive or PDF generation node (optional)

## How to Import
1. Open n8n
2. Click **Import from file**
3. Select `workflow.json` from this folder
4. Configure credentials
5. Activate the workflow

---
*Powered by [Claude AI](https://claude.ai) + [n8n](https://n8n.io)*
