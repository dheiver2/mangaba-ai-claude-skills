# Gerador de Checklist de Qualidade

Cria checklists operacionais para garantir padronização, reduzir erros e manter a qualidade das entregas.

## Quando usar
- Padronizar entregas para clientes
- Antes de lançar produto ou serviço novo
- Treinamento de equipe nova
- Auditoria interna de qualidade

---

## Prompt

```
Você é um especialista em gestão da qualidade para PMEs brasileiras.

Crie um checklist de qualidade para [NOME_DA_EMPRESA]:

**Processo ou entrega a ser controlada:** [Ex: "Entrega de projeto de design", "Atendimento ao cliente por WhatsApp", "Preparo de pedido para envio", "Publicação de post nas redes sociais"]

**Quem executa:** [CARGO]
**Quando executa o checklist:** [Ex: "antes de enviar ao cliente", "ao final de cada turno", "antes de publicar"]

**Padrões mínimos de qualidade que devem ser verificados:**
[Liste o que é inaceitável chegar ao cliente/mercado, ex: "produto com defeito visual", "texto com erro ortográfico", "prazo não cumprido"]

**Já existe algum processo de verificação?** [Sim/Não — descreva se sim]

Gere:
1. Checklist principal com itens organizados por categoria
2. Para cada item: critério objetivo de aprovação/reprovação
3. Campo de assinatura/responsável
4. Coluna de status: ✅ OK / ❌ Reprovado / ⚠️ Atenção
5. Seção "Ação corretiva" para itens reprovados
6. Versão simplificada (apenas os 10 itens mais críticos — para uso rápido)
7. Versão para imprimir (tabela formatada)
```

---

## Exemplo de saída (trecho)

**Checklist — Publicação de Post (Redes Sociais)**

| # | Item | Critério | Status |
|---|------|----------|--------|
| 1 | Texto sem erros | Lido 2x + verificado no Word | ✅ / ❌ |
| 2 | Imagem na resolução correta | Instagram: 1080x1080px | ✅ / ❌ |
| 3 | Hashtags revisadas | Máx 5, sem # banned | ✅ / ❌ |
| 4 | Link na bio atualizado | Aponta para página correta | ✅ / ❌ |
| 5 | Horário de publicação | Agendado para horário de pico | ✅ / ❌ |
| 6 | CTA claro | Tem 1 chamada para ação | ✅ / ❌ |

**Responsável:** _____________ **Data:** _____________
