# Artefato: DRE Simplificada (Demonstrativo de Resultados)

Gera um DRE mensal simplificado para PMEs, sem precisar de contador — útil para acompanhar a saúde do negócio.

## Quando usar
- Fechamento mensal
- Apresentação para sócios ou investidores
- Solicitação de crédito empresarial

---

## Prompt

```
Você é um contador especializado em PMEs brasileiras.

Gere um DRE (Demonstrativo do Resultado do Exercício) simplificado para [NOME_DA_EMPRESA] referente a [MÊS/ANO]:

**Dados do período:**

RECEITAS:
- Receita bruta de vendas/serviços: R$ [VALOR]
- (-) Devoluções e cancelamentos: R$ [VALOR]
- (-) Impostos sobre vendas (Simples/ISS/PIS/COFINS): R$ [VALOR]
= Receita Líquida: [CALCULE]

CUSTOS:
- Custo dos produtos vendidos (CPV) ou Custo dos serviços prestados (CSP): R$ [VALOR]
= Lucro Bruto: [CALCULE]

DESPESAS OPERACIONAIS:
- Pessoal (salários + encargos + benefícios): R$ [VALOR]
- Aluguel e condomínio: R$ [VALOR]
- Utilities (energia, água, internet, telefone): R$ [VALOR]
- Marketing e vendas: R$ [VALOR]
- Tecnologia e softwares: R$ [VALOR]
- Honorários contábeis: R$ [VALOR]
- Outras despesas administrativas: R$ [VALOR]
= Total Despesas Operacionais: [CALCULE]

= EBITDA (Lucro antes de juros, impostos, deprec. e amort.): [CALCULE]
- Depreciação/amortização (se houver): R$ [VALOR ou 0]
= EBIT: [CALCULE]
- Resultado financeiro (juros de empréstimos): R$ [VALOR ou 0]
= EBT: [CALCULE]
- IRPJ/CSLL (se Lucro Real ou Presumido): R$ [VALOR ou 0]
= LUCRO LÍQUIDO: [CALCULE]

Além do DRE, forneça:
1. Margens: Bruta, EBITDA, Líquida (em %)
2. Comparativo com o mês anterior (se informado)
3. 3 indicadores de saúde financeira com diagnóstico
4. Recomendações do contador em 3 tópicos
```

---

## Exemplo de saída

```
DRE SIMPLIFICADA — MAIO/2025
[NOME_DA_EMPRESA] | CNPJ: XX.XXX.XXX/0001-XX

RECEITAS                              R$          %
Receita Bruta                         58.000    120%
(-) Devoluções                        -1.500     -3%
(-) Impostos sobre vendas             -6.500    -13%
= RECEITA LÍQUIDA                     50.000    100%

CUSTOS
(-) CPV/CSP                          -15.000    -30%
= LUCRO BRUTO                         35.000     70%

DESPESAS OPERACIONAIS
Pessoal                              -17.000    -34%
Aluguel                               -4.000     -8%
Utilities                             -1.500     -3%
Marketing                             -2.000     -4%
Tecnologia                              -800     -2%
Administrativas                       -1.200     -2%
= TOTAL DESPESAS                     -26.500    -53%

= EBITDA                               8.500     17%
(-) Depreciação                          -500     -1%
= EBIT                                 8.000     16%
(-) Juros                                  0      0%
= LUCRO LÍQUIDO                        8.000     16%

DIAGNÓSTICO: Margem líquida de 16% — saudável para o segmento.
Atenção: custo de pessoal em 34% está acima do benchmark (ideal < 30%).
```
