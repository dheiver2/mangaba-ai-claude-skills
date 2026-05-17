# Relatório Trimestral de Impostos

Consolida todos os impostos pagos no trimestre, analisa a carga tributária e antecipa obrigações do próximo período.

## Frequência
**Trimestral** — sugerido no 1º dia útil de abril, julho, outubro e janeiro às 9h

## Como agendar com Claude Code

```bash
claude schedule create \
  --name "relatorio-impostos-trimestral" \
  --cron "0 9 1 1,4,7,10 *" \
  --prompt-file fiscal/scheduled/relatorio-impostos.md
```

---

## Prompt

```
Você é o controller fiscal da empresa [NOME_DA_EMPRESA].

Gere o Relatório Trimestral de Impostos do [TRIMESTRE/ANO] (meses: [MÊS1], [MÊS2], [MÊS3]):

**IMPOSTOS PAGOS NO TRIMESTRE:**
[Mês 1:]
- DAS / IRPJ / CSLL: R$
- FGTS: R$
- INSS patronal: R$
- ISS (se aplicável): R$
- Outros: R$

[Repita para Mês 2 e Mês 3]

**FATURAMENTO DO TRIMESTRE:**
- Mês 1: R$
- Mês 2: R$
- Mês 3: R$
- Total: R$

**DECLARAÇÕES ENTREGUES:**
[Liste as que foram entregues e as pendentes]

Gere:
1. Total de impostos pagos no trimestre
2. Carga tributária efetiva (impostos ÷ faturamento) — benchmarked por regime
3. Evolução trimestre a trimestre (se houver histórico)
4. Declarações pendentes ou atrasadas
5. Obrigações especiais do próximo trimestre (ex: IRPF dos sócios, DEFIS, DASN-SIMEI)
6. Estimativa de impostos para o próximo trimestre
7. Alerta de risco fiscal (passivos, atrasos, inconsistências)
```
