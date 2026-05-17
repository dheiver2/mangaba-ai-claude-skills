# Artefato: Mapa do Stack Tecnológico

Gera um documento completo com todas as ferramentas que a empresa usa — útil para onboarding, auditoria e planejamento de TI.

## Quando usar
- Documentar o stack para um novo colaborador
- Passar para novo gestor ou sócio
- Base para planejamento de migração ou upgrade

---

## Prompt

```
Você é o CTO virtual da empresa [NOME_DA_EMPRESA].

Crie um Mapa do Stack Tecnológico completo com base nas informações abaixo:

**FERRAMENTAS QUE USAM (liste tudo que você lembrar):**
[Ex:
- Comunicação interna: WhatsApp grupos, Slack
- Email: Google Workspace
- Documentos: Google Drive, Notion
- Financeiro: Conta Azul, planilha Google
- CRM: RD Station
- Marketing: Canva, Instagram, Mailchimp
- Atendimento: WhatsApp Business
- Emissão de NF: NF-e.io
- Pagamentos: Asaas
- Videoconferência: Google Meet
- Gestão de tarefas: Trello]

Para cada ferramenta, gere uma tabela com:
| Ferramenta | Categoria | Plano | Custo/mês | Usuários | Responsável | Alternativa se parar |
|------------|-----------|-------|-----------|----------|-------------|---------------------|

Também gere:
1. Mapa visual textual (diagrama de fluxo de dados entre ferramentas)
2. Integrações ativas entre as ferramentas
3. Single points of failure (se uma ferramenta cair, o que para?)
4. Gaps: necessidades sem ferramenta dedicada
5. Sobreposições: funções duplicadas entre ferramentas
6. Score de maturidade tecnológica: Básico / Intermediário / Avançado
7. Roadmap sugerido para os próximos 6 meses
```
