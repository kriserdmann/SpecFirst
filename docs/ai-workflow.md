# AI Workflow

## Por que este arquivo existe

Este documento define como agentes de IA devem trabalhar no projeto. Ele reduz entregas impulsivas e cria um fluxo previsivel de contexto, implementacao, validacao e documentacao.

## Principio

- Humano = navegador: define objetivo, prioridade e decisao.
- IA = piloto: explora, implementa, valida e documenta.

## Fluxo Operacional

1. **Intencao antes de implementar**
   - Definir objetivo, restricoes e criterio de pronto.
2. **Contexto minimo**
   - Ler `AGENTS.md` e docs relevantes.
3. **Contrato antes da UI ou automacao**
   - Confirmar dados, entradas, saidas e fronteiras.
4. **Teste antes do codigo**
   - Criar teste quando houver comportamento novo ou contrato importante.
5. **Pequenas entregas**
   - Implementar incrementos curtos, revisaveis e reversiveis.
6. **Validacao**
   - Rodar checks aplicaveis.
7. **Documentacao viva**
   - Atualizar docs quando arquitetura, modelo ou fluxo mudar.

## Kickoff de Tarefa

Antes de implementar, a IA deve registrar:

- objetivo;
- docs lidos;
- criterio de aceite;
- impacto em dados, seguranca, UI e testes;
- riscos ou suposicoes.

## Fechamento de Tarefa

Ao concluir, a IA deve relatar:

- arquivos alterados;
- comportamento entregue;
- testes ou checks executados;
- pendencias ou riscos residuais;
- docs atualizados.

