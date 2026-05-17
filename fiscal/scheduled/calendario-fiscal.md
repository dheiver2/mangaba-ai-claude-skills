# Calendário Fiscal Mensal

Alerta sobre todas as obrigações fiscais do mês — DAS, DCTF, eSocial, FGTS e outras declarações.

## Frequência
**Mensal** — sugerido no 1º dia útil do mês às 8h

## Como agendar com Claude Code

```bash
claude schedule create \
  --name "calendario-fiscal" \
  --cron "0 8 1 * *" \
  --prompt-file fiscal/scheduled/calendario-fiscal.md
```

---

## Prompt

```
Você é o assistente fiscal da empresa [NOME_DA_EMPRESA].

Gere o Calendário de Obrigações Fiscais de [MÊS/ANO]:

**Regime tributário:** [Simples Nacional / Lucro Presumido / Lucro Real]
**Tem funcionários CLT?** [Sim: [X] funcionários / Não]
**Tem MEI paralelo?** [Sim / Não]
**Tem imóveis ou operações especiais?** [DESCREVA ou "não"]

Liste todas as obrigações do mês com:
1. Nome da obrigação
2. Data de vencimento
3. Órgão responsável (Receita Federal, FGTS, Prefeitura, etc.)
4. Valor estimado (se possível) ou "verificar com contador"
5. Como pagar (portal, DARF, DAS, etc.)
6. Consequência do atraso (multa + juros)
7. Alerta se a data cair em feriado (vence no próximo dia útil)

Organize por data de vencimento. Destaque as 3 mais críticas do mês.
```

---

## Exemplo de saída — Maio/2025 (Simples Nacional + 5 funcionários)

---
📅 **CALENDÁRIO FISCAL — MAIO/2025**

| Data | Obrigação | Valor est. | Como pagar | Multa atraso |
|------|-----------|------------|------------|--------------|
| 07/05 | FGTS (abril) | R$ 1.440 | SEFIP/Conectividade | 2% + 0,033%/dia |
| 13/05 | eSocial (folha maio) | — | Portal eSocial | Varia |
| 20/05 | DAS Simples Nacional (abril) | R$ 3.200 | App Receita Federal | 0,33%/dia + 20% |
| 20/05 | DARF IRRF (se aplicável) | — | DARF | 0,33%/dia |
| 31/05 | Folha de pagamento (maio) | R$ 12.000 | Conta bancária | CLT — passivo trabalhista |

🔴 **Críticos do mês:** DAS (20/05), FGTS (07/05), Folha (31/05)
⚠️ **Atenção:** 20/05 é terça — não há feriado. Pagar com antecedência recomendada.

---
