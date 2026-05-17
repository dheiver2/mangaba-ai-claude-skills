# Relatório Semanal de Pipeline

Snapshot do funil de vendas para acompanhamento e priorização da equipe comercial.

## Frequência
**Semanal** — sugerido toda segunda-feira às 8h (para alinhar a semana)

## Como agendar com Claude Code

```bash
claude schedule create \
  --name "pipeline-semanal" \
  --cron "0 8 * * 1" \
  --prompt-file vendas/scheduled/relatorio-pipeline.md
```

---

## Prompt

```
Você é o gerente comercial da empresa [NOME_DA_EMPRESA].

Gere o Relatório de Pipeline da semana de [DATA_INÍCIO] a [DATA_FIM]:

**RESUMO DO FUNIL:**
- Prospecção: [X oportunidades | R$ valor total]
- Qualificação: [X | R$]
- Proposta enviada: [X | R$]
- Negociação: [X | R$]
- Fechamento: [X | R$]

**MOVIMENTAÇÕES DA SEMANA:**
- Novos leads gerados: [NÚMERO]
- Propostas enviadas: [NÚMERO]
- Deals fechados: [NÚMERO] — R$ [VALOR]
- Deals perdidos: [NÚMERO] — motivo principal: [DESCREVA]

**META DO MÊS:** R$ [VALOR]
**Realizado até hoje:** R$ [VALOR]
**Dias úteis restantes no mês:** [NÚMERO]

Gere:
1. Funil visual (barra de texto com % de conversão entre etapas)
2. Receita previsível ponderada
3. Ritmo necessário para bater a meta (R$/dia nos dias restantes)
4. Top 3 deals para fechar esta semana
5. Deals em risco de esfriar (sem contato há mais de 7 dias)
6. Taxa de conversão da semana vs semana anterior
```
