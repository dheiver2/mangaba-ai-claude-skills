# Pesquisa de Satisfação (NPS + CSAT)

Cria pesquisas de satisfação prontas para enviar por email ou WhatsApp e analisa os resultados recebidos.

## Quando usar
- Após entrega de produto ou serviço
- 30 dias após o cliente começar a usar
- Após resolução de reclamação
- Pesquisa trimestral da base de clientes

---

## Prompt para CRIAR a pesquisa

```
Crie uma pesquisa de satisfação para a empresa [NOME_DA_EMPRESA] para enviar após [MOMENTO: entrega do serviço / 30 dias de uso / resolução de suporte]:

**Canal de envio:** [Email / WhatsApp / Google Forms / TypeForm]
**Tempo máximo de resposta:** [ex: 2 minutos]
**Objetivo:** [Entender satisfação geral / Identificar problemas / Coletar depoimentos]

Inclua:
1. Mensagem de abertura (explica o porquê e quanto tempo leva)
2. NPS: "De 0 a 10, qual a probabilidade de indicar [EMPRESA] para um amigo?"
3. CSAT: "Como você avalia sua experiência neste atendimento?" (1-5 estrelas)
4. 2-3 perguntas abertas curtas (dependendo do objetivo)
5. Campo para depoimento (opcional, para usar como testemunho)
6. Mensagem de encerramento com agradecimento

Para WhatsApp: versão conversacional (1 pergunta por vez).
Para Email: versão em formato de formulário inline.
```

---

## Prompt para ANALISAR os resultados

```
Analise os resultados da pesquisa de satisfação da empresa [NOME_DA_EMPRESA] referente a [PERÍODO]:

**Total de respostas:** [NÚMERO]
**NPS (0-10):**
[Cole as respostas, ex:
- 10: 45 respostas
- 9: 38 respostas
- 8: 22 respostas
- 7: 15 respostas
- 6: 8 respostas
- 5 ou menos: 12 respostas]

**CSAT (1-5 estrelas):**
[Cole a distribuição]

**Principais comentários abertos:**
[Cole os mais relevantes, positivos e negativos]

Gere:
1. Score NPS calculado e classificação (Excelente/Bom/Regular/Ruim)
2. Score CSAT médio
3. % de Promotores, Neutros e Detratores
4. Top 3 pontos positivos mais citados
5. Top 3 problemas mais citados
6. 3 ações corretivas baseadas nos feedbacks
7. Seleção dos melhores depoimentos para usar em marketing (com sugestão de onde usar)
```

---

## Exemplo de pesquisa para WhatsApp

```
Oi [NOME]! 👋

Obrigado por confiar na [NOME_DA_EMPRESA]! 
Tenho 2 perguntinhas rápidas (30 segundos):

1️⃣ De 0 a 10, qual a chance de você nos indicar para alguém?

[cliente responde]

2️⃣ O que foi melhor na sua experiência?

[cliente responde]

Obrigado! Seu feedback vai direto para melhorarmos. 🙏
```
