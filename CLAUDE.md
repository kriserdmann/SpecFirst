# CLAUDE.md

Este projeto usa SpecFirst.

Este arquivo e um adaptador operacional para Claude Code. Ele nao substitui nem duplica o contrato do projeto.

## Fonte Canonica

Antes de qualquer implementacao, leia obrigatoriamente:

1. `AGENTS.md`
2. `docs/README.md`
3. `docs/project-overview.md`
4. `docs/architecture.md`
5. `docs/ai-workflow.md`
6. `docs/coding-standards.md`
7. `docs/testing.md`

Em caso de conflito:

1. siga `AGENTS.md`;
2. depois siga `docs/*`;
3. por ultimo, use este arquivo apenas como adaptador do Claude Code.

## Regra Principal

Nao implemente codigo antes de adaptar ou validar a documentacao SpecFirst do projeto.

Quando receber um escopo novo:

1. leia o contrato em `AGENTS.md`;
2. adapte os documentos relevantes em `docs/*`;
3. registre duvidas, riscos e decisoes pendentes;
4. aguarde aprovacao humana antes de iniciar a implementacao.

## Fechamento de Tarefa

Antes de considerar uma tarefa concluida:

1. atualize `docs/issues.md`;
2. atualize `docs/implementation-plan.md`;
3. registre a entrega em `docs/deployment-log.md`;
4. atualize `docs/decision-log.md` apenas quando houver decisao duradoura.

Este arquivo deve permanecer curto. Regras completas pertencem a `AGENTS.md` e `docs/*`.
