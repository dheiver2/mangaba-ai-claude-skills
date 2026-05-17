# Relatório Mensal de Engajamento

Analisa os resultados de marketing do mês e sugere ajustes para o próximo.

## Frequência
**Mensal** — sugerido no último dia do mês às 16h

## Como agendar com Claude Code

```bash
# Criar agendamento no último dia do mês às 16h
claude schedule create \
  --name "relatorio-engajamento" \
  --cron "0 16 28-31 * *" \
  --prompt-file marketing/scheduled/relatorio-engajamento.md \
  --output-format markdown
```

---

## Prompt

```
Você é um analista de marketing digital especializado em PMEs brasileiras.

Analise os resultados de marketing de [NOME_DA_EMPRESA] em [MÊS/ANO]:

**INSTAGRAM:**
- Seguidores: [ANTES] → [DEPOIS] (variação: [+/-X])
- Alcance total: [VALOR]
- Impressões: [VALOR]
- Engajamento médio por post: [%]
- Post com melhor desempenho: [DESCREVA]
- Post com pior desempenho: [DESCREVA]
- Novos seguidores pelo feed: [VALOR]

**LINKEDIN (se aplicável):**
- Seguidores: [ANTES] → [DEPOIS]
- Visualizações de página: [VALOR]
- Post com maior alcance: [DESCREVA]

**EMAIL MARKETING (se aplicável):**
- Emails enviados: [VALOR]
- Taxa de abertura: [%] (benchmark do setor: [%])
- Taxa de clique: [%]
- Descadastramentos: [VALOR]

**RESULTADOS DE NEGÓCIO:**
- Leads gerados pelo marketing: [VALOR]
- Vendas atribuídas ao marketing: R$ [VALOR]
- Custo por lead: R$ [VALOR]

Gere:
1. Resumo executivo em 5 bullet points
2. Top 3 conteúdos que funcionaram (e por quê)
3. Top 3 conteúdos que não funcionaram (e por quê)
4. Análise do ROI de marketing
5. 5 recomendações para o próximo mês
6. Sinal de saúde do marketing: 🟢🟡🔴
```

---

## Exemplo de saída

**RESUMO EXECUTIVO — Marketing Maio/2025:**
- ✅ +320 seguidores no Instagram (melhor mês do ano)
- ✅ Taxa de abertura de email: 32% (benchmark: 22%) — excelente
- 🟡 Engajamento Instagram caiu 2pp vs abril (5,8% → 3,8%)
- 🟡 LinkedIn ainda com pouco alcance — canal em desenvolvimento
- ❌ ROI de marketing: R$ 3,20 por R$ 1 investido (meta era R$ 5)

**O QUE FUNCIONOU:**
1. Carrossel educativo "5 erros financeiros" — 1.240 curtidas, 89 compartilhamentos (conteúdo educativo performa 3x mais)
2. Email de reativação com cupom — 34% de abertura, 8% de conversão
3. Story com enquete — 412 respostas (aumenta alcance orgânico no algoritmo)

**RECOMENDAÇÕES JUNHO:**
1. Dobrar produção de carrosséis educativos (de 2 para 4/mês)
2. Testar Reels de 30 segundos com dica rápida
3. Criar sequência de 3 emails de boas-vindas para novos leads
4. Investir R$ 500 em tráfego pago para ampliar post educativo
5. Postar no LinkedIn às 7h-8h (horário de maior alcance B2B)

**Saúde do Marketing:** 🟡 — crescimento de audiência sólido, ROI abaixo da meta.
