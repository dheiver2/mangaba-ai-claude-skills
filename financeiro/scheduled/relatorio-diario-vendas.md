# Relatório Diário de Vendas

Gera um resumo rápido do dia de vendas para o gestor acompanhar a performance em tempo real.

## Frequência
**Diária** — sugerido às 18h (ao final do expediente)

## Como agendar com Claude Code

```bash
# Criar agendamento diário às 18h (segunda a sexta)
claude schedule create \
  --name "relatorio-diario-vendas" \
  --cron "0 18 * * 1-5" \
  --prompt-file financeiro/scheduled/relatorio-diario-vendas.md \
  --output-format markdown
```

---

## Prompt

```
Você é o assistente financeiro da empresa [NOME_DA_EMPRESA].

Hoje é [DATA_HOJE]. Gere o Relatório Diário de Vendas com base nos dados abaixo:

**Vendas de hoje:**
[Cole os dados do seu sistema, ex:
- Venda #1042 — Cliente: João Silva — Produto: Consultoria Mensal — R$ 1.500
- Venda #1043 — Cliente: Maria Ltda — Produto: Pacote Starter — R$ 800
- Venda #1044 — Cliente: Pedro ME — Produto: Consultoria Avulsa — R$ 350]

**Meta diária:** R$ [META_DO_DIA]
**Acumulado do mês até ontem:** R$ [VALOR_ACUMULADO]
**Meta mensal:** R$ [META_MENSAL]

Gere um relatório conciso com:
1. Total vendido hoje e % da meta diária atingida
2. Ticket médio do dia
3. Acumulado do mês e % da meta mensal
4. Projeção do mês se manter o ritmo atual
5. Status visual: 🟢 (acima da meta) / 🟡 (dentro do esperado) / 🔴 (abaixo da meta)
6. Uma frase de análise em 2 linhas

Formato: compacto, para leitura rápida no celular. Use emojis para facilitar a leitura.
```

---

## Exemplo de saída

---
📊 **RELATÓRIO DE VENDAS — 17/05/2025**

💰 **Hoje:** R$ 2.650 (106% da meta diária de R$ 2.500) 🟢  
🧾 **Ticket médio:** R$ 883  
📅 **Mês:** R$ 38.400 / R$ 50.000 (76,8%) — faltam 14 dias  
📈 **Projeção mensal:** R$ 51.200 (102% da meta) 🟢

✍️ *Dia forte puxado pela venda do pacote Maria Ltda. Se manter o ritmo atual, o mês fecha no azul.*

---
