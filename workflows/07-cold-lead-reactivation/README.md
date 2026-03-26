# WF-07 — Cold Lead Reactivation ❄️

Workflow para reativar leads que não interagem há algum tempo (entre 30 e 180 dias).

## Visão Geral
Este sistema identifica leads "frios" no CRM e utiliza o Claude AI para gerar uma mensagem de reengajamento altamente personalizada baseada no histórico anterior do lead, aumentando as chances de retorno.

## Gatilho (Trigger)
- Cron/Schedule: Execução semanal ou quinzenal.

## Como Usar
1. Importe o `workflow.json`.
2. Configure o filtro de data no seu CRM (ex: Pipedrive) para selecionar leads sem atividade há >30 dias.
3. Personalize o prompt do Claude na pasta `/prompts` se necessário.
