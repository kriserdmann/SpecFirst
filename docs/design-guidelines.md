# Design Guidelines

## Por que este arquivo existe

Este documento define a direcao visual e interativa do projeto antes que telas, componentes e estilos sejam implementados.

Ele evita que a IA invente uma linguagem visual nova a cada tarefa. Use este arquivo para registrar identidade, tokens, componentes, padroes de layout, acessibilidade e exemplos de uso.

Quando o projeto tiver UI, site, app, dashboard, landing page, design system, marca ou experiencia visual, este documento deve ser preenchido antes da implementacao relevante.

## Como Usar

1. Descreva a intencao visual do projeto em linguagem clara.
2. Defina tokens de cor, tipografia, espacamento, raios, sombras e grids.
3. Registre os componentes esperados e suas variacoes.
4. Explique o que a IA deve e nao deve fazer ao criar UI.
5. Atualize este documento quando uma decisao visual virar padrao recorrente.

## Overview

Descreva a direcao de design em 2 a 5 paragrafos.

Inclua:

- tipo de produto ou superficie visual;
- sensacao desejada;
- nivel de densidade da interface;
- relacao entre marca, conteudo e conversao;
- principais padroes visuais;
- restricoes importantes.

Exemplo de preenchimento:

```md
O projeto e um [tipo de produto] para [publico]. A interface deve transmitir [atributos], priorizando [clareza, velocidade, confianca, sofisticacao, densidade, etc.].

A experiencia visual deve evitar [padroes proibidos] e favorecer [padroes desejados]. A marca se expressa principalmente por [cor, tipografia, composicao, fotografia, ilustracao, movimento, etc.].
```

## Principios de Design

- **Clareza:** [como a interface evita ambiguidade]
- **Consistencia:** [quais padroes devem se repetir]
- **Hierarquia:** [como usuarios entendem prioridade]
- **Acessibilidade:** [contraste, foco, teclado, leitura, tamanhos]
- **Responsividade:** [como layouts mudam por viewport]
- **Performance visual:** [o que evitar para nao pesar a experiencia]

## Tokens

### Cores

Defina roles, nao apenas hexadecimais soltos.

| Token | Valor | Uso |
| --- | --- | --- |
| `{colors.primary}` | `[#HEX]` | [acao principal, marca, destaque] |
| `{colors.canvas}` | `[#HEX]` | [fundo principal] |
| `{colors.surface}` | `[#HEX]` | [cards, paineis, regioes] |
| `{colors.text}` | `[#HEX]` | [texto principal] |
| `{colors.text-muted}` | `[#HEX]` | [texto secundario] |
| `{colors.border}` | `[#HEX]` | [divisorias, contornos] |
| `{colors.success}` | `[#HEX]` | [feedback positivo] |
| `{colors.warning}` | `[#HEX]` | [alertas] |
| `{colors.danger}` | `[#HEX]` | [erros e acoes destrutivas] |

Regras:

- `[quando usar a cor primaria]`
- `[quando nao criar novas cores]`
- `[como tratar estados de erro, sucesso e aviso]`

### Tipografia

| Token | Familia | Tamanho | Peso | Line Height | Uso |
| --- | --- | --- | --- | --- | --- |
| `{typography.display}` | `[fonte]` | `[px]` | `[peso]` | `[px]` | [hero, titulo principal] |
| `{typography.heading}` | `[fonte]` | `[px]` | `[peso]` | `[px]` | [secoes] |
| `{typography.body}` | `[fonte]` | `[px]` | `[peso]` | `[px]` | [texto padrao] |
| `{typography.body-strong}` | `[fonte]` | `[px]` | `[peso]` | `[px]` | [enfase, botoes] |
| `{typography.caption}` | `[fonte]` | `[px]` | `[peso]` | `[px]` | [metadados, ajuda] |

Regras:

- `[sentence-case, title-case, uppercase, etc.]`
- `[quando usar peso forte]`
- `[se letter-spacing e permitido ou proibido]`
- `[substitutos de fonte, se houver]`

### Espacamento

| Token | Valor | Uso |
| --- | --- | --- |
| `{spacing.xs}` | `[px]` | [micro espacamento] |
| `{spacing.sm}` | `[px]` | [gaps pequenos] |
| `{spacing.md}` | `[px]` | [padding padrao] |
| `{spacing.lg}` | `[px]` | [cards, secoes compactas] |
| `{spacing.xl}` | `[px]` | [secoes, grids] |
| `{spacing.2xl}` | `[px]` | [bandas grandes] |

Regras:

