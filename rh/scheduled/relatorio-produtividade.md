# Relatório Mensal de Produtividade da Equipe

Consolida indicadores de RH do mês — produtividade, absenteísmo, turnover e clima organizacional.

## Frequência
**Mensal** — sugerido no último dia útil do mês às 17h

## Como agendar com Claude Code

```bash
# Criar agendamento no último dia útil do mês às 17h
claude schedule create \
  --name "relatorio-produtividade-rh" \
  --cron "0 17 28-31 * *" \
  --prompt-file rh/scheduled/relatorio-produtividade.md \
  --output-format markdown
```

---

## Prompt

```
Você é o gerente de RH da empresa [NOME_DA_EMPRESA].

Gere o Relatório Mensal de RH de [MÊS/ANO]:

**EQUIPE:**
- Total de colaboradores: [NÚMERO]
- CLT: [X] | PJ: [X] | Estagiários: [X]
- Novas contratações no mês: [NÚMERO]
- Desligamentos no mês: [NÚMERO] (motivo: [voluntário/involuntário])

**ABSENTEÍSMO:**
- Dias de falta por atestado: [TOTAL DIAS]
- Dias de falta não justificada: [TOTAL DIAS]
- Colaborador com mais faltas: [NOME ou "nenhum"]
- Atrasos registrados: [TOTAL]

**HORAS TRABALHADAS:**
- Banco de horas positivo acumulado: [HORAS]
- Banco de horas negativo: [HORAS]
- Horas extras pagas: [HORAS e VALOR]

**CLIMA E ENGAJAMENTO:**
- Resultado do check-in semanal (média): [BOM/REGULAR/RUIM]
- Feedbacks recebidos da equipe (resumo): [COLE OU DESCREVA]
- Conflitos ou situações relevantes: [DESCREVA OU "nenhum"]

**CUSTOS DE PESSOAL:**
- Folha total: R$ [VALOR]
- Encargos: R$ [VALOR]
- Benefícios: R$ [VALOR]
- Custo total de pessoal: R$ [VALOR]
- % do faturamento: [CALCULE]

Gere:
1. Dashboard de RH com os indicadores principais
2. Taxa de turnover do mês (e acumulada no ano)
3. Taxa de absenteísmo (e comparação com benchmark: < 3,5% é saudável)
4. Análise de clima: sinal 🟢🟡🔴 com justificativa
5. 3 alertas ou ações prioritárias para o próximo mês
6. Custo médio por colaborador
```

---

## Exemplo de saída

---
📊 **RELATÓRIO RH — MAIO/2025 | [NOME_DA_EMPRESA]**

👥 **Equipe:** 12 colaboradores | +1 contratação | 0 desligamentos  
🔄 **Turnover:** 0% no mês | 8,3% acumulado no ano (benchmark: < 15% ✅)

📅 **Absenteísmo:** 3,2% (8 dias no total) ✅ *benchmark: < 3,5%*  
⏰ **Banco de horas positivo:** 47h acumuladas — atenção, precisam ser compensadas

💰 **Custo de pessoal:** R$ 22.400 (42% do faturamento) 🔴 *acima do ideal (35%)*  
💼 **Custo médio por colaborador:** R$ 1.867/mês

🌡️ **Clima:** 🟡 Regular — check-ins mostram equipe cansada após sprint de 6 semanas.

⚠️ **Alertas para Junho:**
1. Compensar banco de horas antes que vire passivo trabalhista (risco CLT)
2. Conversa individual com 2 colaboradores com absenteísmo acima da média
3. Reduzir custo de pessoal de 42% para 38% — avaliar redistribuição de tarefas antes de contratar

---
