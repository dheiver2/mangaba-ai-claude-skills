# Seleção de Software / Ferramenta

Ajuda a escolher o software certo para uma necessidade específica — comparando opções, custos e fit para PME brasileira.

## Quando usar
- Antes de contratar qualquer software novo
- Quando a ferramenta atual não está dando conta
- Para comparar propostas de fornecedores de TI

---

## Prompt

```
Você é um consultor de tecnologia especializado em PMEs brasileiras.

Ajude a escolher o melhor software para [NOME_DA_EMPRESA] para a necessidade abaixo:

**Necessidade:** [Ex: "CRM para gestão de clientes", "ERP para pequena empresa", "Ferramenta de gestão de projetos", "Plataforma de e-commerce"]

**Contexto:**
- Tamanho da equipe que vai usar: [NÚMERO] pessoas
- Orçamento máximo: R$ [VALOR]/mês ou "o menor possível"
- Nível técnico da equipe: [Iniciante / Intermediário / Avançado]
- Integrações necessárias: [Ex: "precisa conectar com meu sistema de NF", "integrar com WhatsApp"]
- Dados precisam ficar no Brasil? [Sim / Não / Não sei]
- Precisa de suporte em português? [Sim / Não]

**O que a ferramenta atual faz (ou por que não tem uma):**
[DESCREVA]

**Critérios mais importantes para você (ordene):**
[Ex: 1. Preço, 2. Facilidade de uso, 3. Suporte BR, 4. Integrações, 5. Escalabilidade]

Gere:
1. Top 3 opções recomendadas (com versão gratuita/paga, preço em R$, prós e contras)
2. Comparativo em tabela por critério
3. Qual você recomendaria para este perfil e por quê
4. Red flags: o que evitar nessa categoria de software
5. Perguntas para fazer ao fornecedor antes de contratar
6. Custo total de implementação (licença + setup + treinamento)
```

---

## Exemplo de saída (CRM para PME de serviços)

| Critério | HubSpot Free | RD Station CRM | Pipedrive |
|----------|-------------|----------------|-----------|
| Preço | Grátis (básico) | R$ 0–249/mês | R$ 75/usuário/mês |
| Idioma | PT-BR ✅ | PT-BR ✅ | PT-BR ✅ |
| Suporte BR | Não no free | ✅ | Chat/email |
| Facilidade | ⭐⭐⭐⭐ | ⭐⭐⭐⭐⭐ | ⭐⭐⭐⭐ |
| Integ. WhatsApp | Plugin pago | Nativo | Plugin pago |

**Recomendação:** RD Station CRM para começar — produto nacional, suporte em PT-BR, melhor integração com o ecossistema brasileiro (NF, WhatsApp, e-mail marketing).
