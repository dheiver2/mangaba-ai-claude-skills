# Contexto do Projeto — Mangaba AI Claude Skills

Este repositório contém prompts e skills Claude para PMEs brasileiras.

## Convenções

- Todos os prompts são em português do Brasil
- Campos variáveis usam `[COLCHETES_MAIÚSCULOS]`
- Cada arquivo tem: descrição, quando usar, prompt pronto, e exemplo de saída
- Skills de `scheduled/` incluem o comando Claude Code para agendar

## Estrutura de cada arquivo de skill

```
# Título da Skill
Descrição curta do que faz.

## Quando usar
Situações ideais para usar esta skill.

## Frequência (apenas scheduled/)
diária / semanal / mensal

## Como agendar (apenas scheduled/)
Comando claude schedule...

## Prompt
[Prompt pronto para copiar]

## Exemplo de saída
[Exemplo do resultado esperado]
```

## Tom e estilo dos prompts

- Linguagem profissional mas acessível
- Resultados sempre em formato pronto para usar (não para editar muito)
- Foco em PMEs brasileiras: contexto fiscal BR, LGPD, CLT quando relevante
