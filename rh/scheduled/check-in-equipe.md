# Check-in Semanal da Equipe

Gera perguntas de check-in para reunião rápida de alinhamento com o time — identifica bloqueios antes que virem problemas.

## Frequência
**Semanal** — sugerido toda segunda-feira às 8h30

## Como agendar com Claude Code

```bash
# Criar agendamento toda segunda às 8h30
claude schedule create \
  --name "checkin-equipe" \
  --cron "30 8 * * 1" \
  --prompt-file rh/scheduled/check-in-equipe.md \
  --output-format markdown
```

---

## Prompt

```
Você é um gestor de equipes de PMEs brasileiras.

Crie o Check-in Semanal para a semana de [DATA_SEGUNDA] a [DATA_SEXTA] da equipe de [NOME_DA_EMPRESA]:

**Tamanho da equipe:** [NÚMERO] pessoas
**Modelo:** [Presencial / Híbrido / Remoto]
**Duração do check-in:** [15 min / 30 min]
**Contexto da semana:**
- Projetos em andamento: [LISTE]
- Entregas previstas para a semana: [LISTE]
- Algum evento especial: [ex: "apresentação para cliente na quinta", "prazo de entrega sexta"]

Gere:
1. Pauta estruturada para a reunião de check-in (com tempo de cada parte)
2. 3 perguntas de abertura (humor e energia do time)
3. Revisão da semana anterior: template para cada pessoa reportar em 1 minuto
4. Prioridades desta semana: o que cada um precisa entregar
5. Identificação de bloqueios: pergunta para descobrir impedimentos
6. Uma pergunta de desenvolvimento pessoal (rotação semanal de temas)
7. Encerramento motivacional (frase ou desafio da semana)

Formato: reunião ágil, sem enrolação. Máximo 15 minutos se seguido à risca.
```

---

## Exemplo de saída

---
📋 **CHECK-IN SEMANAL — 19/05/2025 | [NOME_DA_EMPRESA]**

⏱️ Duração: 15 minutos | Facilitador: [NOME DO GESTOR]

**8h30 — Abertura (2 min)**
> "Em uma palavra: como você está chegando essa semana?"
*(Cada um responde em 5 segundos — dá a temperatura do time)*

**8h32 — Semana passada (3 min)**
Cada pessoa responde em 30 segundos:
- ✅ "O que eu entreguei que vale destacar:"
- ⚠️ "O que ficou pendente e por quê:"

**8h35 — Esta semana (5 min)**
- 🎯 "Minha prioridade #1 esta semana é:"
- 🚧 "Preciso de ajuda ou estou bloqueado em:"

**8h40 — Pergunta da semana (3 min)**
> "Se você fosse dar um conselho para si mesmo 1 ano atrás, qual seria?"
*(Tema: aprendizado e crescimento)*

**8h43 — Encerramento (2 min)**
> "Desafio da semana: esta semana, cada um vai agradecer alguém da equipe por algo específico que fez. Vamos ver na sexta."

---
