# Revisão de Contrato

Analisa um contrato sob a perspectiva da PME contratante ou contratada — identifica cláusulas abusivas, lacunas e riscos.

## Quando usar
- Antes de assinar qualquer contrato com fornecedor, cliente ou parceiro
- Ao renovar contrato existente
- Quando sentir que algo no contrato "não está certo"

---

## Prompt

```
Você é um advogado empresarial especializado em PMEs brasileiras.

Analise o contrato abaixo sob a perspectiva de [CONTRATANTE / CONTRATADA], empresa [NOME_DA_EMPRESA]:

[COLE O TEXTO DO CONTRATO AQUI]

Faça uma análise completa com:

1. **Resumo executivo** (5 linhas): do que se trata, partes, objeto, valor e prazo
2. **Cláusulas favoráveis** à minha empresa (pontos positivos)
3. **Cláusulas de risco** — para cada uma:
   - Transcreva a cláusula
   - Explique o risco em linguagem simples
   - Sugira como renegociar ou alterar
4. **Lacunas perigosas**: o que o contrato NÃO diz mas deveria
5. **Multas e penalidades**: liste todas, com valores e gatilhos
6. **Cláusula de rescisão**: como sair do contrato e a que custo
7. **Score de risco geral**: Baixo / Médio / Alto — com justificativa
8. **Recomendação final**: assinar como está / negociar X pontos / não assinar

Linguagem: clara, sem juridiquês. Foque no que impacta o negócio.

⚠️ Lembre ao final que esta análise é orientativa e não substitui consulta com advogado.
```

---

## Exemplo de saída (trecho)

**Score de risco: 🟡 MÉDIO**

**Cláusula de risco identificada — Art. 8º:**
> *"O contratado se responsabiliza por quaisquer danos diretos e indiretos..."*

**Risco:** Responsabilidade ilimitada por danos indiretos pode expor sua empresa a valores muito superiores ao contrato. Em caso de processo, o cliente pode cobrar lucros cessantes, danos morais e outros prejuízos sem teto definido.

**Como negociar:** Inclua limitação de responsabilidade: *"A responsabilidade total da contratada fica limitada ao valor total do contrato"*.

**Lacuna identificada:** O contrato não define SLA (prazo de atendimento). Se houver atraso, não há critério objetivo para penalidade ou rescisão justificada.
