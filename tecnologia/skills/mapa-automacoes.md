# Mapa de Automações para PME

Identifica quais tarefas repetitivas da empresa podem ser automatizadas — com ferramentas acessíveis e custo estimado.

## Quando usar
- Quando a equipe está sobrecarregada com tarefas manuais e repetitivas
- Antes de contratar (às vezes a automação resolve)
- Planejamento de tecnologia para o próximo semestre

---

## Prompt

```
Você é um especialista em automação de processos para PMEs brasileiras.

Mapeie as oportunidades de automação para [NOME_DA_EMPRESA], segmento [SEGMENTO]:

**Tarefas manuais e repetitivas que a equipe faz hoje:**
[Liste tudo que é feito manualmente e que se repete, ex:
- Enviar email de confirmação para cada novo cliente
- Copiar dados do formulário do site para planilha
- Lembrar clientes de pagamentos vencidos por WhatsApp
- Gerar relatório semanal de vendas toda segunda
- Publicar posts nas redes sociais
- Emitir NF para cada venda fechada]

**Ferramentas que já usam:**
[Ex: Google Workspace, WhatsApp Business, Instagram, sistema de NF, planilhas]

**Orçamento para automação:** R$ [VALOR]/mês ou "zero — só ferramentas gratuitas"

**Nível técnico:** [Básico — só arrastar e soltar / Intermediário / Avançado — pode usar código]

Para cada tarefa, gere:
1. Nome da automação
2. Ferramenta recomendada (Zapier / Make / n8n / Google Apps Script / nativo)
3. Custo estimado (R$/mês)
4. Tempo economizado por mês
5. Dificuldade de implementação: 🟢 Fácil / 🟡 Médio / 🔴 Precisa de ajuda técnica
6. Prioridade: impacto × facilidade

Ao final: ranking de automações por ROI (retorno sobre o investimento de tempo e dinheiro).
```

---

## Exemplo de saída (trecho)

| # | Automação | Ferramenta | Custo | Tempo economizado | Dificuldade |
|---|-----------|------------|-------|-------------------|-------------|
| 1 | Email boas-vindas automático | Gmail + Zapier | Grátis | 2h/semana | 🟢 Fácil |
| 2 | Cobrança automática WhatsApp | Zapi + Planilha | R$ 89/mês | 5h/semana | 🟡 Médio |
| 3 | Relatório semanal de vendas | Claude Code | R$ 20/mês | 3h/semana | 🟢 Fácil |
| 4 | NF automática após pagamento | NFe.io + Asaas | R$ 49/mês | 4h/semana | 🟡 Médio |

**ROI top 1:** Cobrança automática WhatsApp — R$ 89/mês de ferramenta, recupera em média R$ 800-1.500/mês em inadimplência + 5h da equipe.
