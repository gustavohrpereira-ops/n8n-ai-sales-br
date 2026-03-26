# WF-07 — Competitive Analysis with Claude AI

> Monitor competitors and generate strategic insights for consórcio positioning.

## Overview

This workflow gathers market data and competitor information, then uses Claude to generate a strategic competitive analysis with actionable positioning recommendations for the broker.

## Trigger
- **Cron** — runs monthly or on-demand via webhook

## What Claude Does
- Analyzes competitor pricing and positioning
- Identifies market opportunities in the consórcio space
- Generates a competitive positioning brief in Portuguese
- Recommends differentiation strategies
- Highlights advantages of consórcio vs financing for specific segments

## Output
- Competitive intelligence report
- Positioning recommendations
- Talking points for the broker to use in sales conversations

## Required Credentials
- Anthropic API Key (Claude)
- HTTP Request node (for market data)

## How to Import
1. Open n8n
2. Click **Import from file**
3. Select `workflow.json` from this folder
4. Configure credentials
5. Activate the workflow

---
*Powered by [Claude AI](https://claude.ai) + [n8n](https://n8n.io)*
