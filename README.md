<p align="center">
  <img src="https://img.shields.io/badge/Mangaba_AI-Skills_para_PMEs-green?style=for-the-badge&logo=anthropic&logoColor=white" alt="Mangaba AI" />
</p>

<h1 align="center">🥭 Mangaba AI — Claude Skills para PMEs</h1>

<p align="center">
  <strong>75 prompts prontos, agendamentos automáticos e artefatos profissionais<br>para pequenas e médias empresas brasileiras usarem com Claude.</strong>
</p>

<p align="center">
  <a href="#-áreas-disponíveis"><img src="https://img.shields.io/badge/9_Áreas-Financeiro_·_Marketing_·_Vendas_·_RH_e_mais-blue?style=flat-square" /></a>
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

**75 arquivos · 9 áreas de negócio · 3 tipos de skill · 100% em português**

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
    <tr>
      <td><a href="./juridico/">⚖️ Jurídico</a></td>
      <td>Contratos, LGPD, notificações, compliance</td>
      <td align="center">3</td>
      <td align="center">2</td>
      <td align="center">2</td>
    </tr>
    <tr>
      <td><a href="./operacional/">⚙️ Operacional</a></td>
      <td>Processos, SOPs, checklists, continuidade</td>
      <td align="center">3</td>
      <td align="center">2</td>
      <td align="center">2</td>
    </tr>
    <tr>
      <td><a href="./vendas/">🤝 Vendas</a></td>
      <td>Prospecção, pipeline, follow-up, forecast</td>
      <td align="center">3</td>
      <td align="center">2</td>
      <td align="center">2</td>
    </tr>
    <tr>
      <td><a href="./fiscal/">🧾 Fiscal e Contábil</a></td>
      <td>Simples Nacional, regime tributário, calendário fiscal</td>
      <td align="center">3</td>
      <td align="center">2</td>
      <td align="center">2</td>
    </tr>
    <tr>
      <td><a href="./tecnologia/">💻 Tecnologia e TI</a></td>
      <td>Seleção de software, segurança, automações, backup</td>
      <td align="center">3</td>
      <td align="center">2</td>
      <td align="center">2</td>
    </tr>
  </tbody>
</table>

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

<details>
<summary><strong>⚖️ Jurídico</strong> — clique para expandir</summary>

| Arquivo | Tipo | O que faz |
|---------|------|-----------|
| [revisao-contrato.md](./juridico/skills/revisao-contrato.md) | Skill | Analisa contratos, identifica riscos e sugere renegociações |
| [notificacao-extrajudicial.md](./juridico/skills/notificacao-extrajudicial.md) | Skill | Notificação formal para cobrar dívidas ou exigir cumprimento de contrato |
| [conformidade-lgpd.md](./juridico/skills/conformidade-lgpd.md) | Skill | Diagnóstico LGPD com score e plano de adequação |
| [monitoramento-prazos.md](./juridico/scheduled/monitoramento-prazos.md) | ⏰ Semanal | Alerta de vencimentos contratuais, alvarás e obrigações legais |
| [relatorio-compliance.md](./juridico/scheduled/relatorio-compliance.md) | ⏰ Mensal | Status de conformidade regulatória da empresa |
| [contrato-prestacao-servicos.md](./juridico/artefatos/contrato-prestacao-servicos.md) | 📄 Artefato | Contrato completo de prestação de serviços (base legal: CC/2002) |
| [politica-privacidade-lgpd.md](./juridico/artefatos/politica-privacidade-lgpd.md) | 📄 Artefato | Política de Privacidade completa e adequada à LGPD |

</details>

<details>
<summary><strong>⚙️ Operacional</strong> — clique para expandir</summary>

| Arquivo | Tipo | O que faz |
|---------|------|-----------|
| [mapeamento-processo.md](./operacional/skills/mapeamento-processo.md) | Skill | Documenta processo AS-IS, identifica gargalos e propõe TO-BE |
| [checklist-qualidade.md](./operacional/skills/checklist-qualidade.md) | Skill | Cria checklists objetivos para padronizar entregas |
| [analise-gargalo.md](./operacional/skills/analise-gargalo.md) | Skill | Identifica o principal ponto de estrangulamento da operação |
| [relatorio-operacional.md](./operacional/scheduled/relatorio-operacional.md) | ⏰ Semanal | Dashboard de capacidade, prazos, qualidade e alertas |
| [auditoria-processos.md](./operacional/scheduled/auditoria-processos.md) | ⏰ Mensal | Avalia aderência aos SOPs e identifica processos desatualizados |
| [procedimento-padrao-sop.md](./operacional/artefatos/procedimento-padrao-sop.md) | 📄 Artefato | SOP completo com fluxograma, etapas e checklist de conclusão |
| [plano-continuidade.md](./operacional/artefatos/plano-continuidade.md) | 📄 Artefato | Plano de continuidade de negócios para situações de crise |

