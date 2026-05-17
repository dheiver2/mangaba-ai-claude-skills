# Calendário Editorial Semanal

Gera automaticamente o planejamento de conteúdo da semana seguinte — posts prontos para aprovar e publicar.

## Frequência
**Semanal** — sugerido toda sexta-feira às 14h (planejando a próxima semana)

## Como agendar com Claude Code

```bash
# Criar agendamento semanal toda sexta às 14h
claude schedule create \
  --name "calendario-editorial" \
  --cron "0 14 * * 5" \
  --prompt-file marketing/scheduled/calendario-editorial.md \
  --output-format markdown
```

---

## Prompt

```
Você é o gerente de marketing da empresa [NOME_DA_EMPRESA], segmento [SEGMENTO].

Crie o Calendário Editorial para a semana de [DATA_SEGUNDA] a [DATA_SEXTA]:

**Informações da empresa:**
- Tom de voz: [ex: descontraído e próximo]
- Redes ativas: [Instagram / LinkedIn / WhatsApp]
- Frequência de posts: [X posts por semana]

**Contexto atual:**
- Promoções ou novidades para comunicar: [DESCREVA ou "nenhuma"]
- Datas comemorativas na semana: [ex: "Dia do Empreendedor — terça" ou "nenhuma"]
- Tema mensal da empresa: [ex: "junho é o mês da gestão financeira"]

**Objetivo da semana:** [Engajamento / Vendas / Educação / Mix]

Gere:
1. Calendário com data, rede, tipo de post e tema
2. Para cada post: legenda completa pronta + hashtags + sugestão de arte
3. Horários recomendados de publicação
4. 1 ideia para Stories interativo (enquete, quiz, caixa de perguntas)
5. 1 conteúdo para repostar/compartilhar (curadoria)

Formato de tabela + conteúdo completo de cada post.
```

---

## Exemplo de saída

| Data | Rede | Tipo | Tema | Horário |
|------|------|------|------|---------|
| Seg 19/05 | Instagram | Educativo | 5 erros financeiros de PMEs | 18h |
| Ter 20/05 | LinkedIn | Institucional | Case de sucesso cliente | 12h |
| Qua 21/05 | Instagram | Engajamento | Enquete: como você controla o caixa? | 19h |
| Qui 22/05 | WhatsApp | Oferta | Promoção semana | 10h |
| Sex 23/05 | Instagram | Entretenimento | Meme do empreendedor | 17h |

**POST SEGUNDA (Educativo — Instagram):**

---
5 erros financeiros que todo dono de PME comete (e como evitar) 🚨

1️⃣ Misturar conta pessoal com PJ
2️⃣ Não separar pró-labore do lucro
3️⃣ Não controlar o fluxo de caixa
4️⃣ Ignorar a inadimplência até virar problema
5️⃣ Não saber o CMV dos produtos

Você comete algum desses? Comenta aqui 👇

#GestaoFinanceira #PME #Empreendedorismo #MangabaAI
---
**Arte:** fundo azul escuro, lista numerada em branco, ícone de erro (X) em vermelho
