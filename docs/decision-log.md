# Decision Log

## Por que este arquivo existe

Este documento registra decisoes que mudam arquitetura, modelo, fluxo, escopo ou operacao. Ele evita que o motivo de uma escolha desapareca com o tempo.

## Como Usar

- Identificador incremental: `0001`, `0002`, `0003`.
- Estado: `Proposta`, `Aceita`, `Substituida` ou `Rejeitada`.
- Cada decisao deve listar contexto, decisao e consequencias.
- Decisoes substituidas devem apontar para a decisao nova.

## Template de Decisao

```md
## 0001 - [Titulo curto]

- **Data:** AAAA-MM-DD
- **Estado:** Proposta

### Contexto

[Qual problema, conflito ou oportunidade motivou a decisao?]

### Decisao

[O que foi decidido?]

### Consequencias

- [Impacto positivo]
- [Tradeoff]
- [O que precisa mudar agora]
```

## 0001 - Adotar AGENTS.md como contrato universal

- **Data:** 2026-05-19
- **Estado:** Aceita

### Contexto

O projeto pode ser trabalhado por pessoas, agentes e ferramentas diferentes. Sem uma fonte comum, regras e arquitetura podem divergir.

### Decisao

Adotar `AGENTS.md` como contrato universal e `docs/*` como fonte canonica tecnica e de produto.

### Consequencias

- Menos dependencia de uma ferramenta especifica.
- Maior consistencia entre entregas.
- Necessidade de manter documentacao viva.
