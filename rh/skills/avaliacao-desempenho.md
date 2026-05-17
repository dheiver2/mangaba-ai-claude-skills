# Avaliação de Desempenho

Gera um formulário de avaliação de desempenho e analisa os resultados com orientações para feedbacks.

## Quando usar
- Avaliações semestrais ou anuais
- Período de experiência (45 e 90 dias)
- Revisão salarial baseada em mérito

---

## Prompt para CRIAR o formulário

```
Você é um especialista em gestão de pessoas para PMEs brasileiras.

Crie um formulário de avaliação de desempenho para [NOME_DA_EMPRESA]:

**Cargo avaliado:** [CARGO]
**Tipo de avaliação:** [Autoavaliação / Avaliação do gestor / 360° (pares + gestor + auto)]
**Período avaliado:** [PERÍODO, ex: Jan-Jun 2025]
**Objetivo:** [Revisão salarial / Desenvolvimento / Período de experiência]

**Competências a avaliar:**
[Ex:
- Qualidade das entregas
- Cumprimento de prazos
- Comunicação e relacionamento
- Proatividade e autonomia
- Aprendizado contínuo
- Alinhamento com a cultura]

**Escala:** [1-5 / 1-10 / Abaixo/Dentro/Acima do esperado]

Gere:
1. Formulário completo com todas as competências
2. Instruções de preenchimento (para o avaliador e para o avaliado)
3. Seção de metas: avaliação das metas do período + definição de metas para o próximo
4. Campo de pontos fortes e pontos de desenvolvimento
5. Campo de feedback livre (qualitativo)
6. Seção de PDI (Plano de Desenvolvimento Individual) simplificado
7. Orientações para conduzir a conversa de feedback
```

---

## Prompt para ANALISAR os resultados

```
Analise os resultados da avaliação de desempenho do colaborador [NOME], cargo [CARGO]:

**Notas por competência (escala 1-5):**
[Ex:
- Qualidade das entregas: 4
- Cumprimento de prazos: 3
- Comunicação: 4
- Proatividade: 2
- Aprendizado: 5
- Cultura: 5]

**Comentários do gestor:** [COLE OS COMENTÁRIOS]
**Autoavaliação (se houver):** [COLE]
**Metas do período:** [QUAIS ERAM E SE FORAM ATINGIDAS]

Gere:
1. Score geral (média ponderada se houver pesos)
2. Pontos fortes destacados (top 2)
3. Áreas de desenvolvimento prioritárias (top 2)
4. Sugestão de PDI com 3 ações concretas
5. Sugestão de meta para o próximo período
6. Script de feedback (o que falar na conversa 1:1)
7. Recomendação sobre ajuste salarial (baseado no resultado, sem valor)
```

---

## Exemplo de script de feedback

> **Como abrir a conversa:**
> "Obrigado por se dedicar a essa avaliação. Antes de compartilhar minha visão, quero ouvir a sua — como você avaliou seu próprio desempenho neste semestre?"
>
> **Ao destacar ponto forte:**
> "Quero começar reconhecendo [COMPETÊNCIA]. Em [SITUAÇÃO ESPECÍFICA], você demonstrou [COMPORTAMENTO] e o resultado foi [IMPACTO]. Isso faz diferença real no time."
>
> **Ao abordar ponto de melhoria:**
> "Uma área que acredito que você pode se desenvolver é [ÁREA]. Minha percepção é que [COMPORTAMENTO OBSERVADO]. O que você acha? O que poderia ajudar você a avançar nisso?"
