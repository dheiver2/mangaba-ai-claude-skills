# Previsão de Receita (Forecast)

Gera uma projeção de faturamento para os próximos 3 meses com base no histórico e sazonalidade.

## Quando usar
- Planejamento trimestral
- Antes de contratar ou investir
- Para apresentar ao banco ao solicitar crédito

---

## Prompt

```
Você é um analista financeiro especializado em PMEs brasileiras.

Crie uma previsão de receita para [NOME_DA_EMPRESA], segmento [SEGMENTO], para os próximos 3 meses ([MÊS1], [MÊS2], [MÊS3]).

**Histórico dos últimos 6 meses:**
[Ex:
- Dezembro/24: R$ 42.000
- Janeiro/25: R$ 35.000 (queda — pós-festas)
- Fevereiro/25: R$ 38.000
- Março/25: R$ 45.000
- Abril/25: R$ 47.000
- Maio/25: R$ 50.000]

**Informações adicionais:**
- Novos clientes/contratos previstos: [DESCREVA ou "nenhum"]
- Campanhas de marketing planejadas: [DESCREVA ou "nenhuma"]
- Sazonalidade conhecida: [DESCREVA, ex: "junho é fraco, novembro é forte"]
- Meta de crescimento desejada: [X%] ao mês

Gere:
1. Projeção conservadora (cenário pessimista -15%)
2. Projeção realista (cenário base)
3. Projeção otimista (cenário com crescimento)
4. Premissas usadas para cada cenário
5. KPIs para monitorar mensalmente
6. Alertas: o que pode fazer o forecast não se realizar
```

---

## Exemplo de saída

**Projeções para Jun/Jul/Ago 2025:**

| Cenário | Junho | Julho | Agosto | Total Trim. |
|---------|-------|-------|--------|-------------|
| Pessimista | R$ 42.500 | R$ 44.000 | R$ 46.000 | R$ 132.500 |
| Realista | R$ 50.000 | R$ 52.000 | R$ 54.000 | R$ 156.000 |
| Otimista | R$ 57.500 | R$ 61.000 | R$ 65.000 | R$ 183.500 |

**Premissas (realista):** Crescimento de 2% a.m. com base na tendência dos últimos 3 meses. Julho com leve queda por recesso escolar no segmento.

**KPIs para monitorar:**
- Ticket médio (meta: R$ 850)
- Número de novos clientes/mês (meta: 8)
- Taxa de recompra (meta: 40%)

**Alertas:** Inadimplência acima de 5% pode derrubar o cenário realista para o pessimista.