</details>

<details>
<summary><strong>🤝 Vendas</strong> — clique para expandir</summary>

| Arquivo | Tipo | O que faz |
|---------|------|-----------|
| [script-prospeccao.md](./vendas/skills/script-prospeccao.md) | Skill | Scripts personalizados para LinkedIn, email frio e WhatsApp |
| [analise-pipeline.md](./vendas/skills/analise-pipeline.md) | Skill | Avalia o funil, aponta deals travados e receita previsível |
| [sequencia-follow-up.md](./vendas/skills/sequencia-follow-up.md) | Skill | Cadência de 5 touchpoints para reativar prospects frios |
| [relatorio-pipeline.md](./vendas/scheduled/relatorio-pipeline.md) | ⏰ Semanal | Snapshot do funil com prioridades e deals em risco |
| [forecast-vendas.md](./vendas/scheduled/forecast-vendas.md) | ⏰ Mensal | Projeção de fechamento com 3 cenários (feito no dia 20) |
| [playbook-vendas.md](./vendas/artefatos/playbook-vendas.md) | 📄 Artefato | Guia completo do processo comercial para treinar vendedores |
| [kit-objecoes.md](./vendas/artefatos/kit-objecoes.md) | 📄 Artefato | Respostas estratégicas para as 6 objeções mais comuns |

</details>

<details>
<summary><strong>🧾 Fiscal e Contábil</strong> — clique para expandir</summary>

| Arquivo | Tipo | O que faz |
|---------|------|-----------|
| [analise-regime-tributario.md](./fiscal/skills/analise-regime-tributario.md) | Skill | Compara Simples × Lucro Presumido × Lucro Real |
| [calculo-simples-nacional.md](./fiscal/skills/calculo-simples-nacional.md) | Skill | Verifica DAS, alíquota, fator "r" e oportunidades de redução |
| [planejamento-tributario.md](./fiscal/skills/planejamento-tributario.md) | Skill | Planejamento anual com top 5 oportunidades de economia fiscal |
| [calendario-fiscal.md](./fiscal/scheduled/calendario-fiscal.md) | ⏰ Mensal | Todas as obrigações fiscais do mês com datas e multas |
| [relatorio-impostos.md](./fiscal/scheduled/relatorio-impostos.md) | ⏰ Trimestral | Consolidado de impostos pagos e estimativa do próximo trimestre |
| [guia-obrigacoes-pme.md](./fiscal/artefatos/guia-obrigacoes-pme.md) | 📄 Artefato | Guia personalizado de todas as obrigações fiscais e legais |
| [checklist-fechamento-contabil.md](./fiscal/artefatos/checklist-fechamento-contabil.md) | 📄 Artefato | Checklist mensal para enviar documentos ao contador |

</details>

<details>
<summary><strong>💻 Tecnologia e TI</strong> — clique para expandir</summary>

| Arquivo | Tipo | O que faz |
|---------|------|-----------|
| [selecao-software.md](./tecnologia/skills/selecao-software.md) | Skill | Compara ferramentas e recomenda a melhor para o perfil da empresa |
| [politica-seguranca.md](./tecnologia/skills/politica-seguranca.md) | Skill | Política de segurança da informação acessível e prática |
| [mapa-automacoes.md](./tecnologia/skills/mapa-automacoes.md) | Skill | Identifica tarefas para automatizar com ROI estimado |
| [auditoria-ferramentas.md](./tecnologia/scheduled/auditoria-ferramentas.md) | ⏰ Mensal | Revisa assinaturas, acessos ativos e desperdícios de TI |
| [relatorio-custos-ti.md](./tecnologia/scheduled/relatorio-custos-ti.md) | ⏰ Mensal | Consolida gastos com tecnologia e analisa ROI por ferramenta |
| [mapa-stack-tecnologico.md](./tecnologia/artefatos/mapa-stack-tecnologico.md) | 📄 Artefato | Documentação completa de todas as ferramentas da empresa |
| [plano-backup-seguranca.md](./tecnologia/artefatos/plano-backup-seguranca.md) | 📄 Artefato | Plano de backup com regra 3-2-1 e procedimento de recuperação |

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
  Acesse: <a href="https://www.mangaba.ia.br/">mangaba.ia.br</a>
</p>

---

<p align="center">
  <sub>Licença MIT — use, adapte e compartilhe livremente.</sub><br>
  <sub>Feito com ❤️ para as PMEs do Brasil</sub>
</p>
