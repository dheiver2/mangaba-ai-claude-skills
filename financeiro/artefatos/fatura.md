# Artefato: Fatura / Nota de Cobrança

Gera uma fatura profissional formatada pronta para enviar ao cliente por email ou WhatsApp.

## Quando usar
- Ao finalizar um serviço ou venda
- Para cobrar parcelas de contratos mensais
- Como aviso de vencimento

---

## Prompt

```
Crie uma fatura profissional com os seguintes dados:

**EMITENTE (sua empresa):**
- Razão Social: [NOME_DA_EMPRESA]
- CNPJ: [CNPJ]
- Endereço: [ENDEREÇO]
- Email: [EMAIL]
- Telefone: [TELEFONE]

**CLIENTE:**
- Nome/Razão Social: [NOME_CLIENTE]
- CPF/CNPJ: [DOCUMENTO]
- Email: [EMAIL_CLIENTE]

**SERVIÇO/PRODUTO:**
[Ex:
- Item 1: Consultoria de Marketing Digital — R$ 2.500,00
- Item 2: Gestão de Redes Sociais (maio/25) — R$ 1.800,00]

**DADOS DE PAGAMENTO:**
- Vencimento: [DATA]
- Forma de pagamento: [PIX/Boleto/Transferência]
- Chave PIX / Dados bancários: [DADOS]

**Observações:** [TEXTO ADICIONAL OU "nenhuma"]

Gere a fatura em formato profissional, com:
1. Cabeçalho com dados do emitente
2. Número da fatura (FAT-[ANO][MÊS][SEQUENCIAL])
3. Dados do cliente
4. Tabela de itens com quantidade, descrição, valor unitário e total
5. Subtotal, impostos se aplicável, e total
6. Instruções de pagamento
7. Mensagem cordial de agradecimento
```

---

## Exemplo de saída

```
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
         FATURA Nº FAT-202505-001
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

EMITENTE
Mangaba Serviços Ltda | CNPJ: 00.000.000/0001-00
Rua das Flores, 100 — São Paulo/SP
contato@mangaba.ai | (11) 99999-9999

CLIENTE
Maria Empreendimentos ME | CNPJ: 11.111.111/0001-11
Data de emissão: 17/05/2025
Vencimento: 25/05/2025

SERVIÇOS PRESTADOS
─────────────────────────────────
Consultoria de Marketing Digital    R$ 2.500,00
Gestão de Redes Sociais (mai/25)    R$ 1.800,00
─────────────────────────────────
TOTAL                               R$ 4.300,00

PAGAMENTO
Chave PIX: 00.000.000/0001-00
Banco: Nubank Empresas | Ag: 0001 | CC: 123456-7

Após o pagamento, enviar comprovante para contato@mangaba.ai

Obrigado pela confiança! Em caso de dúvidas, estamos à disposição.
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━
```
