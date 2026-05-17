# Análise de Gargalo Operacional

Identifica o principal ponto de estrangulamento da operação que está limitando crescimento ou gerando retrabalho.

## Quando usar
- Quando a empresa cresce mas os problemas crescem junto
- Quando um setor está sempre atrasado
- Antes de contratar (às vezes o gargalo não é falta de gente)
- Quando clientes reclamam de prazo ou qualidade

---

## Prompt

```
Você é um consultor de operações especializado em PMEs brasileiras.

Analise os gargalos operacionais da empresa [NOME_DA_EMPRESA], segmento [SEGMENTO]:

**Contexto:**
- Faturamento atual: R$ [VALOR]/mês
- Número de colaboradores: [NÚMERO]
- Capacidade máxima atual: [X clientes/pedidos/projetos por mês]
- Demanda atual: [Y clientes/pedidos — está acima ou abaixo da capacidade?]

**Sintomas observados (marque os que se aplicam):**
[Ex:
- Prazo de entrega aumentou nos últimos meses
- Erros e retrabalho frequentes em [ÁREA]
- Uma pessoa específica é sempre o ponto de espera
- Clientes reclamam de demora na resposta
- A equipe faz hora extra mas o volume não aumenta
- Acúmulo de tarefas na fila de [ÁREA]]

**Mapeamento básico do fluxo (da venda à entrega):**
[Descreva as etapas principais, ex: prospecção → proposta → assinatura → onboarding → execução → entrega → cobrança]

**Onde você acha que está o gargalo:** [DESCREVA ou "não sei"]

**Dados de tempo (se disponíveis):**
[Ex: proposta leva 3 dias, onboarding 2 semanas, execução 1 semana]

Gere:
1. Identificação do gargalo principal (com fundamentação)
2. Gargalos secundários (até 3)
3. Impacto financeiro estimado do gargalo (receita perdida ou custo de retrabalho)
4. Causa raiz (processo / pessoa / ferramenta / volume?)
5. Solução de curto prazo (implementar esta semana)
6. Solução de médio prazo (1-3 meses)
7. Indicadores para monitorar se o gargalo foi resolvido
```
