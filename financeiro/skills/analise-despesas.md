# Análise e Corte de Despesas

Identifica despesas excessivas, compara com benchmarks do setor e sugere onde cortar sem prejudicar a operação.

## Quando usar
- Quando a margem de lucro caiu e você não sabe por quê
- Antes de demitir alguém — há cortes mais inteligentes antes disso
- Planejamento anual / revisão semestral de custos

---

## Prompt

```
Você é um especialista em redução de custos para pequenas e médias empresas brasileiras.

Analise as despesas mensais da empresa [NOME_DA_EMPRESA], segmento [SEGMENTO_EX: varejo/serviços/industria], faturamento mensal médio: R$ [FATURAMENTO]:

**DESPESAS FIXAS:**
[Ex:
- Aluguel: R$ 4.000
- Internet/telefone: R$ 800
- Softwares/assinaturas: R$ 1.200
- Energia elétrica: R$ 600
- Contador: R$ 700]

**DESPESAS VARIÁVEIS:**
[Ex:
- Fornecedores/matéria-prima: R$ 15.000
- Comissões de vendas: R$ 2.500
- Frete/logística: R$ 1.800
- Marketing: R$ 900]

**DESPESAS COM PESSOAL:**
[Ex:
- Salários: R$ 12.000
- Encargos (FGTS, INSS): R$ 3.600
- Benefícios (VT, VR): R$ 1.400]

Faça:
1. Total por categoria e % do faturamento
2. Compare com benchmarks saudáveis para o segmento informado
3. Marque em vermelho despesas acima do benchmark
4. Liste 5 oportunidades concretas de corte ou renegociação (com economia estimada)
5. O que NÃO cortar (despesas estratégicas)
6. Meta de economia possível em 90 dias
```

---

## Exemplo de saída

**Resumo de despesas:**
| Categoria | Valor | % Faturamento | Benchmark | Status |
|-----------|-------|---------------|-----------|--------|
| Pessoal | R$ 17.000 | 42,5% | máx 35% | 🔴 Acima |
| Fixos | R$ 7.300 | 18,3% | máx 20% | ✅ OK |
| Variáveis | R$ 20.200 | 50,5% | máx 45% | 🔴 Acima |

**Top 5 oportunidades de corte:**
1. **Assinaturas duplicadas** (R$ 1.200 → R$ 600): Há 3 ferramentas com funções sobrepostas. Consolidar em uma.
2. **Renegociar frete** (economia est. R$ 400/mês): Volume atual permite negociar tabela preferencial com transportadora.
3. **Tarifa de energia** (economia est. R$ 150/mês): Migrar para mercado livre de energia — viável acima de R$ 500/mês.
4. **Banco** (economia est. R$ 200/mês): Taxa de manutenção de conta PJ — bancos digitais cobram zero.
5. **Fornecedor principal** (economia est. R$ 800/mês): Pagamento à vista dá desconto médio de 5-8% — negocie.

**Meta 90 dias:** Economia de R$ 1.550 a R$ 2.100/mês (R$ 18.600 a R$ 25.200/ano)
