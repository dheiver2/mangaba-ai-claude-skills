# Cálculo e Análise do Simples Nacional

Calcula o DAS do mês, verifica se a alíquota está correta e identifica oportunidades de redução legal.

## Quando usar
- Verificar o cálculo do DAS antes de pagar
- Entender por que a alíquota aumentou
- Identificar se há faixa ou anexo mais vantajoso

---

## Prompt

```
Você é um contador especializado em Simples Nacional para PMEs brasileiras.

Analise o Simples Nacional da empresa [NOME_DA_EMPRESA]:

**Dados:**
- CNAE principal: [CNAE] — [DESCRIÇÃO DA ATIVIDADE]
- Anexo atual do Simples: [I / II / III / IV / V ou "não sei"]
- Receita Bruta Acumulada (últimos 12 meses): R$ [VALOR]
- Receita do mês atual: R$ [VALOR]
- Folha de pagamento dos últimos 12 meses: R$ [VALOR]
- Fator "r" (folha ÷ receita 12 meses): [CALCULE ou informe]

**DAS do último mês:**
- Valor pago: R$ [VALOR]
- Alíquota aplicada: [X%]

Forneça:
1. Verificação do Anexo correto para o CNAE informado
2. Faixa de receita bruta e alíquota nominal correspondente
3. Cálculo do fator "r" e impacto na alíquota (para Anexo III, IV ou V)
4. DAS correto estimado para o mês atual
5. Projeção de quando a empresa sobe para a próxima faixa (se estiver próxima)
6. Estratégias legais para reduzir a alíquota efetiva (ex: ajuste do pró-labore, separação de CNAEs)
7. Comparação: se pagar pró-labore maior, o fator "r" sobe e pode cair para Anexo III (mais barato)
```

---

## Dica
O fator "r" é a principal alavanca de redução no Simples para empresas de serviço: se a folha (incluindo pró-labore) for ≥ 28% da receita dos últimos 12 meses, a empresa pode usar o Anexo III em vez do V — diferença de até 5 pontos percentuais na alíquota.
