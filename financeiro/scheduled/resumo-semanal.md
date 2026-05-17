# Resumo Semanal Financeiro

Consolidado da semana: vendas, despesas, inadimplência e alertas para a semana seguinte.

## Frequência
**Semanal** — sugerido toda sexta-feira às 17h

## Como agendar com Claude Code

```bash
# Criar agendamento semanal toda sexta às 17h
claude schedule create \
  --name "resumo-semanal-financeiro" \
  --cron "0 17 * * 5" \
  --prompt-file financeiro/scheduled/resumo-semanal.md \
  --output-format markdown
```

---

## Prompt

```
Você é o assistente financeiro da empresa [NOME_DA_EMPRESA].

Gere o Resumo Semanal Financeiro da semana de [DATA_INÍCIO] a [DATA_FIM]:

**RECEITAS DA SEMANA:**
[Ex:
- Segunda: R$ 3.200
- Terça: R$ 1.800
- Quarta: R$ 4.500
- Quinta: R$ 2.900
- Sexta: R$ 3.600]

**DESPESAS DA SEMANA:**
[Ex:
- Fornecedores pagos: R$ 6.000
- Despesas operacionais: R$ 1.200
- Salários (se pagos na semana): R$ 0]

**INADIMPLÊNCIA:**
[Ex:
- Cliente A — vencida há 15 dias — R$ 2.500
- Cliente B — vencida há 3 dias — R$ 800]

**CONTAS A PAGAR NA PRÓXIMA SEMANA:**
[Ex:
- Fornecedor X: R$ 3.500 (vence segunda)
- Aluguel: R$ 4.000 (vence quarta)]

Gere:
1. Resumo financeiro da semana (receita, despesa, saldo líquido)
2. Dia mais forte e mais fraco de vendas
3. Situação da inadimplência (total e % do faturamento)
4. Alertas de pagamentos da próxima semana
5. Sinal de saúde financeira: 🟢🟡🔴 com justificativa
6. Uma ação prioritária para a próxima semana
```

---

## Exemplo de saída

---
📊 **RESUMO SEMANAL — 12 a 16/05/2025**

**Receita:** R$ 16.000  
**Despesas:** R$ 7.200  
**Saldo líquido:** +R$ 8.800 🟢

📅 **Melhor dia:** Quarta (R$ 4.500) | **Mais fraco:** Terça (R$ 1.800)

⚠️ **Inadimplência:** R$ 3.300 (20,6% da receita semanal) — acima do limite saudável de 5%  
📌 **Alertas próx. semana:** R$ 7.500 em contas a pagar (segunda + quarta)

🩺 **Saúde:** 🟡 — caixa positivo, mas inadimplência preocupa

🎯 **Ação da semana:** Cobrar Cliente A (R$ 2.500, 15 dias em atraso) — ligar hoje antes de fechar.

---
