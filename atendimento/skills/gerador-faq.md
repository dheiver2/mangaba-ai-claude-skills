# Gerador de FAQ

Cria uma seção completa de Perguntas Frequentes para site, WhatsApp automático ou material de vendas.

## Quando usar
- Montar FAQ do site
- Configurar respostas automáticas do WhatsApp Business
- Preparar material para equipe de vendas responder dúvidas

---

## Prompt

```
Você é um especialista em experiência do cliente para PMEs brasileiras.

Crie um FAQ completo para a empresa [NOME_DA_EMPRESA], que oferece [DESCREVA O PRODUTO/SERVIÇO].

**Contexto:**
- Principais dúvidas que os clientes costumam ter: [LISTE O QUE VOCÊ JÁ SABE, ex: "preço, prazo de entrega, formas de pagamento, cancelamento"]
- Canal onde o FAQ será usado: [Site / WhatsApp Business / Material impresso / Chatbot]
- Tom: [Formal / Informal / Técnico]

**Informações para responder corretamente:**
- Preços: [DESCREVA ou "variam conforme plano"]
- Formas de pagamento: [PIX, cartão, boleto, etc.]
- Prazo de entrega/início: [DESCREVA]
- Política de cancelamento: [DESCREVA]
- Garantia: [DESCREVA]
- Horário de atendimento: [DESCREVA]
- Contato de suporte: [EMAIL/TELEFONE/WHATSAPP]

Gere:
1. 15 perguntas e respostas organizadas por categoria
2. Categorias sugeridas: Sobre o produto, Pagamento, Entrega/Prazo, Cancelamento, Suporte
3. Para WhatsApp: versão curta de cada resposta (até 200 caracteres)
4. Para site: versão completa com links e CTAs quando relevante
5. 3 perguntas que os clientes ainda não fazem mas deveriam (FAQ proativo)
```

---

## Exemplo de saída (trecho)

**CATEGORIA: PAGAMENTO**

**P: Quais formas de pagamento vocês aceitam?**
R: Aceitamos PIX (com 5% de desconto), cartão de crédito em até 12x (sem juros nos planos anuais) e boleto bancário com vencimento em 3 dias úteis. Não aceitamos transferência bancária para pessoa física.

*Versão WhatsApp:* "Aceitamos PIX (5% OFF), cartão até 12x e boleto. Para mais detalhes: [LINK]"

---

**CATEGORIA: CANCELAMENTO**

**P: Posso cancelar a qualquer momento?**
R: Sim. Planos mensais podem ser cancelados com 30 dias de antecedência, sem multa. Planos anuais podem ser cancelados com reembolso proporcional nos primeiros 30 dias. Após esse período, o valor pago não é reembolsado, mas o acesso permanece até o fim do período contratado.

*Versão WhatsApp:* "Sim! Mensais: cancela com 30 dias de aviso. Anuais: reembolso proporcional em 30 dias."

---

**FAQ PROATIVO (o que deveriam perguntar):**
1. "Vocês têm suporte em português?" — Sim, 100% em PT-BR, sem scripts robóticos.
2. "Tenho dados sensíveis — como vocês protegem?" — Aborda LGPD e segurança dos dados.
3. "Posso usar em mais de um dispositivo?" — Esclarece limitações de uso da licença.
