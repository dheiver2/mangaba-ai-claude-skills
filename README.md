<p align="center">
  <img src="https://img.shields.io/badge/Mangaba_AI-Skills_para_PMEs-green?style=for-the-badge&logo=anthropic&logoColor=white" alt="Mangaba AI" />
</p>

<h1 align="center">🥭 Mangaba AI — Claude Skills para PMEs</h1>

<p align="center">
  <strong>35 prompts prontos, agendamentos automáticos e artefatos profissionais<br>para pequenas e médias empresas brasileiras usarem com Claude.</strong>
</p>

<p align="center">
  <a href="#-áreas-disponíveis"><img src="https://img.shields.io/badge/4_Áreas-Financeiro_·_Marketing_·_Atendimento_·_RH-blue?style=flat-square" /></a>
  <a href="#-como-usar"><img src="https://img.shields.io/badge/Compatível-Claude.ai_e_Claude_Code-purple?style=flat-square&logo=anthropic" /></a>
  <img src="https://img.shields.io/badge/Idioma-Português_BR-009c3b?style=flat-square" />
  <img src="https://img.shields.io/badge/Licença-MIT-yellow?style=flat-square" />
  <img src="https://img.shields.io/github/stars/dheiver2/mangaba-ai-claude-skills?style=flat-square&color=orange" />
</p>

<br />

---

## O que é este repositório?

Uma coleção de **skills práticas do Claude** organizadas por área de negócio. Cada skill é um prompt otimizado — você preenche os campos em `[colchetes]`, cola no Claude e recebe um resultado profissional em segundos, sem precisar saber escrever prompt.

Também inclui **Scheduled Tasks** para automatizar relatórios e rotinas diárias, e **Artefatos** prontos para editar e usar com clientes.

> **Para quem é?** Donos de PMEs, gestores e equipes que querem usar IA no dia a dia sem precisar de um especialista técnico ao lado.

---

## Áreas disponíveis

<table>
  <thead>
    <tr>
      <th>Área</th>
      <th>O que resolve</th>
      <th>Skills</th>
      <th>Scheduled</th>
      <th>Artefatos</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="./financeiro/">💰 Financeiro</a></td>
      <td>Fluxo de caixa, DRE, faturas, previsão de receita</td>
      <td align="center">3</td>
      <td align="center">3</td>
      <td align="center">3</td>
    </tr>
    <tr>
      <td><a href="./marketing/">📣 Marketing Digital</a></td>
      <td>Posts, email marketing, calendário editorial</td>
      <td align="center">3</td>
      <td align="center">2</td>
      <td align="center">2</td>
    </tr>
    <tr>
      <td><a href="./atendimento/">💬 Atendimento ao Cliente</a></td>
      <td>Respostas, FAQ, NPS, scripts WhatsApp</td>
      <td align="center">3</td>
      <td align="center">1</td>
      <td align="center">2</td>
    </tr>
    <tr>
      <td><a href="./rh/">👥 RH e Pessoas</a></td>
      <td>Vagas, entrevistas, onboarding, avaliações</td>
      <td align="center">3</td>
      <td align="center">2</td>
      <td align="center">2</td>
    </tr>
  </tbody>
</table>

**35 arquivos · 3 tipos · 4 áreas · 100% em português**

---

## Como usar

### Opção 1 — Claude.ai (zero instalação)

```
1. Abra claude.ai
2. Abra o arquivo .md da skill desejada neste repositório
3. Copie o bloco "## Prompt"
4. Cole no Claude e substitua os [CAMPOS] com seus dados reais
5. Pronto — resultado profissional em segundos
```

### Opção 2 — Claude Code CLI (com agendamentos)

```bash
# 1. Instalar o Claude Code
npm install -g @anthropic-ai/claude-code

# 2. Clonar este repositório
git clone https://github.com/dheiver2/mangaba-ai-claude-skills.git
cd mangaba-ai-claude-skills

# 3. Rodar uma skill manualmente
claude --print "$(cat financeiro/skills/analise-fluxo-caixa.md)"

# 4. Criar um agendamento automático (exemplo: relatório todo dia às 8h)
claude schedule create \
  --name "relatorio-diario" \
  --cron "0 8 * * 1-5" \
  --prompt-file financeiro/scheduled/relatorio-diario-vendas.md
```

---

## O que tem dentro de cada arquivo

Cada skill segue o mesmo padrão para facilitar o uso:

```
# Nome da Skill
Descrição do que faz em uma linha.

## Quando usar
Situações ideais para acionar esta skill.

## Prompt              ← copie este bloco e cole no Claude
[...]

## Exemplo de saída    ← veja antes de usar
[...]
```

Os arquivos em `scheduled/` incluem também o **comando exato** para criar o agendamento no Claude Code.

---

## Mapa completo das skills

<details>
<summary><strong>💰 Financeiro</strong> — clique para expandir</summary>

| Arquivo | Tipo | O que faz |
|---------|------|-----------|
| [analise-fluxo-caixa.md](./financeiro/skills/analise-fluxo-caixa.md) | Skill | Analisa entradas/saídas e sugere ações de liquidez |
| [analise-despesas.md](./financeiro/skills/analise-despesas.md) | Skill | Identifica despesas acima do benchmark e onde cortar |
| [previsao-receita.md](./financeiro/skills/previsao-receita.md) | Skill | Forecast trimestral (3 cenários: pessimista/base/otimista) |
| [relatorio-diario-vendas.md](./financeiro/scheduled/relatorio-diario-vendas.md) | ⏰ Diário | Resumo de vendas do dia vs meta — ideal às 18h |
| [resumo-semanal.md](./financeiro/scheduled/resumo-semanal.md) | ⏰ Semanal | Consolidado da semana: receitas, despesas, inadimplência |
| [fechamento-mensal.md](./financeiro/scheduled/fechamento-mensal.md) | ⏰ Mensal | DRE simplificada + metas para o próximo mês |
| [fatura.md](./financeiro/artefatos/fatura.md) | 📄 Artefato | Fatura profissional pronta para enviar ao cliente |
| [proposta-comercial.md](./financeiro/artefatos/proposta-comercial.md) | 📄 Artefato | Proposta completa com diagnóstico, solução e preços |
| [relatorio-dre.md](./financeiro/artefatos/relatorio-dre.md) | 📄 Artefato | DRE detalhada com margens e diagnóstico |

