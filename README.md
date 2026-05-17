# Mangaba AI — Claude Skills para PMEs

> Coleção de prompts, skills agendadas e artefatos prontos para pequenas e médias empresas usarem com Claude (claude.ai ou Claude Code).

---

## O que é isso?

Este repositório reúne **skills práticas** organizadas por área de negócio. Cada skill é um prompt otimizado que você cola no Claude e recebe um resultado profissional imediatamente — sem precisar saber escrever prompt.

Também inclui **Scheduled Tasks** (tarefas agendadas) para automatizar relatórios e rotinas, e **Artefatos** prontos para editar e usar.

---

## Estrutura

```
mangaba-ai-claude-skills/
├── financeiro/          # Fluxo de caixa, faturas, DRE
│   ├── skills/          # Prompts de análise
│   ├── scheduled/       # Tarefas automáticas (diária/semanal/mensal)
│   └── artefatos/       # Templates de documentos
├── marketing/           # Redes sociais, email, conteúdo
│   ├── skills/
│   ├── scheduled/
│   └── artefatos/
├── atendimento/         # FAQ, respostas, pesquisa de satisfação
│   ├── skills/
│   ├── scheduled/
│   └── artefatos/
└── rh/                  # Vagas, onboarding, avaliações
    ├── skills/
    ├── scheduled/
    └── artefatos/
```

---

## Como usar

### Opção 1 — Claude.ai (sem instalação)
1. Abra [claude.ai](https://claude.ai)
2. Abra o arquivo `.md` da skill desejada
3. Copie o bloco `## Prompt` e cole no Claude
4. Preencha os campos entre `[colchetes]` com seus dados

### Opção 2 — Claude Code CLI (agendamentos)
```bash
# Instalar Claude Code
npm install -g @anthropic-ai/claude-code

# Executar uma skill agendada
claude --print "$(cat financeiro/scheduled/relatorio-diario-vendas.md)"

# Criar agendamento recorrente (exemplo: todo dia às 8h)
claude schedule create --cron "0 8 * * *" --file financeiro/scheduled/relatorio-diario-vendas.md
```

---

## Áreas disponíveis

| Área | Skills | Scheduled | Artefatos |
|------|--------|-----------|-----------|
| [Financeiro](./financeiro/) | 3 | 3 | 3 |
| [Marketing Digital](./marketing/) | 3 | 2 | 2 |
| [Atendimento ao Cliente](./atendimento/) | 3 | 1 | 2 |
| [RH e Pessoas](./rh/) | 3 | 2 | 2 |

---

## Legenda dos arquivos

- `skills/` — Prompts avulsos, use quando precisar
- `scheduled/` — Prompts para rodar automaticamente (diário/semanal/mensal)
- `artefatos/` — Templates de documentos profissionais para gerar com Claude

---

## Desenvolvido por

**Mangaba AI** — Inteligência Artificial para empresas brasileiras  
Site: [mangaba.ai](https://mangaba.ai)

---

*Licença MIT — use, adapte e compartilhe livremente.*
