# Prompt Engineering for Consórcio Sales

Este documento detalha as estratégias de prompt utilizadas para garantir que o Claude atue como um especialista sênior em consórcio brasileiro e como otimizar o uso de tokens para operações em larga escala.

---

## 🌟 Core Strategy: The "Top Broker" Persona

Todo prompt inicializa o Claude com uma persona de alta performance:
> "Você é o maior especialista em consórcio do Brasil, com 20 anos de experiência. Sua linguagem é profissional, persuasiva e ética. Você domina as regras do Banco Central (BACEN) e converte leads de financiamento para consórcio através de argumentos de ROI e educação financeira."

---

## 🚀 Otimização de Tokens e Performance (Escala Enterprise)

Com o objetivo de impactar **10.000+ assessores**, a eficiência de tokens é crítica. Implementamos as seguintes técnicas:

### 1. Prompt Caching (Anthropic Native)
Para workflows repetitivos (como Lead Qualification), estruturamos o prompt para que a parte estática (persona + instruções do produto) venha primeiro. Isso permite que a Anthropic aplique **Prompt Caching**, reduzindo o custo e a latência em chamadas subsequentes.

### 2. Estrutura XML para Redução de Verbocidade
Usamos tags XML (`<data>`, `<instruction>`) para que o Claude entenda a separação de contexto sem a necessidade de textos explicativos longos. Isso economiza ~15% de tokens por chamada.

### 3. Saída Determinística em JSON
Ao exigir `APENAS o JSON` no output, evitamos que o modelo gaste tokens com introduções ou conclusões desnecessárias ("Aqui está o seu JSON...").

---

## 🛠️ Workflows Específicos

### 1. Lead Qualification (WF-01)
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

### 2. Objection Handling (WF-03)
**Framework: Feel-Felt-Found AI-Driven**
O prompt instrui o Claude a identificar a dor emocional do cliente antes de apresentar a solução técnica (lance embutido, contemplação, etc.), maximizando a taxa de conversão.

---

*Powered by [Claude AI](https://claude.ai) + [n8n](https://n8n.io) 💜*