</details>

<details>
<summary><strong>📣 Marketing Digital</strong> — clique para expandir</summary>

| Arquivo | Tipo | O que faz |
|---------|------|-----------|
| [post-redes-sociais.md](./marketing/skills/post-redes-sociais.md) | Skill | Posts prontos para Instagram, LinkedIn e WhatsApp |
| [email-marketing.md](./marketing/skills/email-marketing.md) | Skill | Emails de boas-vindas, promoção, reativação e cobrança |
| [criacao-conteudo.md](./marketing/skills/criacao-conteudo.md) | Skill | Artigos para blog/LinkedIn com SEO otimizado |
| [calendario-editorial.md](./marketing/scheduled/calendario-editorial.md) | ⏰ Semanal | Planejamento da semana seguinte com posts prontos |
| [relatorio-engajamento.md](./marketing/scheduled/relatorio-engajamento.md) | ⏰ Mensal | Análise de resultados e recomendações para o próximo mês |
| [plano-marketing-mensal.md](./marketing/artefatos/plano-marketing-mensal.md) | 📄 Artefato | Plano completo: estratégia, canais, orçamento e KPIs |
| [briefing-campanha.md](./marketing/artefatos/briefing-campanha.md) | 📄 Artefato | Briefing para agência ou freelancer de marketing |

</details>

<details>
<summary><strong>💬 Atendimento ao Cliente</strong> — clique para expandir</summary>

| Arquivo | Tipo | O que faz |
|---------|------|-----------|
| [resposta-reclamacao.md](./atendimento/skills/resposta-reclamacao.md) | Skill | Respostas profissionais para reclamações (email, WhatsApp, Reclame Aqui) |
| [gerador-faq.md](./atendimento/skills/gerador-faq.md) | Skill | FAQ completo para site, WhatsApp Business ou chatbot |
| [pesquisa-satisfacao.md](./atendimento/skills/pesquisa-satisfacao.md) | Skill | Cria pesquisas NPS/CSAT e analisa os resultados |
| [relatorio-atendimentos.md](./atendimento/scheduled/relatorio-atendimentos.md) | ⏰ Semanal | Dashboard de tickets, SLA e clientes em risco de churn |
| [templates-email.md](./atendimento/artefatos/templates-email.md) | 📄 Artefato | 4 templates prontos: confirmação, cobrança, encerramento |
| [script-whatsapp.md](./atendimento/artefatos/script-whatsapp.md) | 📄 Artefato | Scripts para WhatsApp Business (boas-vindas, fora do horário, follow-up) |

</details>

<details>
<summary><strong>👥 RH e Pessoas</strong> — clique para expandir</summary>

| Arquivo | Tipo | O que faz |
|---------|------|-----------|
| [descricao-vaga.md](./rh/skills/descricao-vaga.md) | Skill | Vaga atrativa e inclusiva para LinkedIn, Indeed ou Gupy |
| [roteiro-entrevista.md](./rh/skills/roteiro-entrevista.md) | Skill | Perguntas STAR estruturadas por competência |
| [avaliacao-desempenho.md](./rh/skills/avaliacao-desempenho.md) | Skill | Formulário de avaliação + script de feedback |
| [check-in-equipe.md](./rh/scheduled/check-in-equipe.md) | ⏰ Semanal | Pauta de 15 min para alinhamento do time |
| [relatorio-produtividade.md](./rh/scheduled/relatorio-produtividade.md) | ⏰ Mensal | Turnover, absenteísmo, custo de pessoal e clima |
| [onboarding-colaborador.md](./rh/artefatos/onboarding-colaborador.md) | 📄 Artefato | Plano 30/60/90 dias para novo colaborador |
| [politica-home-office.md](./rh/artefatos/politica-home-office.md) | 📄 Artefato | Política de trabalho remoto alinhada à CLT |

</details>

---

## Legenda

| Ícone | Tipo | Como usar |
|-------|------|-----------|
| Skill | Prompt avulso | Cole no Claude quando precisar |
| ⏰ Scheduled | Tarefa agendada | Use com `claude schedule create` |
| 📄 Artefato | Template de documento | Gera um documento profissional completo |

---

## Contribuindo

Tem uma skill que faria diferença para PMEs brasileiras? Contribuições são bem-vindas.

1. Fork este repositório
2. Crie sua branch: `git checkout -b skill/nome-da-skill`
3. Siga o padrão dos arquivos existentes (seções: descrição, quando usar, prompt, exemplo)
4. Abra um Pull Request com uma breve descrição

---

## Desenvolvido por

<p>
  <strong>Mangaba AI</strong> — Inteligência Artificial para empresas brasileiras<br>
  Acesse: <a href="https://mangaba.ai">mangaba.ai</a>
</p>

---

<p align="center">
  <sub>Licença MIT — use, adapte e compartilhe livremente.</sub><br>
  <sub>Feito com ❤️ para as PMEs do Brasil</sub>
</p>
