<div align="center">

# 🤖 n8n-ai-sales-br

### Open-source AI-powered sales automation workflows for the Brazilian market
### Automação de vendas com IA para consórcio, imóveis e CRM no Brasil

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![n8n](https://img.shields.io/badge/n8n-compatible-orange)](https://n8n.io)
[![Claude](https://img.shields.io/badge/Powered%20by-Claude%20AI-blueviolet)](https://claude.ai)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Workflows](https://img.shields.io/badge/workflows-10-blue)](workflows/)

**🇧🇷 [Português](#-português) | 🇺🇸 [English](#-english)**

</div>

---

## 🇧🇷 Português

### O Problema

O mercado de consórcio e imóveis no Brasil movimenta **+R$500 bilhões/ano** com **8 milhões+ de participantes ativos**, mas ainda opera com processos manuais: planilhas, follow-ups perdidos, propostas feitas na mão e leads sem qualificação inteligente. **Este projeto resolve isso.**

### O Que É

Uma coleção de **10 workflows prontos para n8n** que automatizam todo o ciclo de vendas usando Claude AI como motor de inteligência. Funciona para:

- 🏠 Corretores de imóveis e imobiliárias
- 📋 Vendedores e gestores de consórcio
- 🤝 Correspondentes bancários e brokers
- 📊 Times de CRM e inside sales

### ⚡ 10 Workflows Disponíveis

| # | Workflow | O que faz | Tempo economizado |
|---|----------|-----------|------------------|
| 01 | Lead Qualification | Classifica leads HOT/WARM/COLD com Claude | ~3h/dia |
| 02 | WhatsApp Follow-up | Follow-up automático e personalizado | ~2h/dia |
| 03 | Proposal Generator | Gera propostas HTML/PDF automaticamente | ~1h/lead |
| 04 | CRM Enrichment | Enriquece dados de leads via IA + CNPJ | ~4h/semana |
| 05 | AI Sales Report | Relatórios semanais com insights de IA | ~3h/semana |
| 06 | Client Onboarding | Boas-vindas personalizada ao novo cliente | ~30min/cliente |
| 07 | Cold Lead Reactivation | Reactiva leads frios (30-180 dias) | ~2h/semana |
| 08 | Objection Handler FAQ | Responde objeções e perguntas com IA | ~1h/dia |
| 09 | Contemplation Notification | Notifica e orienta cliente contemplado | ~45min/evento |
| 10 | Referral Pipeline | Automatiza programa de indicações | ~3h/semana |

### 🚀 Quick Start (5 minutos)

```bash
# 1. Clone o repositório
git clone https://github.com/gustavohrpereira-ops/n8n-ai-sales-br.git

# 2. Configure suas credenciais
cp templates/env.example .env
# Edite .env com sua ANTHROPIC_API_KEY e demais tokens

# 3. Importe o workflow no n8n
# Vá em n8n > Import > selecione o arquivo workflow.json desejado
```

### 📋 Pré-requisitos

- [n8n](https://n8n.io) (self-hosted ou cloud)
- [Claude API Key](https://console.anthropic.com) (Anthropic)
- WhatsApp Business API (opcional, para workflows 02)
- Google Sheets (opcional, para CRM)

---

## 🇺🇸 English

### What Is This

A collection of **10 production-ready n8n workflows** powering AI-driven sales automation, built specifically for the Brazilian consórcio and real estate markets.

Claude AI (Anthropic) is the **core intelligence engine** across all 10 workflows, handling lead scoring, personalized messaging, proposal generation, objection handling, and sales insights.

### Why It Matters

Brazil’s consórcio market is the **largest in the world** — a R$500B/year sector with 8M+ active participants and **zero modern AI tooling**. This project brings enterprise-grade AI workflows to 50,000+ individual brokers and SMBs through open-source tooling.

---

## 💜 Built with Claude AI

> This project is part of a larger **Claude-powered ecosystem** being built for the Brazilian financial and real estate market.

### What’s Already Built with Claude

| Product | Status | Description |
|---------|--------|-------------|
| **These 10 Workflows** | ✅ Live | Full sales cycle automation for consórcio |
| **Financial Dashboard (SaaS)** | 🔧 Phase 1 Complete | Claude-powered financial analysis and reporting for brokers |
| **Business Website** | ✅ Live | Built and refined entirely with Claude |

### What’s Coming (Roadmap)

| Product | Status | Description |
|---------|--------|-------------|
| **Financial Dashboard Phase 2** | 🚧 In Progress | Multi-tenant SaaS, payment processing, automated reports |
| **5 Conversion Landing Pages** | 🚧 Planned | Claude-generated pages for consórcio verticals (real estate, vehicles, services, travel, equipment) |
| **Full SaaS Launch** | 🚧 Planned | Targeting 50,000+ brokers in Brazil |

### Why Claude is Central

Every single workflow in this repository makes **direct API calls to Claude**. Claude is not a helper — it **is** the product:

- 🧠 **Lead intelligence**: scoring, classification, profile inference
- ✍️ **Content generation**: proposals, messages, reports, objection responses
- 📊 **Analysis**: sales metrics interpretation, recommendations
- 🎁 **Relationship automation**: onboarding, contemplation alerts, referrals

This open-source project is the foundation for a **Claude-native SaaS platform** serving the Brazilian consórcio industry.

---

## 🌎 Impact

- 🇧🇷 **Market size**: R$500B/year, 8M+ active participants
- 👥 **Target users**: 50,000+ brokers currently using spreadsheets
- 📱 **Primary channel**: WhatsApp (200M+ Brazilian users)
- 🤖 **AI penetration today**: Near zero — this project changes that
- 🇺🇸 **Language gap**: First major open-source AI sales toolkit in Portuguese for this sector

---

## 🤝 Contributing

All contributions are welcome! See [CONTRIBUTING.md](CONTRIBUTING.md).

Found a bug? [Open an issue](../../issues/new).
Want a new workflow? [Request it](../../issues/new).

---

<div align="center">

Built with ❤️ in Brazil 🇧🇷 | Powered by [Claude AI](https://claude.ai) + [n8n](https://n8n.io)

**Se este projeto ajudou você, deixe uma ⭐ — isso mantém o projeto vivo!**

</div>
