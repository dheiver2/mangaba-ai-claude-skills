# Relatório Mensal de Custos de TI

Consolida todos os gastos com tecnologia do mês e analisa o ROI de cada ferramenta.

## Frequência
**Mensal** — sugerido no último dia útil do mês às 15h

## Como agendar com Claude Code

```bash
claude schedule create \
  --name "custos-ti-mensal" \
  --cron "0 15 28-31 * *" \
  --prompt-file tecnologia/scheduled/relatorio-custos-ti.md
```

---

## Prompt

```
Você é o gerente de tecnologia da empresa [NOME_DA_EMPRESA].

Gere o Relatório de Custos de TI de [MÊS/ANO]:

**GASTOS DO MÊS:**

Infraestrutura:
- Hospedagem/servidor: R$ [VALOR]
- Domínios: R$ [VALOR]
- CDN/armazenamento em nuvem: R$ [VALOR]

Software e SaaS:
[Liste cada ferramenta com valor]

Hardware:
- Manutenção/reparo: R$ [VALOR]
- Aquisição: R$ [VALOR]

Serviços:
- Suporte técnico terceirizado: R$ [VALOR]
- Desenvolvimento: R$ [VALOR]

**FATURAMENTO DA EMPRESA:** R$ [VALOR]
**NÚMERO DE COLABORADORES:** [NÚMERO]

Gere:
1. Total de gastos com TI e % do faturamento (benchmark saudável: 3-8% para PMEs)
2. Custo de TI por colaborador
3. Ranking de ferramentas por custo
4. Análise de ROI de cada ferramenta principal (o que ela entrega vs quanto custa)
5. Tendência: TI está crescendo mais rápido que o faturamento?
6. Recomendações de otimização
7. Investimentos de TI previstos para o próximo mês
```
