# Implementation Governance

## Por que este arquivo existe

Este documento define como controlar escopo durante a implementacao. Ele ajuda a evitar que uma tarefa pequena vire reescrita ampla.

## Regras de Governanca

- Implementar o menor incremento seguro.
- Registrar tradeoffs relevantes.
- Atualizar docs quando mudar contrato, arquitetura ou fluxo.
- Nao adicionar dependencia nova sem motivo claro.
- Separar bugfix, refatoracao e feature quando possivel.

## Quando Pausar e Decidir

Pausar para decisao humana quando:

- houver conflito entre docs;
- a solucao exigir mudanca arquitetural;
- houver risco de perda de dados;
- o escopo crescer alem da issue original.

## Registro

Decisoes duradouras vao para `docs/decision-log.md`.
Pendencias operacionais vao para `docs/issues.md` ou issue tracker.

