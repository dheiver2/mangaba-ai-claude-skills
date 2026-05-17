# Análise de Fluxo de Caixa

Analisa entradas e saídas do mês, identifica gargalos e sugere ações para melhorar a liquidez da empresa.

## Quando usar
- Ao final de cada mês para revisar o desempenho financeiro
- Quando sentir que o caixa está apertado
- Antes de tomar decisões de investimento

---

## Prompt

```
Você é um consultor financeiro especialista em PMEs brasileiras.

Analise o fluxo de caixa abaixo da empresa [NOME_DA_EMPRESA] referente ao período [MÊS/ANO]:

**ENTRADAS:**
[Liste cada entrada com valor, ex:
- Vendas à vista: R$ 12.000
- Recebimentos parcelados: R$ 8.500
- Outras receitas: R$ 1.200]

**SAÍDAS:**
[Liste cada saída com valor, ex:
- Fornecedores: R$ 6.000
- Folha de pagamento: R$ 9.000
- Aluguel: R$ 3.500
- Impostos: R$ 2.800
- Outras despesas: R$ 1.100]

**Saldo inicial do mês:** R$ [VALOR]

Com base nesses dados, me forneça:
1. Saldo final do mês e variação em relação ao saldo inicial
2. Índice de liquidez corrente (entradas ÷ saídas)
3. Top 3 maiores despesas e percentual sobre o total
4. Análise em 3 linhas: o que está indo bem e o que preocupa
5. 3 ações concretas para melhorar o fluxo no próximo mês
6. Alerta se o saldo cair abaixo de 2 meses de despesas fixas

Responda em formato estruturado, use R$ para todos os valores e seja direto.
```

---

## Exemplo de saída

**Saldo final:** R$ 18.300 (+R$ 5.100 vs início do mês)  
**Liquidez:** 1,27 — positivo, empresa cobre todas as despesas com folga de 27%

**Top 3 despesas:**
1. Folha de pagamento: R$ 9.000 (40% do total)
2. Fornecedores: R$ 6.000 (26,8%)
3. Aluguel: R$ 3.500 (15,6%)

**Análise:** O mês foi positivo com saldo crescendo 38%. Porém a folha representa 40% das saídas — acima do recomendado (30%) para PMEs. Os recebimentos parcelados são R$ 8.500 que ainda não entraram — monitorar inadimplência.

**Ações:**
1. Antecipar R$ 4.000 em recebíveis via antecipação de recebíveis no banco para reforçar caixa em agosto
2. Negociar prazo maior com fornecedor X (atual 15 dias → 30 dias)
3. Revisar estrutura de equipe: custo de pessoal está acima do benchmark do setor
