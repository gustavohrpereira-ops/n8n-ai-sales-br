# n8n-ai-sales-br
I built 5 free AI sales automation workflows for n8n — powered by Claude (open source 🇧🇷
<div align="center">

# 🤖 n8n-ai-sales-br

### Open-source AI-powered sales automation workflows for the Brazilian market
### Automação de vendas com IA para consórcio, imóveis e CRM no Brasil

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![n8n](https://img.shields.io/badge/n8n-compatible-orange)](https://n8n.io)
[![Claude](https://img.shields.io/badge/Powered%20by-Claude%20AI-blueviolet)](https://claude.ai)
[![Stars](https://img.shields.io/github/stars/SEU-USER/n8n-ai-sales-br?style=social)]()
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

**🇧🇷 [Português](#-português) | 🇺🇸 [English](#-english)**

![Demo GIF](assets/demo.gif)

</div>

---

## 🇧🇷 Português

### O Problema

O mercado de consórcio e imóveis no Brasil movimenta **+R$500 bilhões/ano**, mas ainda opera com processos manuais: planilhas, follow-ups perdidos, propostas feitas na mão e leads sem qualificação inteligente. **Este projeto resolve isso.**

### O Que É

Uma coleção de **workflows prontos para n8n** que automatizam todo o ciclo de vendas usando Claude AI como motor de inteligência. Funciona para:

- 🏠 Corretores de imóveis e imobiliárias
- 📋 Vendedores e gestores de consórcio
- 🤝 Correspondentes bancários e brokers
- 📊 Times de CRM e inside sales

### ⚡ Workflows Disponíveis

| # | Workflow | O que faz | Tempo economizado |
|---|----------|-----------|------------------|
| 01 | Lead Qualification | Classifica leads por potencial com Claude | ~3h/dia |
| 02 | WhatsApp Follow-up | Follow-up automático e personalizado | ~2h/dia |
| 03 | Proposal Generator | Gera propostas em PDF automaticamente | ~1h/lead |
| 04 | CRM Enrichment | Enriquece dados de leads via IA | ~4h/semana |
| 05 | AI Sales Report | Relatórios automáticos com insights | ~3h/semana |

### 🚀 Quick Start (5 minutos)

\`\`\`bash
# 1. Clone o repositório
git clone https://github.com/SEU-USER/n8n-ai-sales-br.git

# 2. Configure suas credenciais
cp templates/env.example .env
# Edite .env com sua ANTHROPIC_API_KEY e demais tokens

# 3. Importe o workflow no n8n
# Vá em n8n > Import > selecione o arquivo workflow.json desejado
\`\`\`

### 📋 Pré-requisitos

- [n8n](https://n8n.io) (self-hosted ou cloud)
- [Claude API Key](https://console.anthropic.com) (Anthropic)
- WhatsApp Business API (opcional, para workflows 01 e 02)
- Google Sheets ou Airtable (opcional, para CRM)

---

## 🇺🇸 English

### What Is This

A collection of **production-ready n8n workflows** powering AI-driven sales automation, built specifically for the Brazilian consórcio and real estate markets — but fully adaptable to any sales team globally.

Claude AI (Anthropic) is the core intelligence engine across all workflows, handling lead scoring, personalized messaging, proposal generation, and sales insights.

### Why It Matters

Brazil has one of the world's most complex and underserved sales automation landscapes. This project brings enterprise-grade AI workflows to individual brokers and SMBs through open-source tooling — closing the gap between large players and independent professionals.

### 🤝 Contributing

All contributions are welcome! See [CONTRIBUTING.md](CONTRIBUTING.md).
Found a bug? [Open an issue](.github/ISSUE_TEMPLATE/bug_report.md).
Want a new workflow? [Request it](.github/ISSUE_TEMPLATE/workflow_request.md).

---

<div align="center">

Built with ❤️ in Brazil 🇧🇷 | Powered by [Claude AI](https://claude.ai) + [n8n](https://n8n.io)

**Se este projeto ajudou você, deixe uma ⭐ — isso mantém o projeto vivo!**

</div>
