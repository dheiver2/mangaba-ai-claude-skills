# Relatório Semanal de Atendimentos

Consolida todos os atendimentos da semana, identifica padrões e alerta sobre clientes em risco de churn.

## Frequência
**Semanal** — sugerido toda segunda-feira às 9h (revisando a semana anterior)

## Como agendar com Claude Code

```bash
# Criar agendamento toda segunda às 9h
claude schedule create \
  --name "relatorio-atendimentos" \
  --cron "0 9 * * 1" \
  --prompt-file atendimento/scheduled/relatorio-atendimentos.md \
  --output-format markdown
```

---

## Prompt

```
Você é o gerente de Customer Success da empresa [NOME_DA_EMPRESA].

Analise os atendimentos da semana de [DATA_INÍCIO] a [DATA_FIM]:

**VOLUME:**
- Total de atendimentos: [NÚMERO]
- Por canal: WhatsApp [X] | Email [X] | Telefone [X] | Chat [X]
- Atendimentos resolvidos: [NÚMERO]
- Atendimentos em aberto: [NÚMERO]
- Tempo médio de primeira resposta: [MINUTOS/HORAS]
- Tempo médio de resolução: [HORAS/DIAS]

**TIPOS DE SOLICITAÇÃO:**
[Ex:
- Dúvidas sobre uso: 45%
- Problemas técnicos: 25%
- Solicitações de cancelamento: 10%
- Reclamações: 8%
- Outros: 12%]

**SATISFAÇÃO (se coletada):**
- NPS médio da semana: [SCORE]
- CSAT médio: [SCORE]

**CASOS CRÍTICOS:**
[Liste clientes com problemas sérios ou que solicitaram cancelamento]

**SOLICITAÇÕES DE CANCELAMENTO:**
[Nome do cliente | Motivo | Status]

Gere:
1. Dashboard textual da semana (métricas principais)
2. Alerta de SLA: atendimentos que ultrapassaram o prazo ideal
3. Padrões identificados: O que os clientes mais estão precisando?
4. Clientes em risco de churn (com motivo e ação sugerida)
5. Quick wins: o que pode ser resolvido esta semana para melhorar a satisfação
6. Comparativo com semana anterior (se possível)
```

---

## Exemplo de saída

---
📊 **RELATÓRIO DE ATENDIMENTO — Semana 12-16/05/2025**

**Volume:** 87 atendimentos | 79 resolvidos (90,8%) | 8 em aberto  
**Tempo 1ª resposta:** 2h15min (meta: < 2h) 🟡  
**Tempo resolução:** 1,4 dias (meta: < 1 dia) 🔴  
**Satisfação:** NPS 72 🟢 | CSAT 4,1/5 🟢

⚠️ **Alertas SLA:** 3 tickets abertos há mais de 48h — #1042, #1055, #1061

📌 **Padrão da semana:** 34% dos contatos são dúvidas de onboarding. Sinal de que o material de boas-vindas não está claro.

🔴 **Risco de Churn (2 clientes):**
1. Empresa X — solicitou cancelamento por "falta de suporte rápido" → Acionar gerente de conta hoje
2. João ME — 3 reclamações nesta semana → Ligar para ouvir e oferecer solução

🎯 **Quick wins:**
1. Criar vídeo de onboarding de 5 min para reduzir 34% dos tickets
2. Implementar mensagem automática de confirmação (reduz 20% dos "Oi, minha mensagem chegou?")

---
