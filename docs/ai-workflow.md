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
7. **Sincronia de progresso**
   - Atualizar issue, plano e log tecnico antes de considerar a tarefa pronta.
8. **Documentacao viva**
   - Atualizar docs quando arquitetura, modelo ou fluxo mudar.

## Kickoff de Tarefa

Antes de implementar, a IA deve registrar:

- objetivo;
- issue ou fase relacionada;
- docs lidos;
- criterio de aceite;
- impacto em dados, seguranca, UI e testes;
- riscos ou suposicoes.

## Fechamento de Tarefa

Antes de encerrar a tarefa, commitar ou responder como concluida, a IA deve persistir o progresso no repositorio:

1. Atualizar `docs/issues.md`.
   - Mudar o status da issue quando aplicavel: `Planejada`, `Em andamento`, `Concluida` ou `Bloqueada`.
   - Registrar uma nota datada em `### Estado atual`.
2. Atualizar `docs/implementation-plan.md`.
   - Marcar checklists concluidos.
   - Atualizar a fase atual quando a entrega destravar a proxima etapa.
   - Nao pular fases com pendencias abertas sem decisao humana.
3. Atualizar `docs/deployment-log.md`.
   - Registrar o que foi feito, arquivos modificados, checks executados e riscos tecnicos.
4. Atualizar `docs/decision-log.md` apenas quando houver decisao de arquitetura, produto, modelo, seguranca ou operacao.

Depois de persistir o progresso, a IA deve relatar no chat:

- arquivos alterados;
- comportamento entregue;
- testes ou checks executados;
- status atualizado da issue;
- fase ou checklist atualizado no plano;
- entrada criada no log tecnico;
- pendencias ou riscos residuais;
- docs atualizados.

## Diferenca entre Logs

- `docs/decision-log.md` registra decisoes duradouras e seus motivos.
- `docs/deployment-log.md` registra entregas tecnicas realizadas.
- `docs/issues.md` registra o estado vivo de cada trabalho planejado.

Nao misture decisao arquitetural com historico operacional. Se uma entrega tecnica tambem gerar uma decisao duradoura, registre nos dois lugares com propositos diferentes.
