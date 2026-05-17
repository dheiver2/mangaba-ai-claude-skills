# Auditoria Mensal de Processos

Avalia a aderência aos processos definidos, identifica desvios e atualiza os SOPs quando necessário.

## Frequência
**Mensal** — sugerido no último dia útil do mês às 14h

## Como agendar com Claude Code

```bash
claude schedule create \
  --name "auditoria-processos" \
  --cron "0 14 28-31 * *" \
  --prompt-file operacional/scheduled/auditoria-processos.md
```

---

## Prompt

```
Você é o gerente de qualidade da empresa [NOME_DA_EMPRESA].

Faça a Auditoria Mensal de Processos de [MÊS/ANO]:

**PROCESSOS MAPEADOS (liste os que existem documentados):**
[Ex: processo de vendas, onboarding de cliente, emissão de NF, atendimento via WhatsApp]

**DESVIOS OBSERVADOS NO MÊS:**
[Ex:
- Proposta enviada sem aprovação do gestor em 3 casos
- 2 NFs emitidas com dados errados
- Onboarding pulado para clientes "urgentes" em 5 casos]

**PROCESSOS QUE MUDARAM NA PRÁTICA (mas o SOP não foi atualizado):**
[Descreva o que mudou]

**VOLUME DE EXECUÇÕES POR PROCESSO:**
[Ex: vendas: 12x / onboarding: 8x / NF: 45x]

Gere:
1. Score de aderência por processo (% de execuções sem desvio)
2. Ranking de processos por risco (qual gera mais problema quando não seguido)
3. Causa raiz dos desvios (processo ruim? treinamento? pressão de prazo?)
4. SOPs que precisam ser atualizados
5. Treinamento necessário (quem, sobre o quê)
6. 3 melhorias de processo para implementar no próximo mês
```
