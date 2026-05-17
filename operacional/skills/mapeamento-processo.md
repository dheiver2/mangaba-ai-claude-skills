# Mapeamento de Processo

Documenta e analisa um processo da empresa, identifica ineficiências e propõe melhorias com ganho de tempo estimado.

## Quando usar
- Antes de contratar alguém (documentar o que a pessoa vai fazer)
- Quando o processo depende de uma só pessoa e vira gargalo
- Para treinar novos colaboradores mais rápido
- Antes de automatizar uma tarefa

---

## Prompt

```
Você é um especialista em melhoria de processos para PMEs brasileiras.

Mapeie e analise o processo abaixo da empresa [NOME_DA_EMPRESA]:

**Nome do processo:** [Ex: "Onboarding de novo cliente", "Fechamento de venda", "Emissão de nota fiscal"]
**Responsável atual:** [NOME/CARGO]
**Frequência:** [Diário / Semanal / Por demanda — quantas vezes por semana/mês?]
**Tempo médio atual:** [X horas/minutos]
**Ferramentas usadas:** [Ex: WhatsApp, planilha, sistema X, email]

**Passo a passo atual (descreva como é feito hoje):**
[Ex:
1. Cliente entra em contato pelo WhatsApp
2. Vendedor anota os dados em papel
3. Passa para o financeiro por WhatsApp
4. Financeiro cria proposta no Word
5. Envia por email
6. Aguarda resposta...]

**Problemas que ocorrem:**
[Ex: dados se perdem, demora muito, cliente reclama, erros frequentes]

Gere:
1. Fluxograma textual do processo atual (AS-IS)
2. Identificação dos 3 maiores gargalos com impacto estimado
3. Processo otimizado sugerido (TO-BE) — fluxograma + descrição
4. Ganho de tempo estimado com a otimização
5. Ferramentas recomendadas para automatizar etapas (preferencialmente gratuitas ou baratas)
6. Checklist para implementação da melhoria
7. Como documentar para que qualquer pessoa da equipe execute
```

---

## Exemplo de saída (trecho)

**Gargalo #1 — Anotação manual em papel**
Impacto: ~30 min de retrabalho por cliente (digitalizar + repassar). Risco: perda de dados.
Solução: Formulário Google Forms com preenchimento direto no atendimento → alimenta planilha automaticamente.
Ganho estimado: 25 min por atendimento.

**Processo TO-BE (resumo):**
Cliente → formulário (2 min) → planilha automática → financeiro recebe notificação → proposta gerada pelo Claude → enviada em 10 min.
Tempo total: 15 min (vs. 55 min atuais) — **redução de 73%**
