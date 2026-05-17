# Fechamento Mensal

Relatório completo de fechamento: DRE simplificada, análise de desempenho e metas para o próximo mês.

## Frequência
**Mensal** — sugerido no 1º dia útil do mês seguinte às 9h

## Como agendar com Claude Code

```bash
# Criar agendamento no 1º dia de cada mês às 9h
claude schedule create \
  --name "fechamento-mensal" \
  --cron "0 9 1 * *" \
  --prompt-file financeiro/scheduled/fechamento-mensal.md \
  --output-format markdown
```

---

## Prompt

```
Você é o CFO virtual da empresa [NOME_DA_EMPRESA].

Gere o Relatório de Fechamento Mensal de [MÊS/ANO]:

**RECEITAS:**
- Faturamento bruto: R$ [VALOR]
- Descontos concedidos: R$ [VALOR]
- Devoluções/cancelamentos: R$ [VALOR]
- **Receita líquida:** R$ [CALCULE]

**CUSTOS E DESPESAS:**
- Custo dos produtos/serviços (CMV/CSV): R$ [VALOR]
- Folha de pagamento + encargos: R$ [VALOR]
- Aluguel: R$ [VALOR]
- Marketing: R$ [VALOR]
- Tecnologia/softwares: R$ [VALOR]
- Impostos (Simples Nacional ou regime): R$ [VALOR]
- Outras despesas: R$ [VALOR]

**METAS DO MÊS:**
- Meta de faturamento: R$ [META]
- Meta de novos clientes: [NÚMERO]
- Meta de margem líquida: [X%]

Gere:
1. DRE Simplificada com: Receita Líquida → Lucro Bruto → EBITDA → Lucro Líquido
2. Margem bruta e margem líquida (%)
3. Comparação com meta: atingida / não atingida por quanto
4. Top 3 resultados positivos do mês
5. Top 3 pontos de melhoria
6. Metas sugeridas para o próximo mês (com base na tendência)
7. Resumo executivo em 5 linhas para apresentar à equipe
```

---

## Exemplo de saída

---
📊 **FECHAMENTO — MAIO/2025 | [NOME_DA_EMPRESA]**

**DRE Simplificada:**
| | Valor | % Receita |
|--|-------|-----------|
| Receita Líquida | R$ 48.500 | 100% |
| (-) CMV/CSV | R$ 14.550 | 30% |
| **Lucro Bruto** | **R$ 33.950** | **70%** |
| (-) Despesas Operacionais | R$ 22.400 | 46,2% |
| **EBITDA** | **R$ 11.550** | **23,8%** |
| (-) Impostos | R$ 3.880 | 8% |
| **Lucro Líquido** | **R$ 7.670** | **15,8%** |

**Meta de faturamento:** R$ 50.000 — atingida 97% 🟡  
**Meta de novos clientes:** 10 — atingida 8 (80%) 🟡

✅ **Destaques:** Margem bruta de 70% (excelente). Controle de despesas fixas estável. Taxa de recompra atingiu 45%.  
⚠️ **Melhoras:** Faltaram 2 novos clientes para a meta. Marketing com ROI abaixo do esperado. Inadimplência 8% (acima do ideal).

🎯 **Metas Junho:** Faturamento R$ 52.000 | 11 novos clientes | Reduzir inadimplência para 5%

---
