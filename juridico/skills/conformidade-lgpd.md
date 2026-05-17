# Diagnóstico de Conformidade LGPD

Avalia o nível de conformidade da empresa com a Lei Geral de Proteção de Dados (Lei 13.709/2018) e gera um plano de adequação.

## Quando usar
- Verificar se sua empresa está em conformidade com a LGPD
- Antes de fechar contrato com cliente grande (muitos exigem DPO ou declaração LGPD)
- Após um incidente de vazamento de dados
- Revisão anual de conformidade

---

## Prompt

```
Você é um especialista em LGPD (Lei 13.709/2018) para PMEs brasileiras.

Faça um diagnóstico de conformidade LGPD para a empresa [NOME_DA_EMPRESA], segmento [SEGMENTO]:

**Dados que a empresa coleta e trata:**
[Ex: nome, CPF, email, telefone, endereço, dados de pagamento, localização, dados de saúde]

**Como coleta:**
[Ex: formulário no site, WhatsApp, cadastro presencial, cookies]

**Onde armazena:**
[Ex: planilha Excel local, Google Sheets, CRM HubSpot, banco de dados próprio, e-mails]

**Com quem compartilha:**
[Ex: contador, plataforma de pagamento, empresa de marketing, não compartilha]

**Tem DPO (Encarregado de Proteção de Dados)?** [Sim / Não / Não sei o que é]
**Tem Política de Privacidade publicada?** [Sim / Não]
**Tem formulário de consentimento?** [Sim / Não]
**Já teve incidente de vazamento?** [Sim / Não]

Gere:
1. Score de conformidade atual (0-100) com classificação: Iniciante / Em desenvolvimento / Adequado / Exemplar
2. Os 5 maiores riscos de penalidade (ANPD pode multar até R$ 50 milhões)
3. Checklist de adequação com prioridade (Alta/Média/Baixa) e prazo sugerido
4. Documentos obrigatórios que a empresa precisa ter
5. O que fazer nos primeiros 30 dias (quick wins)
6. Custo estimado de adequação (sem contratar escritório)
```

---

## Exemplo de saída (trecho)

**Score de conformidade: 28/100 — Iniciante** 🔴

**Top 3 riscos imediatos:**
1. **Site sem Política de Privacidade** — infração direta ao Art. 9º. Risco de notificação da ANPD.
2. **Dados de clientes em planilha Excel sem senha** — violação do princípio de segurança (Art. 46). Em caso de vazamento, multa + danos morais.
3. **Sem consentimento explícito para marketing** — enviar email marketing sem opt-in viola Art. 7º, inciso I.

**Quick wins (30 dias, custo próximo de zero):**
- ✅ Publicar Política de Privacidade (use o artefato `politica-privacidade-lgpd.md`)
- ✅ Proteger planilhas com senha e habilitar 2FA no Google
- ✅ Adicionar caixa de consentimento no formulário do site