- `[unidade base, ex: 4px ou 8px]`
- `[padding de secoes]`
- `[gaps entre componentes]`

### Raios, Bordas e Sombras

| Token | Valor | Uso |
| --- | --- | --- |
| `{rounded.sm}` | `[px]` | [inputs pequenos] |
| `{rounded.md}` | `[px]` | [cards menores] |
| `{rounded.lg}` | `[px]` | [cards padrao] |
| `{rounded.pill}` | `999px` | [chips, botoes pill, se aplicavel] |
| `{shadow.sm}` | `[valor]` | [elevacao sutil] |
| `{shadow.md}` | `[valor]` | [modais, cards elevados] |

Regras:

- `[quais elementos podem ter sombra]`
- `[quais elementos devem ser planos]`
- `[qual shape assina a marca]`

## Layout

### Grid e Container

- **Container maximo:** `[px]`
- **Gutters desktop:** `[px]`
- **Gutters mobile:** `[px]`
- **Padroes de coluna:** `[1-col, 2-col, sidebar, dashboard, etc.]`

### Breakpoints

| Nome | Largura | Mudancas principais |
| --- | --- | --- |
| Mobile | `[px]` | `[mudancas]` |
| Tablet | `[px]` | `[mudancas]` |
| Desktop | `[px]` | `[mudancas]` |

### Responsividade

- `[como cards empilham]`
- `[como navegacao muda]`
- `[como tabelas ou dashboards respondem]`
- `[como imagens e midias se comportam]`

## Componentes

Descreva os componentes esperados, seus estados e variacoes.

### Buttons

**`button-primary`**

- Uso: `[acao principal]`
- Visual: `[cor, tipografia, raio, padding]`
- Estados: `[hover, focus, disabled, loading]`

**`button-secondary`**

- Uso: `[acao secundaria]`
- Visual: `[cor, tipografia, raio, padding]`
- Estados: `[hover, focus, disabled, loading]`

### Cards

**`card-default`**

- Uso: `[conteudo agrupado]`
- Visual: `[fundo, borda, sombra, raio, padding]`

### Inputs

**`text-input`**

- Uso: `[entrada textual]`
- Visual: `[fundo, borda, raio, tipografia]`
- Estados: `[focus, error, disabled]`

### Navigation

**`nav-bar`**

- Uso: `[navegacao principal]`
- Visual: `[altura, alinhamento, estados]`
- Responsivo: `[desktop/mobile]`

Adicione secoes para componentes especificos do projeto, como tabelas, modais, sidebars, command palettes, mapas, players, editores ou formularios complexos.

## Conteudo Visual

Defina regras para imagens, ilustracoes, icones, videos e graficos.

- **Fotografia:** `[estilo, proporcao, tratamento, proibicoes]`
- **Ilustracao:** `[quando usar, estilo, cores, proporcao]`
- **Icones:** `[biblioteca, peso visual, tamanho, uso]`
- **Graficos:** `[paleta, labels, densidade, acessibilidade]`
- **Midia responsiva:** `[aspect-ratio, crop, fallback]`

## Interacao e Estados

- **Hover:** `[como feedback aparece]`
- **Focus:** `[como foco de teclado aparece]`
- **Pressed/Active:** `[como estado ativo aparece]`
- **Loading:** `[skeleton, spinner, disabled state]`
- **Empty states:** `[texto, acao, visual]`
- **Errors:** `[tom, cor, local de exibicao]`
- **Success:** `[feedback, duracao, persistencia]`

## Acessibilidade

- Contraste minimo: `[regra]`
- Tamanho minimo de toque: `[px]`
- Navegacao por teclado: `[regra]`
- Labels e aria: `[regra]`
- Movimento reduzido: `[regra]`
- Conteudo nao deve depender apenas de cor.

## Do's and Don'ts

### Do

- `[padrao desejado]`
- `[padrao desejado]`
- `[padrao desejado]`

### Don't

- `[padrao proibido]`
- `[padrao proibido]`
- `[padrao proibido]`

## Diretrizes para IA

Ao implementar UI, a IA deve:

1. ler este documento antes de criar componentes, paginas ou estilos;
2. reutilizar tokens, componentes e padroes existentes;
3. nao introduzir nova paleta, fonte, grid ou linguagem visual sem justificativa;
4. registrar decisao em `docs/decision-log.md` quando mudar o sistema visual;
5. atualizar este documento quando um padrao visual virar contrato do projeto;
6. validar responsividade, acessibilidade e estados interativos antes de concluir.

Se este documento ainda estiver incompleto, a IA deve propor o preenchimento antes de implementar UI relevante.
