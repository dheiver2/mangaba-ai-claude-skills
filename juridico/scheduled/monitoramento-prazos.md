# Monitoramento Semanal de Prazos Jurídicos

Alerta sobre vencimentos contratuais, renovações e obrigações legais da semana.

## Frequência
**Semanal** — sugerido toda segunda-feira às 8h

## Como agendar com Claude Code

```bash
claude schedule create \
  --name "prazos-juridicos" \
  --cron "0 8 * * 1" \
  --prompt-file juridico/scheduled/monitoramento-prazos.md
```

---

## Prompt

```
Você é o assistente jurídico da empresa [NOME_DA_EMPRESA].

Revise os prazos e obrigações jurídicas da semana de [DATA_INÍCIO] a [DATA_FIM]:

**CONTRATOS ATIVOS:**
[Liste: nome do contrato, contraparte, valor, data de vencimento/renovação]

**NOTIFICAÇÕES ENVIADAS AGUARDANDO RESPOSTA:**
[Liste: destinatário, motivo, data envio, prazo de resposta]

**AÇÕES JUDICIAIS OU ADMINISTRATIVAS EM ANDAMENTO:**
[Liste ou "nenhuma"]

**OBRIGAÇÕES LEGAIS DO MÊS:**
[Ex: renovação de alvará em 20/06, entrega de relatório ANPD em 30/06]

Gere:
1. Alertas de prazo para esta semana (classificados por urgência 🔴🟡🟢)
2. Contratos que vencem nos próximos 30 dias (renovar ou encerrar?)
3. Notificações sem resposta vencidas (escalar para advogado?)
4. Ação recomendada para cada item
5. Resumo de exposição jurídica atual da empresa
```

---

## Exemplo de saída

---
⚖️ **PRAZOS JURÍDICOS — Semana 19/05/2025**

🔴 **URGENTE:**
- Contrato Fornecedor X vence **quinta (22/05)** — decidir renovação até quarta
- Notificação enviada à Cliente Y em 05/05 — prazo de 15 dias vence **sexta (23/05)** sem resposta

🟡 **ATENÇÃO (próximos 30 dias):**
- Alvará de funcionamento vence em 15/06 — iniciar renovação esta semana
- Contrato de aluguel renovação automática em 01/07 — verificar se quer renegociar

🟢 **OK:**
- 3 contratos ativos sem vencimento próximo

🎯 **Ação desta semana:** Ligar para Cliente Y antes de sexta — evita necessidade de protesto.

---
