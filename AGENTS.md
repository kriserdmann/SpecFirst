# AGENTS.md

## Por que este arquivo existe

Este arquivo e o contrato universal do projeto para pessoas, agentes de IA e ferramentas automatizadas. Ele deve ser lido antes de qualquer implementacao relevante.

Ele nao substitui a documentacao completa. Ele resume as regras obrigatorias, a arquitetura esperada e o caminho para encontrar contexto nos documentos certos.

## Proposito do Projeto

- **Nome:** `SpecFirst`
- **Tipo:** framework de documentacao em Markdown para projetos.
- **Problema resolvido:** projetos iniciam sem contrato claro de contexto, arquitetura, validacao e fluxo de trabalho para humanos e agentes de IA.
- **Publico-alvo:** pessoas desenvolvedoras, product builders, equipes pequenas, agentes de IA e ferramentas automatizadas que precisam operar sobre um projeto com regras claras.
- **Resultado esperado:** qualquer novo projeto pode copiar `AGENTS.md` e `docs` para nascer com documentacao minima, criterio de pronto e trilha de contexto.

## Regras Inviolaveis

Liste regras que nenhum agente ou desenvolvedor deve quebrar sem registrar uma decisao.

Exemplos:

1. Nunca criar codigo fora da arquitetura definida em `docs/architecture.md`.
2. Todo comportamento novo relevante deve ter teste.
3. Nenhum commit pode quebrar lint, testes ou typecheck.
4. Entradas externas devem ser validadas na fronteira apropriada.
5. Decisoes arquiteturais devem ser registradas em `docs/decision-log.md`.

Regras do SpecFirst:

1. A raiz do repositorio e o template replicavel.
2. Os arquivos devem permanecer genericos o bastante para serem copiados para novos projetos.
3. Toda nova rota de documentacao deve ser refletida em `README.md`, `AGENTS.md` e `docs/README.md`.

## Stack do Projeto

Explique as tecnologias principais e suas versoes quando isso afetar decisoes.

- Linguagem: Markdown.
- Framework: estrutura documental propria baseada em `AGENTS.md + docs`.
- Banco: nao aplicavel.
- UI: nao aplicavel.
- Testes: revisao estrutural dos links, rotas e consistencia dos documentos.
- Deploy: distribuicao por copia de `AGENTS.md` e `docs` ou publicacao do repositorio.

## Estrutura de Pastas Esperada

- `/README.md` -> guia de uso do SpecFirst.
- `/AGENTS.md` -> contrato universal copiavel para novos projetos.
- `/docs` -> documentacao canonica copiavel.

## Fluxo de Trabalho Esperado

Todo trabalho relevante deve seguir este ciclo:

1. Entender objetivo, contexto operacional e criterio de pronto.
2. Ler `AGENTS.md` e docs relevantes.
3. Escrever ou ajustar testes quando houver comportamento novo.
4. Implementar o menor incremento seguro.
5. Refatorar quando houver duplicacao real ou complexidade desnecessaria.
6. Validar com os checks definidos em `docs/testing.md`.
7. Atualizar docs quando arquitetura, modelo ou fluxo mudar.

## Definition of Done

Uma tarefa so esta pronta quando:

- o comportamento solicitado foi implementado;
- testes relevantes foram criados ou atualizados;
- tipagem, lint e checks aplicaveis foram executados;
- entradas externas estao validadas;
- nao ha duplicacao evidente;
- a arquitetura foi respeitada;
- documentacao foi atualizada quando necessario;
- impossibilidades ou riscos residuais foram registrados.

## Referencias de Documentacao

### Nucleo minimo

Ler sempre antes de implementacoes relevantes:

- `docs/project-overview.md`
- `docs/README.md`
- `docs/architecture.md`
- `docs/ai-workflow.md`
- `docs/coding-standards.md`
- `docs/testing.md`

### Ler sob demanda

| Documento | Quando consultar |
| --- | --- |
| `docs/domains.md` | Ao alterar fronteiras de responsabilidade. |
| `docs/data-model.md` | Ao alterar dados, schemas, entidades ou persistencia. |
| `docs/security.md` | Ao tocar auth, permissoes, uploads, secrets ou dados sensiveis. |
| `docs/workflows.md` | Ao alterar jornada operacional ou fluxo de usuario. |
| `docs/operations.md` | Ao mexer em ambiente, deploy, backups ou operacao. |
| `docs/templates.md` | Ao criar padroes reutilizaveis de UI, codigo ou documento. |
| `docs/decision-log.md` | Quando houver decisao arquitetural nova ou conflito entre regras. |
| `docs/implementation-plan.md` | Ao planejar fases, sprints ou sequencia de entrega. |
| `docs/issues.md` | Ao executar trabalho planejado por issue. |

## Hierarquia de Contexto

1. `AGENTS.md` e o contrato universal.
2. `docs/*` e a fonte canonica tecnica e de produto.
3. Arquivos de ferramenta, como `CLAUDE.md`, `.cursorrules` ou similares, sao adaptadores operacionais.
4. Em caso de conflito, seguir `AGENTS.md`, docs canonicos e `docs/decision-log.md`.

## Diretrizes de Uso de IA

A IA atua como piloto de implementacao.
O humano atua como navegador de decisao.

Nunca:

- implementar sem entender o objetivo;
- criar arquitetura complexa sem necessidade comprovada;
- esconder tradeoffs ou riscos;
- deixar regras importantes apenas na memoria da ferramenta.

Sempre:

- simplificar solucoes;
- manter entregas pequenas;
- preferir contratos claros;
- validar antes de concluir;
- atualizar docs quando a decisao mudar.
