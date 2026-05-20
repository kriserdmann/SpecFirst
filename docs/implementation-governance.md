# Implementation Governance

## Por que este arquivo existe

Este documento define como controlar escopo durante a implementacao. Ele ajuda a evitar que uma tarefa pequena vire reescrita ampla.

## Regras de Governanca

- Implementar o menor incremento seguro.
- Registrar tradeoffs relevantes.
- Atualizar docs quando mudar contrato, arquitetura ou fluxo.
- Nao adicionar dependencia nova sem motivo claro.
- Separar bugfix, refatoracao e feature quando possivel.
- Manter `docs/issues.md`, `docs/implementation-plan.md` e `docs/deployment-log.md` sincronizados.

## Travamento de Escopo

A IA nao tem autorizacao para:

- criar nova issue quando a tarefa atual ainda puder ser resolvida dentro da issue existente;
- pular para a proxima fase se a fase atual tiver checklists obrigatorios abertos;
- expandir o escopo para uma feature nao planejada;
- transformar uma correcao pequena em refatoracao ampla sem aprovacao humana.

Se a IA identificar que precisa mudar o rumo, deve pausar e pedir decisao humana antes de implementar.

## Avanco de Fase

Uma fase so pode ser marcada como concluida quando:

- os itens do checklist da fase foram concluidos ou explicitamente descartados;
- os checks definidos em `docs/testing.md` foram executados ou tiveram impossibilidade registrada;
- issues relacionadas foram atualizadas em `docs/issues.md`;
- a entrega foi registrada em `docs/deployment-log.md`.

## Quando Pausar e Decidir

Pausar para decisao humana quando:

- houver conflito entre docs;
- a solucao exigir mudanca arquitetural;
- houver risco de perda de dados;
- o escopo crescer alem da issue original.

## Registro

Decisoes duradouras vao para `docs/decision-log.md`.
Entregas tecnicas vao para `docs/deployment-log.md`.
Pendencias operacionais vao para `docs/issues.md` ou issue tracker.
