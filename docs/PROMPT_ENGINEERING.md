# Prompt Engineering for Consórcio Sales

This document details the specific prompt strategies used across the 10 n8n workflows to ensure Claude performs as a top-tier Brazilian consórcio broker.

---

## Core Strategy: The "Top Broker" Persona

Every prompt initializes Claude with a high-performance persona:
> "Você é o maior especialista em consórcio do Brasil, com 20 anos de experiência na Ademicon. Sua linguagem é profissional, persuasiva, mas extremamente ética. Você conhece todas as regras do Banco Central (BACEN) e sabe como converter leads de financiamento para consórcio usando argumentos de ROI e educação financeira."

---

## 1. Workflow: Lead Qualification (WF-01)

### The Prompt Structure
We use structural XML-like tagging to separate data from instructions:

```text
<lead_data>
Nome: {{ $json.name }}
Interesse: {{ $json.interest }}
Mensagem: {{ $json.message }}
</lead_data>

<instructions>
Analise os dados acima e atribua um score de 0-100 baseado em:
1. Intencionalidade de compra
2. Urgência
3. Ticket médio estimado
</instructions>

Retorne APENAS um JSON válido.
```

---

## 2. Workflow: Objection Handling (WF-03)

### Strategic Rebuttal Framework
We implement the **Feel-Felt-Found** variant:

```text
Identifique a objeção nesta mensagem: "{{ $json.message }}"

Framework de resposta:
1. Validar (Eu entendo como você se sente...)
2. Normalizar (Muitos dos meus clientes sentiram o mesmo...)
3. Resolver (Mas o que eles descobriram foi que o lance embutido...)

Gere a resposta em Português do Brasil, tom consultivo.
```

---

## Why Claude?

After testing several models, Claude 3.5 Sonnet was selected for:
1. **Financial Nuance**: Correctly uses terms like "taxa de administração" vs "juros".
2. **Safety**: Never guarantees contemplação (illegal by BACEN rules).
3. **Reasoning**: Can calculate ROI comparisons inside the prompt.

---

*Powered by [Claude AI](https://claude.ai) + [n8n](https://n8n.io) 💜*
