# Auditoria Mensal de Ferramentas e Acessos

Revisa todas as assinaturas de software, acessos ativos e identifica desperdícios ou riscos de segurança.

## Frequência
**Mensal** — sugerido no 1º dia útil do mês às 10h

## Como agendar com Claude Code

```bash
claude schedule create \
  --name "auditoria-ferramentas" \
  --cron "0 10 1 * *" \
  --prompt-file tecnologia/scheduled/auditoria-ferramentas.md
```

---

## Prompt

```
Você é o gerente de TI da empresa [NOME_DA_EMPRESA].

Faça a Auditoria Mensal de Ferramentas e Acessos de [MÊS/ANO]:

**ASSINATURAS ATIVAS:**
[Liste: ferramenta | plano | valor mensal | quantos usuários | quem usa]

**ACESSOS:**
[Liste colaboradores que saíram no mês e verificar se acessos foram revogados]
[Colaboradores com acesso a sistemas que não usam mais o cargo justificaria]

**USO REAL (se souber):**
[Ex: "Notion — 10 licenças, mas só 4 pessoas abriram no mês"]

**NOVOS SOFTWARES CONTRATADOS NO MÊS:**
[Liste ou "nenhum"]

Gere:
1. Total gasto em software/mês e custo por colaborador
2. Ferramentas com baixo uso (candidatas ao corte)
3. Funcionalidades sobrepostas (2 ferramentas que fazem a mesma coisa)
4. Acessos de ex-colaboradores ainda ativos 🔴
5. Licenças sobrando (pago por X, usando Y < X)
6. Economia possível com cancelamentos e downgrades
7. Riscos de segurança identificados
8. Ações recomendadas para o mês
```
