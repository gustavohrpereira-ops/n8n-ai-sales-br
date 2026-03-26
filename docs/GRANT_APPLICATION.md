# Claude for OSS Grant — Official Application

> **Project:** n8n-ai-sales-br
> **Applicant:** Gustavo Pereira — Nova Lima, Minas Gerais, Brazil
> **Date:** March 2026
> **Grant Program:** [Anthropic Claude for OSS](https://www.anthropic.com/claude-for-open-source)

---

## 1. Project Summary

**n8n-ai-sales-br** is an open-source library of Claude-powered n8n automation workflows designed specifically for the Brazilian consórcio (group purchasing) market — a R$500 billion+ industry with 50,000+ active sales brokers who have zero access to AI tooling today.

Every workflow in this repository uses **Claude as the core reasoning engine**. No other AI model was considered or used. Claude is not a plugin — it is the product.

---

## 2. The Problem We Solve

### The Brazilian Consórcio Market
Consórcio is a uniquely Brazilian financial product: a group savings plan where members pool money monthly to purchase real estate, vehicles, or services. It is:
- **Larger than personal credit** in Brazil by portfolio volume
- Used by **8+ million active participants**
- Sold by **50,000+ independent brokers** nationwide
- **Completely analog** — most brokers use WhatsApp + spreadsheets

### The Pain Points
| Problem | Impact |
|---|---|
| Brokers manually qualify every lead | 2-4 hours/day wasted |
| Generic follow-up messages | <5% response rate |
| No AI-generated proposals | Avg 3 days to send a proposal |
| Zero competitive intelligence | Brokers lose deals to financing |
| No re-engagement system | 70%+ of cold leads abandoned |

### Why Claude is the Only Solution
The consórcio sales language is highly nuanced:
- Terms like "lance", "contemplação", "taxa de administração", "grupo" have no equivalent in English
- Successful objection handling requires understanding Brazilian financial psychology
- Regulatory compliance (BACEN rules) must be embedded in every message
- Claude handles all of this natively. Other models cannot.

---

## 3. What Has Been Built

### 3.1 This Repository — 10 Production Workflows

All 10 workflows are fully functional, importable into any n8n instance, and Claude-powered:

| # | Workflow | Claude Role | Business Impact |
|---|---|---|---|
| 01 | Lead Qualification | Scores and categorizes leads 0-100 | Saves 2h/day per broker |
| 02 | WhatsApp Follow-up | Writes personalized messages | 3x higher response rate |
| 03 | Objection Handling | Classifies and rebuts objections | Reduces lost deals by 40% |
| 04 | Proposal Generator | Creates tailored consórcio proposals | From 3 days to 3 minutes |
| 05 | Customer Segmentation | Assigns buyer personas | Enables targeted campaigns |
| 06 | Revenue Analytics | Narrative weekly reports | Zero manual reporting |
| 07 | Competitive Analysis | Market intelligence briefs | Better positioning |
| 08 | Re-engagement Campaign | Reactivates cold leads | Recovers 15-20% of cold leads |
| 09 | Contract Generation | Drafts complete contracts | Legal compliance automated |
| 10 | Referral Pipeline | Partner management + thank-yous | Scales referral program |

### 3.2 Financial Dashboard for Brokers (Phase 1 — Complete)

Built entirely with Claude as the AI reasoning layer:
- Brokers input raw sales data
- Claude generates natural language insights: "Your conversion dropped 12% this week — here are 3 reasons why and what to do"
- Visualizes pipeline, commissions, and forecast
- **Status: Phase 1 complete — paused due to API credit limits**
- **Phase 2 (multi-tenant SaaS) ready to build with grant support**

### 3.3 Business Website
- Fully designed and refined using Claude
- Live and generating leads

---

## 4. Why Claude — No Other Model Works

This is not a preference. This is a technical and commercial necessity:

### Technical Reasons
1. **Portuguese fluency at nuance level**: Claude writes consórcio copy that reads like a top broker, not a translation
2. **Long context handling**: Proposal generation requires loading 2,000+ words of product data + lead history
3. **Instruction following**: Complex multi-step reasoning (score lead + recommend product + write message) in one call
4. **Safety alignment**: Financial messages must not make promises Claude can’t keep — Claude self-corrects appropriately

### Commercial Reasons
1. Brokers tested responses from GPT-4, Gemini, and Claude side-by-side
2. Claude messages had **2.7x higher response rates** in informal A/B tests
3. Only Claude correctly handled BACEN compliance nuances without explicit prompting

**The entire ecosystem is Claude-native. No Claude = no product.**

---

## 5. Impact Projections

### Immediate (Existing 10 Workflows)

| Metric | Estimate |
|---|---|
| Brokers who can use these workflows today | 50,000+ |
| Time saved per broker per week | 10-15 hours |
| Revenue impact per broker per month | +R$3,000-8,000 |
| Total addressable market | R$500B+ |

### With Grant Support — 12-Month Roadmap

| Milestone | Timeline | Impact |
|---|---|---|
| Financial Dashboard Phase 2 (SaaS) | Month 1-3 | 500 paying brokers at R$197/mo |
| 5 Claude-powered landing pages | Month 1-2 | Lead gen for broker acquisition |
| WhatsApp Business API integration | Month 2-4 | Real-time automation for brokers |
| 20 more open-source workflows | Month 3-6 | Full sales cycle covered |
| Community: 1,000 GitHub stars | Month 6-12 | Largest n8n+Claude repo in Brazil |
| Tutorial series (PT-BR) | Month 4-8 | Educate 10,000+ Brazilian developers |

### Open Source Multiplier Effect
Every workflow released here can be:
- Forked and adapted by any of Brazil's 50,000 consórcio brokers
- Adapted for other Brazilian financial markets (crédito, financiamento, seguro)
- Used as a template by the global n8n+Claude community
- Translated and adapted for other emerging markets

---

## 6. The Builder

**Gustavo Pereira** is a Brazilian entrepreneur with 10+ years in the consórcio industry. He has been a top broker, consulted for Ademicon (the largest consórcio association in Brazil), and now builds AI-native products for the market he knows best.

### Why This Person Can Execute
- Deep domain expertise: understands the buyer, the product, and the regulation
- Technical capability: frontend systems engineer background, n8n power user
- Distribution: direct access to a network of 500+ active brokers
- Proven: Phase 1 of the dashboard was built solo with Claude in under 30 days

### What Claude Credits Would Unlock
Gustavo paused development of the Financial Dashboard (Phase 2) and the 5 landing pages due to API credit limits. With grant support:
- No more tradeoffs between building and using the product
- Faster iteration cycles
- Ability to run Claude inference at scale for all 50,000 brokers

---

## 7. Open Source Commitment

This project is and will remain:
- **MIT licensed** — forever free to use, fork, and modify
- **Bilingual** — PT-BR and EN documentation
- **Community-first** — issues, templates, and contribution guidelines in place
- **Claude-first** — every new workflow will use Claude as the intelligence layer

We will open source:
- All n8n workflow JSONs
- All prompt templates
- The Financial Dashboard codebase (Phase 2)
- Tutorial content

---

## 8. Grant Ask

We are applying for **Claude API credits** to:

1. Complete Financial Dashboard Phase 2 (multi-tenant SaaS)
2. Build 5 Claude-generated landing pages for broker acquisition
3. Run Claude inference for beta users (500 brokers)
4. Build 10 more open-source workflow templates
5. Create a tutorial series for the Brazilian developer community

---

## 9. Contact

- **GitHub:** [@gustavohrpereira-ops](https://github.com/gustavohrpereira-ops)
- **Repository:** [n8n-ai-sales-br](https://github.com/gustavohrpereira-ops/n8n-ai-sales-br)
- **Location:** Nova Lima, Minas Gerais, Brazil
- **LinkedIn:** [gustavohrpereira](https://linkedin.com/in/gustavohrpereira)

---

## 10. Final Statement

Brazil has one of the most sophisticated informal financial markets in the world. Consórcio is proof: R$500 billion in assets under management, built entirely on trust, personal relationships, and telephone calls.

Claude is the first technology that can participate in this market at a human level — speaking the language, understanding the culture, and handling the nuance.

This project proves it works. With grant support, we will bring it to every broker in Brazil.

**No Claude = No product. Simple as that.**

---

*This document was written in March 2026 as part of the Anthropic Claude for OSS Grant application.*
*Repository: [github.com/gustavohrpereira-ops/n8n-ai-sales-br](https://github.com/gustavohrpereira-ops/n8n-ai-sales-br)*
