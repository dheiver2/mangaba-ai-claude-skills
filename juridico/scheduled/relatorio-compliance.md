# Relatório Mensal de Compliance

Consolida o status de conformidade regulatória da empresa — contratos, LGPD, alvarás e obrigações legais.

## Frequência
**Mensal** — sugerido no 1º dia útil do mês às 9h

## Como agendar com Claude Code

```bash
claude schedule create \
  --name "compliance-mensal" \
  --cron "0 9 1 * *" \
  --prompt-file juridico/scheduled/relatorio-compliance.md
```

---

## Prompt

```
Você é o gerente de compliance da empresa [NOME_DA_EMPRESA].

Gere o Relatório de Compliance de [MÊS/ANO]:

**CONTRATOS:**
- Total de contratos ativos: [NÚMERO]
- Contratos vencidos sem renovação: [NÚMERO]
- Contratos renegociados no mês: [NÚMERO]
- Novos contratos assinados: [NÚMERO]

**LGPD:**
- Incidentes de dados no mês: [NÚMERO ou "nenhum"]
- Solicitações de titulares (acesso, exclusão): [NÚMERO]
- Respondidas no prazo (15 dias): [SIM/NÃO/PARCIAL]

**LICENÇAS E ALVARÁS:**
[Liste: documento, órgão emissor, validade]

**OBRIGAÇÕES TRABALHISTAS:**
- FGTS recolhido em dia: [SIM/NÃO]
- e-Social atualizado: [SIM/NÃO]
- Férias vencidas sem gozo: [NÚMERO de colaboradores]

**PENDÊNCIAS DO MÊS ANTERIOR:**
[Liste o que ficou em aberto]

Gere:
1. Score de compliance geral (semáforo 🟢🟡🔴 por área)
2. Top 3 riscos regulatórios ativos
3. Obrigações cumpridas vs pendentes
4. Ações corretivas prioritárias
5. Calendário de compliance para o próximo mês
```
