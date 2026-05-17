# Relatório Operacional Semanal

Dashboard rápido da operação: capacidade, entregas, atrasos e alertas da semana.

## Frequência
**Semanal** — sugerido toda sexta-feira às 16h

## Como agendar com Claude Code

```bash
claude schedule create \
  --name "relatorio-operacional" \
  --cron "0 16 * * 5" \
  --prompt-file operacional/scheduled/relatorio-operacional.md
```

---

## Prompt

```
Você é o gerente de operações da empresa [NOME_DA_EMPRESA].

Gere o Relatório Operacional da semana de [DATA_INÍCIO] a [DATA_FIM]:

**CAPACIDADE E VOLUME:**
- Pedidos/projetos/atendimentos abertos: [NÚMERO]
- Concluídos na semana: [NÚMERO]
- Em andamento: [NÚMERO]
- Cancelados: [NÚMERO]

**PRAZOS:**
- Entregas no prazo: [NÚMERO] ([%])
- Entregas atrasadas: [NÚMERO] — motivos: [DESCREVA]
- Atrasos acima de 3 dias: [NÚMERO]

**QUALIDADE:**
- Retrabalhos registrados: [NÚMERO]
- Reclamações operacionais: [NÚMERO]
- Devoluções/refações: [NÚMERO]

**EQUIPE:**
- Horas produtivas estimadas: [NÚMERO]
- Tarefas bloqueadas (aguardando algo externo): [NÚMERO e MOTIVO]
- Colaborador mais sobrecarregado: [NOME/CARGO ou "equipe equilibrada"]

**PRÓXIMA SEMANA:**
- Volume previsto: [NÚMERO]
- Prazos críticos: [LISTE]

Gere:
1. Dashboard visual com semáforo por categoria (🟢🟡🔴)
2. Taxa de entrega no prazo vs benchmark (meta: >90%)
3. Alerta de capacidade: a equipe consegue absorver a próxima semana?
4. Top 2 problemas operacionais da semana com ação corretiva
5. Uma quick win para melhorar na semana seguinte
```
