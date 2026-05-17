# Análise de Regime Tributário

Compara Simples Nacional, Lucro Presumido e Lucro Real para identificar qual regime é mais vantajoso para a empresa.

## Quando usar
- Janeiro (antes do prazo de opção pelo Simples — 31/jan)
- Quando o faturamento está se aproximando dos limites do Simples (R$ 4,8M/ano)
- Quando a margem líquida está caindo mesmo com crescimento de receita

---

## Prompt

```
Você é um contador especializado em PMEs brasileiras.

Faça uma análise comparativa de regime tributário para [NOME_DA_EMPRESA]:

**Dados da empresa:**
- Segmento: [SEGMENTO]
- CNAE principal: [CNAE ou "não sei"]
- Regime atual: [Simples Nacional / Lucro Presumido / Lucro Real / MEI]
- Faturamento anual (últimos 12 meses): R$ [VALOR]
- Projeção de faturamento próximo ano: R$ [VALOR]
- Folha de pagamento mensal (salários + encargos): R$ [VALOR]
- Margem bruta média: [X%]
- Principais despesas dedutíveis: [Ex: aluguel, energia, insumos, importações]

**Sócios:**
- Número de sócios: [NÚMERO]
- Pró-labore mensal total: R$ [VALOR]

Compare os 3 regimes e forneça:
1. Alíquota efetiva em cada regime (% sobre faturamento)
2. Imposto total anual estimado em cada regime
3. Economia/custo adicional vs regime atual
4. Impacto no preço de venda para manter a margem
5. Regime recomendado com justificativa
6. Prazo e procedimento para troca de regime
7. Riscos de cada regime para este perfil de empresa

⚠️ Inclua aviso de que a decisão final deve ser tomada com o contador da empresa.
```

---

## Exemplo de saída (trecho)

| Regime | Alíquota efetiva | Imposto anual | vs Atual |
|--------|-----------------|---------------|----------|
| Simples Nacional (Anexo III) | 14,7% | R$ 88.200 | — |
| Lucro Presumido | 11,3% | R$ 67.800 | -R$ 20.400 ✅ |
| Lucro Real | 13,1% | R$ 78.600 | -R$ 9.600 |

**Recomendação:** Migrar para Lucro Presumido pode economizar ~R$ 1.700/mês. Viável se a folha de pagamento for abaixo de 28% do faturamento — o que é o caso. Consulte seu contador até dezembro para fazer a opção em janeiro.
