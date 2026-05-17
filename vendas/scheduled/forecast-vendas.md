# Forecast Mensal de Vendas

Projeção de fechamento do mês com análise de probabilidade por deal e comparativo com a meta.

## Frequência
**Mensal** — sugerido no dia 20 de cada mês às 9h (para ajustar estratégia nos últimos dias)

## Como agendar com Claude Code

```bash
claude schedule create \
  --name "forecast-mensal-vendas" \
  --cron "0 9 20 * *" \
  --prompt-file vendas/scheduled/forecast-vendas.md
```

---

## Prompt

```
Você é o diretor comercial da empresa [NOME_DA_EMPRESA].

Gere o Forecast de Vendas de [MÊS/ANO] — análise feita no dia 20:

**JÁ FECHADO NO MÊS:** R$ [VALOR]
**META DO MÊS:** R$ [VALOR]
**DIAS ÚTEIS RESTANTES:** [NÚMERO]

**PIPELINE PROVÁVEL DE FECHAR ATÉ O FIM DO MÊS:**
[Para cada deal, informe:
- Nome/empresa
- Valor
- Etapa atual
- % de probabilidade de fechar este mês (seja honesto)
- O que falta para fechar]

**PIPELINE POSSÍVEL (pode entrar, mas incerto):**
[Mesma estrutura acima]

**HISTÓRICO:**
- Mês anterior: R$ [VALOR] (atingiu [X%] da meta)
- Média dos últimos 3 meses: R$ [VALOR]

Gere:
1. Forecast comprometido (só o que está quase certo)
2. Forecast estendido (comprometido + provável)
3. Gap para a meta e o que faria fecha-la
4. Cenários: Pessimista / Realista / Otimista
5. Recomendação de ação para os 10 dias restantes
6. Deals que devem ser descartados (evitar perda de tempo)
```
