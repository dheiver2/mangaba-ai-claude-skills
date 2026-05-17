# Artefato: Plano de Backup e Segurança de Dados

Gera um plano prático de backup e segurança para PMEs — sem precisar de equipe de TI dedicada.

## Quando usar
- Nunca teve um plano de backup formal
- Após perda de dados (para não repetir)
- Exigência de cliente ou auditoria de segurança
- Adequação à LGPD (Art. 46 — medidas de segurança)

---

## Prompt

```
Você é um especialista em segurança e backup para PMEs brasileiras.

Crie um Plano de Backup e Segurança de Dados para [NOME_DA_EMPRESA]:

**Dados críticos que precisam de backup:**
[Ex:
- Base de clientes (planilha Google)
- Documentos financeiros (Google Drive)
- Projetos e arquivos de clientes (pasta local no servidor)
- Banco de dados do site (WordPress)
- Emails importantes]

**Infraestrutura atual:**
- Servidor próprio? [Sim / Não — dados só em nuvem]
- Computadores com dados locais? [NÚMERO]
- Ferramentas SaaS (dados na nuvem do fornecedor): [LISTE]

**Último backup feito:** [DATA ou "nunca fiz"]
**Já perdeu dados alguma vez?** [Sim / Não]

Crie o plano com:

**POLÍTICA DE BACKUP:**
- O que fazer backup (classificação: crítico / importante / descartável)
- Frequência por tipo de dado (diário / semanal / mensal)
- Destinos de backup (regra 3-2-1: 3 cópias, 2 mídias, 1 fora do local)
- Retenção (por quanto tempo guardar)
- Quem é responsável por cada backup

**PROCEDIMENTO DE TESTE:**
- Como verificar se o backup funcionou (teste mensal)
- Simulação de restauração (semestral)

**SEGURANÇA DOS BACKUPS:**
- Criptografia recomendada
- Controle de acesso aos backups

**FERRAMENTAS RECOMENDADAS (por orçamento):**
- Opção zero custo
- Opção até R$ 50/mês
- Opção até R$ 200/mês

**EM CASO DE PERDA DE DADOS:**
- Passo a passo de recuperação
- Contatos de suporte técnico
- Quando acionar ANPD (obrigatório se dados pessoais de clientes forem afetados)
```
