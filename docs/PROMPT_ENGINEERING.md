# Prompt Engineering for Consórcio Sales

[English](#english) | [Português](#português)

---

<a name="english"></a>
## English Version

This document details the prompt strategies used to ensure that Claude acts as a senior specialist in Brazilian consórcio and how to optimize token usage for large-scale operations.

---

### 🌟 Core Strategy: The "Top Broker" Persona

Every prompt initializes Claude with a high-performance persona:
> "You are the leading consórcio specialist in Brazil, with 20 years of experience. Your language is professional, persuasive, and ethical. You master the rules of the Central Bank (BACEN) and convert financing leads to consórcio through ROI arguments and financial education."

---

### 🚀 Token & Performance Optimization (Enterprise Scale)

With the goal of impacting **10,000+ advisors**, token efficiency is critical. We implement the following techniques:

#### 1. Prompt Caching (Anthropic Native)
For repetitive workflows (like Lead Qualification), we structure the prompt so the static part (persona + product instructions) comes first. This allows Anthropic to apply **Prompt Caching**, reducing cost and latency in subsequent calls.

#### 2. XML Structure for Verbosity Reduction
We use XML tags (`<data>`, `<instruction>`) so Claude understands the context separation without the need for connective filler text, saving tokens per interaction.

#### 3. Deterministic JSON Output
By requiring `ONLY the JSON` in the output, we prevent the model from spending tokens on unnecessary introductions or conclusions ("Here is the result..."), which is vital for automated processing.

---

### 🛠️ Specific Workflows

#### 1. Lead Qualification (WF-01)
**Prompt Structure:**
```text
<system_context>
Persona: Top Broker
Rules: Score 0-100, Categories Hot/Warm/Cold
</system_context>
<lead_data>
Name: {{ $json.name }}
Message: {{ $json.message }}
</lead_data>
<instruction>
Return a JSON with: { "score": int, "category": string, "reasoning": string }
</instruction>
```

#### 2. Objection Handling (WF-03)
**Framework: Feel-Felt-Found AI-Driven**
The prompt instructs Claude to identify the client's emotional pain before presenting the technical solution, ensuring a highly humanized and persuasive interaction.

---

<a name="português"></a>
## Versão em Português

Este documento detalha as estratégias de prompt utilizadas para garantir que o Claude atue como um especialista sênior em consórcio brasileiro e como otimizar o uso de tokens para operações em larga escala.

---

### 🌟 Estratégia Central: Persona "Top Broker"

Todo prompt inicializa o Claude com uma persona de alta performance:
> "Você é o maior especialista em consórcio do Brasil, com 20 anos de experiência. Sua linguagem é profissional, persuasiva e ética. Você domina as regras do Banco Central (BACEN) e converte leads de financiamento para consórcio através de argumentos de ROI e educação financeira."

---

### 🚀 Otimização de Tokens e Performance (Escala Enterprise)

Com o objetivo de impactar **10.000+ assessores**, a eficiência de tokens é crítica. Implementamos as seguintes técnicas:

#### 1. Prompt Caching (Anthropic Native)
Para workflows repetitivos (como Lead Qualification), estruturamos o prompt para que a parte estática (persona + instruções do produto) venha primeiro. Isso permite que a Anthropic aplique **Prompt Caching**, reduzindo o custo e a latência em chamadas subsequentes.

#### 2. Estrutura XML para Redução de Verbocidade
Usamos tags XML (`<data>`, `<instruction>`) para que o Claude entenda a separação de contexto sem a necessidade de textos explicativos longos, economizando tokens por interação.

#### 3. Saída Determinística em JSON
Ao exigir `APENAS o JSON` no output, evitamos que o modelo gaste tokens com introduções ou conclusões desnecessárias, o que é vital para o processamento automatizado.

---

### 🛠️ Workflows Específicos

#### 1. Lead Qualification (WF-01)
**Estrutura do Prompt:**
```text
<system_context>
Persona: Top Broker
Regras: Score 0-100, Categorias Hot/Warm/Cold
</system_context>
<lead_data>
Nome: {{ $json.name }}
Mensagem: {{ $json.message }}
</lead_data>
<instruction>
Retorne um JSON com: { "score": int, "category": string, "reasoning": string }
</instruction>
```

#### 2. Objection Handling (WF-03)
**Framework: Feel-Felt-Found AI-Driven**
O prompt instrui o Claude a identificar a dor emocional do cliente antes de apresentar a solução técnica, garantindo uma interação altamente humanizada e persuasiva.

---
*Optimized for Claude 3.5 Sonnet*
