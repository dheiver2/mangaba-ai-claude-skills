# Análise de Pipeline de Vendas

Avalia o funil de vendas atual, identifica oportunidades travadas e estima a receita previsível.

## Quando usar
- Revisão semanal ou quinzenal do pipeline com a equipe
- Antes de definir prioridades de prospecção
- Para apresentar previsão de receita para sócios

---

## Prompt

```
Você é um gerente de vendas especializado em PMEs brasileiras.

Analise o pipeline de vendas da empresa [NOME_DA_EMPRESA]:

**FUNIL ATUAL (liste as oportunidades por etapa):**

PROSPECÇÃO (contato inicial feito):
[Nome do prospect | Valor estimado | Há quanto tempo está aqui]

QUALIFICAÇÃO (reunião/diagnóstico feito):
[Nome | Valor | Tempo]

PROPOSTA ENVIADA:
[Nome | Valor | Tempo | Feedback recebido]

NEGOCIAÇÃO:
[Nome | Valor | Tempo | Principal objeção]

FECHAMENTO (aguardando assinatura/pagamento):
[Nome | Valor | Tempo]

**META DE VENDAS DO MÊS:** R$ [VALOR]
**Vendas já fechadas no mês:** R$ [VALOR]
**Ciclo médio de vendas:** [X dias]

Gere:
1. Valor total do pipeline e receita previsível (ponderado por probabilidade de cada etapa)
2. Oportunidades "travadas" — ficaram mais tempo que o ciclo médio em uma etapa
3. Top 3 deals para priorizar esta semana (maior chance × maior valor)
4. Oportunidades para dar low-up urgente
5. Gap para a meta: quanto falta e de onde pode vir
6. Taxa de conversão por etapa (se houver histórico)
7. Ação recomendada para cada deal em negociação ou proposta enviada
```

---

## Exemplo de saída (trecho)

**Pipeline total:** R$ 87.500  
**Receita previsível (ponderada):** R$ 31.200  
**Meta:** R$ 50.000 | **Gap:** R$ 18.800

🔴 **Deals travados (ação urgente):**
- Empresa X — proposta enviada há 18 dias sem resposta (ciclo médio: 7 dias) → Ligar hoje, não email
- Empresa Y — negociação há 22 dias → Oferecer concessão de baixo custo para destravar

🎯 **Top 3 prioridades da semana:**
1. Empresa Z — R$ 12.000 em fechamento, só aguarda contrato → Enviar hoje
2. Empresa W — R$ 8.500 em negociação, objeção de preço → Apresentar case de ROI
3. Empresa V — R$ 6.000 em proposta → Follow-up por WhatsApp com depoimento de cliente
