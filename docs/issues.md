# Issues

## Por que este arquivo existe

Este documento registra trabalho planejado em formato executavel por humanos e agentes. Ele e util quando o projeto ainda nao tem issue tracker ou quando voce quer manter um plano local canonico.

## Formato Recomendado

```md
## ISSUE-001 - [Titulo]

**Tipo:** Feature | Chore | Bug | Docs
**Epic:** [EPIC-XX]
**Status:** Planejada | Em andamento | Concluida | Bloqueada
**Fase:** [Fase do docs/implementation-plan.md]

### Objetivo

[O que esta issue entrega?]

### Criterios de aceite

- [criterio verificavel]

### Docs relevantes

- `docs/[arquivo].md`

### Estado atual

- **AAAA-MM-DD (IA):** [nota de progresso, bloqueio ou conclusao]
```

## Regras de Atualizacao

- Toda issue em execucao deve ter status `Em andamento`.
- Toda entrega concluida deve mudar o status para `Concluida`, salvo bloqueio explicito.
- O campo `### Estado atual` deve funcionar como log vivo da issue, com entradas datadas.
- Se a entrega alterar arquitetura, fluxo, dados ou seguranca, referencie os docs atualizados.
- Se a entrega gerar rastro tecnico, registre tambem em `docs/deployment-log.md`.

## ISSUE-001 - Fundacao documental

**Tipo:** Docs
**Epic:** EPIC-01
**Status:** Concluida
**Fase:** Fase 0 - Fundacao documental

### Objetivo

Criar contrato de trabalho e documentacao canonica inicial.

### Criterios de aceite

- `AGENTS.md` descreve proposito, regras, stack e fluxo de trabalho.
- `docs/architecture.md` define camadas e dependencias.
- `docs/testing.md` define checks esperados.
- `docs/decision-log.md` contem decisoes iniciais.
- `docs/ai-workflow.md` define sincronia obrigatoria entre issue, plano e log tecnico.
- `docs/deployment-log.md` define o rastro tecnico das entregas.

### Docs relevantes

- `AGENTS.md`
- `docs/project-overview.md`
- `docs/architecture.md`
- `docs/testing.md`

### Estado atual

- **2026-05-20 (IA):** [CONCLUIDA] Fundacao documental ampliada com governanca de progresso, travamento de escopo, diferenca entre Decision Log e Deployment Log, Prompt Mestre de kickoff e rastro tecnico em `docs/deployment-log.md`.
