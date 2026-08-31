---
version: alpha
name: Bullet Identity Source
description: >-
  Forma compilada do 00 Tokens And Manifest (versao-tokens v1.15) do
  Bulletpedia. O Bulletpedia é a única fonte (P12): este arquivo é gerado,
  nunca editado à mão. Divergência se corrige no Manifest e recompila.
colors:
  # ── papéis da convenção DESIGN.md, mapeados aos conceitos Bullet
  # primary = tinta principal (títulos e leitura) · tertiary = o único driver de
  # interação (acento funcional, cota 10%) · neutral = o chão de tudo (dark, P13)
  primary: "{colors.paper-100}"
  secondary: "{colors.grey-350}"
  tertiary: "{colors.lime-500}"
  neutral: "{colors.ink-990}"
  # ── Camada 0 · rampa de superfície (base do sistema, 4 degraus + 5º restrito)
  ink-990: "#070707"
  ink-980: "#0C0C0C"
  ink-960: "#131313"
  ink-940: "#1A1A1A"
  ink-920: "#242424"
  # ── rampa de arte (superfície única de peça de marca)
  ink-900: "#161616"
  ink-870: "#1D1D1D"
  ink-850: "#202020"
  ink-800: "#292928"
  ink-750: "#333333"
  ink-700: "#3A3A3A"
  # ── neutros de texto e contorno
  white-pure: "#FFFFFF"
  paper-100: "#F8F3E9"
  grey-350: "#A3A3A3"
  grey-400: "#8A8A8A"
  grey-450: "#7C7C7C"
  grey-500: "#6E6E6E"
  # ── escala quente (só lane Email)
  paper-200: "#C9C4BA"
  paper-300: "#A8A39A"
  paper-400: "#8A857C"
  # ── acento e cor funcional
  lime-500: "#C2F141"
  amber-500: "#E3B84D"
  red-500: "#EF6461"
  black-pure: "#000000"
  # ── camadas de estado (véus, nunca repintura)
  overlay-hover: "rgba(255,255,255,.08)"
  overlay-press: "rgba(255,255,255,.10)"
  # ── semânticos (Camada 1, já resolvidos para a base; overrides de lane na seção Lanes)
  surface: "{colors.ink-990}"
  surface-raised: "{colors.ink-980}"
  surface-card: "{colors.ink-960}"
  surface-elevated: "{colors.ink-940}"
  surface-drop: "{colors.ink-920}"
  surface-print: "{colors.paper-100}"
  text-primary: "{colors.white-pure}"
  text-brand: "{colors.paper-100}"
  text-secondary: "{colors.grey-350}"
  text-tertiary: "{colors.grey-400}"
  text-disabled: "{colors.grey-400}"
  text-error: "{colors.red-500}"
  accent: "{colors.lime-500}"
  status-live: "{colors.lime-500}"
  status-success: "{colors.lime-500}"
  status-attention: "{colors.amber-500}"
  status-error: "{colors.red-500}"
  status-idle: "{colors.grey-400}"
  border-selected: "{colors.grey-500}"
  border-subtle: "{colors.grey-500}"
  border-field-focus: "{colors.grey-500}"
  border-focus: "{colors.lime-500}"
  border-error: "{colors.red-500}"
  divider: "{colors.ink-940}"
  # ── PROPOSTA v0 (pendência 3 do Manifest, aguarda aprovação do Léo)
  # Paleta categórica de série de gráfico, dark-only, ordem FIXA chart-1→5.
  # Validada: banda OKLCH L .48–.67, croma ≥ .10, pior par adjacente CVD ΔE 10.0,
  # piso de visão normal 20.3, contraste ≥ 3:1 sobre ink-990 e ink-960.
  chart-1: "#0099A6"
  chart-2: "#BA823C"
  chart-3: "#6959AE"
  chart-4: "#1C8F6E"
  chart-5: "#C86EB0"
  chart-other: "{colors.grey-400}"
  # ── PROPOSTA v0: esqueleto de carregamento
  skeleton: "{colors.ink-940}"
typography:
  # ── escala de interface (px na Camada 0; interface implementa em rem = px/16)
  ui-display:
    fontFamily: Open Sans
    fontSize: 64px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.03em
  ui-title:
    fontFamily: Open Sans
    fontSize: 56px
    fontWeight: 300
    lineHeight: 1.1
    letterSpacing: -0.03em
  app-title:
    fontFamily: Open Sans
    fontSize: 48px
    fontWeight: 300
    lineHeight: 1.12
    letterSpacing: -0.02em
  ui-metric:
    fontFamily: Open Sans
    fontSize: 48px
    fontWeight: 300
    lineHeight: 1
    letterSpacing: -0.03em
    fontFeature: "'tnum'"
  app-metric:
    fontFamily: Open Sans
    fontSize: 44px
    fontWeight: 400
    lineHeight: 1.1
    letterSpacing: -0.03em
    fontFeature: "'tnum'"
  app-flow:
    fontFamily: Open Sans
    fontSize: 32px
    fontWeight: 300
    lineHeight: 1.15
    letterSpacing: -0.02em
  ui-section:
    fontFamily: Open Sans
    fontSize: 28px
    fontWeight: 300
    lineHeight: 1.2
    letterSpacing: -0.01em
  ui-lead:
    fontFamily: Open Sans
    fontSize: 20px
    fontWeight: 300
    lineHeight: 1.3
    letterSpacing: -0.01em
  ui-read:
    fontFamily: Open Sans
    fontSize: 17px
    fontWeight: 400
    lineHeight: 1.6
  ui-body:
    fontFamily: Open Sans
    fontSize: 14px
    fontWeight: 400
    lineHeight: 1.4
  ui-support:
    fontFamily: Open Sans
    fontSize: 13px
    fontWeight: 400
    lineHeight: 1.4
  ui-label:
    fontFamily: Open Sans
    fontSize: 12px
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: 0.04em
  # ── escala de arte (peça de marca; razão 1.25 a partir de 16; peso: grande = leve, 3.4)
  art-200:
    fontFamily: Open Sans
    fontSize: 200px
    fontWeight: 300
    lineHeight: 1.05
  art-100:
    fontFamily: Open Sans
    fontSize: 100px
    fontWeight: 300
    lineHeight: 1.05
  art-64:
    fontFamily: Open Sans
    fontSize: 64px
    fontWeight: 300
    lineHeight: 1.1
  art-40:
    fontFamily: Open Sans
    fontSize: 40px
    fontWeight: 300
    lineHeight: 1.15
  art-25:
    fontFamily: Open Sans
    fontSize: 25px
    fontWeight: 400
    lineHeight: 1.3
  art-16:
    fontFamily: Open Sans
    fontSize: 16px
    fontWeight: 400
    lineHeight: 1.5
rounded:
  xs: 4px
  sm: 8px
  md: 12px
  lg: 16px
  xl: 24px
  2xl: 28px
  pill: 999px
spacing:
  space-1: 4px
  space-2: 8px
  space-3: 12px
  space-4: 16px
  space-5: 24px
  space-6: 32px
  space-8: 48px
  target-min: 48px
  control-sm: 32px
  control-md: 40px
  control-lg: 56px
  row-2l: 64px
  disc-avatar: 52px
  disc-profile: 64px
  nav-w: 296px
  nav-w-compact: 232px
  nav-w-collapsed: 72px
  appbar-h: 80px
  topbar-h: 40px
  dock-h: 52px
  dock-clear: 96px
  doc-sm: 640px
  reading-max: 864px
  mail-w: 600px
  mail-pad: 40px
components:
  button-primary:
    backgroundColor: "{colors.surface-elevated}"
    textColor: "{colors.text-primary}"
    rounded: "{rounded.pill}"
    height: "{spacing.target-min}"
    padding: "{spacing.space-3}"
  button-cta-flow:
    backgroundColor: "{colors.text-brand}"
    textColor: "{colors.surface}"
    rounded: "{rounded.pill}"
    height: "{spacing.target-min}"
    padding: "{spacing.space-3}"
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.text-brand}"
    rounded: "{rounded.pill}"
    height: "{spacing.target-min}"
    padding: "{spacing.space-3}"
  button-destructive-confirm:
    backgroundColor: "{colors.status-error}"
    textColor: "{colors.surface}"
    rounded: "{rounded.pill}"
    height: "{spacing.target-min}"
  button-disabled:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.text-disabled}"
    rounded: "{rounded.pill}"
    height: "{spacing.target-min}"
  input:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.text-primary}"
    rounded: "{rounded.md}"
    padding: "{spacing.space-3}"
    height: "{spacing.target-min}"
  input-search:
    backgroundColor: "{colors.surface-card}"
    textColor: "{colors.text-primary}"
    rounded: "{rounded.pill}"
    height: "{spacing.control-md}"
  chip:
    backgroundColor: "{colors.surface-elevated}"
    textColor: "{colors.text-primary}"
    rounded: "{rounded.pill}"
    height: "{spacing.control-md}"
  card:
    backgroundColor: "{colors.surface-card}"
    rounded: "{rounded.md}"
  panel:
    backgroundColor: "{colors.surface-raised}"
    rounded: "{rounded.lg}"
  sheet:
    backgroundColor: "{colors.surface-card}"
    rounded: "{rounded.2xl}"
---

# Bullet Identity Source

> **Compilado do Bulletpedia** · `04 Growth/01 Foundation/Brand/Identity Source/00 Tokens And Manifest.md` · `versao-tokens: v1.15` (2026-08-29).
> O sistema chama-se **Identity Source**, nunca "design system" (P11). O Bulletpedia é a única fonte (P12): este arquivo é forma compilada, e quando divergir do Manifest, o Manifest manda. Valores marcados **PROPOSTA v0** ainda não existem no Manifest: aguardam aprovação do Léo (seção 9) antes de virarem lei.

## Overview

A Bullet é uma plataforma financeira em stablecoin. A interface é **dark por regra, não por tema** (P13): superfície clara só existe como exceção de meio (papel impresso). A linguagem é preto e branco com **um único acento funcional**, o verde `lime-500` — que marca ação e estado, nunca decora, nunca passa de 10% da composição e nunca preenche superfície.

O sistema resolve composição por **postura antes de valor**: separação se faz por salto de nível na rampa de superfícies, não por fio; profundidade sobe a partir do fundo e nunca inverte; sombra só quando algo flutua de verdade; ênfase se faz por hierarquia antes de cor; estado é um véu translúcido por cima do elemento, nunca repintura. O tom resultante é sóbrio, denso de informação e imediato — uma ferramenta financeira usada todos os dias, não uma vitrine.

Ordem de resolução em qualquer geração: **constraint dura → postura → tipo da lane → briefing → bloco → item → semântico → primitivo**. Valor bruto existe num lugar só (P1); tudo rio abaixo referencia nome semântico (P2).

## Colors

Na convenção deste formato: **primary** é a tinta principal da marca (`paper-100`, títulos e corpo de leitura), **secondary** o apoio (`grey-350`), **tertiary** o único driver de interação (`lime-500`, o acento funcional com cota de 10%), e **neutral** o chão de tudo (`ink-990` — o sistema é dark por regra, P13).

A base de toda interface é a **rampa de quatro superfícies**: `ink-990` (fundo de página) → `ink-980` (painel) → `ink-960` (card e container) → `ink-940` (estado ativo, chip, divider). O quinto degrau `ink-920` existe para um caso só: quando a rampa de quatro já foi consumida pelo próprio container (lista aberta dentro de card, thumb de segmentado). Nunca é card nem painel. Peça de marca (Social, Decks, Mídia Paga, WhatsApp) usa a **rampa de arte** de superfície única, de `ink-900` em diante.

- **Texto:** `white-pure` é exclusivo de interface (fora dela, branco puro é só do logo); `paper-100` carrega título e corpo de leitura; `grey-350` é o secundário (piso 4.5:1 sem arredondar); `grey-400` é terciário, label e régua. `grey-500` é **só contorno**, nunca texto; `#666666` é proibido em texto.
- **Acento:** `lime-500` com cota de 10%, nunca fundo, nunca sobre superfície clara, nunca sublinhado de link, nunca em pontuação.
- **Status:** `status-live` e `status-success` → lime; `status-attention` → amber; `status-error` → red; `status-idle` → grey. Status sempre acompanha forma, ícone ou rótulo — nunca só a cor. Cores de status são **reservadas**: nunca personificam série de gráfico.
- **Véus de estado:** `overlay-hover` (.08) e `overlay-press` (.10), sempre como camada por cima do container.
- **Fora do vocabulário** (nunca resolver um semântico para eles): navy `#0C0F17`/`#0D0F1A` e a paleta antiga do app; `#3a3a39`; cinzas azulados; `#E8705F`; qualquer lima que não seja `lime-500`; as cores de folha de sistema operacional (`#F2F2F7`, `#007AFF`…). Lista completa na seção 4.1 do Manifest.

## Typography

**Uma família só: Open Sans** (fallback Arial). Não existe segunda família na marca, nem exceção — JUST Sans, ainda rodando em pontos do app e do site, é dívida de migração. Valor financeiro usa **dígito tabular da própria família** (`tnum`), nunca troca de fonte.

Regra de peso: **grande é leve, pequeno é pesado** — o maior texto de qualquer composição é sempre o mais leve; texto pequeno e pesado não é título, é rótulo. Uma exceção, e só uma: valor financeiro grande usa peso regular, porque dígito fino em tamanho grande perde peso óptico.

- **Escala de interface** (`ui-*`, e `app-*` em tela de bolso): do `ui-display` 64 ao `ui-label` 12. `app-metric` 44 é o **único** tamanho de métrica do app (P18). A Camada 0 declara px; interface implementa em rem (px ÷ 16).
- **Escala de arte** (`art-*`): razão 1.25 a partir de 16 — 16 · 20 · 25 · 32 · 40 · 50 · 64 · 80 · 100 · 125 · 160 · 200. Tipo não segue o múltiplo de 4; segue a razão.
- **Piso absoluto de 12px** em toda a marca, inclusive label. Tracking sempre em `em`. `ui-label` roda uppercase com tracking de +0.04 a +0.06em (o token compila o piso 0.04).
- Título nunca em caixa alta; título isolado sem ponto final; sentence case. Nome de card não é título.

## Layout

Grade de **8px com sub-passo de 4** (`space-1` 4 → `space-8` 48). Todo espaçamento e todo raio é múltiplo de 4; valor fora da escala é erro auditável.

- **Alvo mínimo de interação: 48px** (`target-min`), que é também a altura única do botão primário. `control-sm/md/lg` (32/40/56) são o desenho do controle, nunca o alvo — o alvo se estende por área invisível.
- **Leitura:** texto corrido trava em `reading-max` 864px (`doc-sm` 640 para leitura estreita). Nunca aplicar largura de leitura em região de dados.
- **Navegação:** painel 296px (denso 232, trilho colapsado 72); barra de tela desktop 80px; app: topo 40px, dock 52px, folga de pé 96px. Canvas de referência do app: 390×844.
- **E-mail** é o único meio de largura travada: corpo 600px, respiro lateral 40px (`mail-pad`; `space-5` abaixo de 480), valores sempre inline porque cliente de e-mail não resolve variável CSS.
- Português ocupa cerca de 30% mais que inglês: reservar respiro. Lista rolável reserva a calha da barra de rolagem.

## Elevation & Depth

Profundidade é **tonal, pela rampa** — nunca por sombra em superfície plana. O que está na frente é um degrau mais claro que o que está atrás, e a hierarquia nunca inverte: painel jamais é mais escuro que a página, card jamais mais escuro que o painel (exceção declarada: a lane Email inverte de propósito, composição, não interface).

Sombra existe **só quando um elemento flutua de verdade**: menu, popover, folha sobreposta — `shadow-overlay: 0 12px 32px rgba(0,0,0,.55)`. Sempre escura sobre a própria escala, nunca colorida, nunca azulada. Thumb de controle segmentado não flutua: separa por salto de nível (`surface-drop`).

## Shapes

Escala fechada de raios, papel fixado por componente (P18):

- `xs` 4 — checkbox e controle mínimo · `sm` 8 — anel de foco, controle pequeno · `md` 12 — **card, item de lista, célula, campo** (campo compartilha o raio da família do card) · `lg` 16 — painel, menu · `xl` 24 — corpo de e-mail · `2xl` 28 — folha, dock e bloco de app · `pill` 999 — pill, chip, badge, avatar, **botão**.
- **Cápsula que anima canto usa raio finito** (`2xl`), nunca `pill`: quando a soma de dois raios excede a caixa, o navegador rescala todos e o canto oscila durante a animação. Em repouso, os dois são visualmente idênticos numa altura de 56.
- **Contorno é permitido em exatamente três casos** (postura 3.1): estado selecionado (`border-selected`, anel interno 1.5px), controle sem rótulo nem ícone que o identifique (`border-subtle`), e divisor estrutural (`divider`, máximo um por painel ou fronteira de região). **Qualquer quarto fio é erro auditável.** Card não tem borda; chip não tem borda; botão com rótulo legível não tem borda; campo de busca com lupa não tem borda.

## Components

As matrizes completas (anatomia × estado, item por item) vivem no Bulletpedia em `Identity Source/02 Components/` — 16 Items e 16 Blocos escritos. Este arquivo compila os contratos mais usados; **em conflito, a matriz do pedia manda.**

- **Button** — uma altura só (`target-min` 48), raio `pill`. Primário: container `surface-elevated`, rótulo `text-primary`. **O acento nunca preenche o container**: botão que precisa de destaque usa elevação, não cor. CTA de conclusão de fluxo (app): container claro `text-brand` com rótulo `surface` — ênfase máxima, um por contexto. Secundário: transparente com `border-subtle` e rótulo `text-brand`. Ação destrutiva usa `status-error` de fundo **só na segunda pergunta de apagar**. Disabled: `surface-card` + `text-disabled`, sem toque. Confirmação irreversível em toque **segura em vez de tocar**: pressão contínua com progresso visível (`motion-grow`, linear); soltar cancela.
- **Text Field** — superfície **um degrau acima do container em que está** (sobre página → `surface-card`; sobre card → `surface-elevated`), sem borda em repouso: o salto de nível separa. Raio `md`. Foco pelo **anel interno da própria caixa** (`border-field-focus`, 2px), nunca o anel verde externo. Erro: `border-error` 1.5px interno + mensagem em `text-error` — nunca só o anel. Placeholder nunca substitui o rótulo. Variante busca: lupa à esquerda, raio `pill`, altura `control-md` estendida a `target-min`, sem fio.
- **Estados (todo controle)** — hover e pressed são **véus por cima** (`overlay-hover`/`overlay-press` em pseudo-elemento), nunca troca de background (P14). Estado nunca é comunicado só por cor. Foco tem dois portadores: campo foca pela própria caixa; todo controle **sem** caixa de digitação foca pelo anel externo `border-focus` (verde, 2px, offset 2, raio `sm`). Nenhum controle focalizável fica sem portador de foco.
- **Bloco arranja, não repinta** (P14): um bloco nunca redefine cor, borda ou estado de um item que monta. Item responde a interação; bloco responde a conteúdo (cheio · vazio · carregando · erro · sem permissão). Componente com mais de uma variante fixa a condição de uso de cada uma — variante nunca é escolha de gosto.

## Do's and Don'ts

- Do: separar por salto de nível na rampa; fio só nos três casos permitidos.
- Do: contraste mínimo 4.5:1 em texto (sem arredondar) e 3:1 em elemento não textual que identifica componente ou estado.
- Do: dígito tabular em todo valor financeiro; moeda por código ISO em texto.
- Do: `prefers-reduced-motion: reduce` corta toda animação, sem exceção.
- Do: animar apenas `opacity` e `transform` (altura só em crescimento no lugar, via FLIP), alvo 60fps, texto legível durante todo o movimento.
- Don't: cifrão como grafismo. Em texto, código ISO.
- Don't: travessão — em peça, em tela e em assinatura.
- Don't: segunda família tipográfica, em qualquer contexto.
- Don't: neon, holograma, glitch e futurismo.
- Don't: logo digitado. "bullet." é sempre asset: uma ocorrência por tela, altura mínima 21px, nunca sem o ponto, e o ponto do logo **nunca é verde**.
- Don't: pontuação com `accent` — pontuação herda a cor do texto, sempre.
- Don't: texto abaixo de 12px, em qualquer escala, inclusive label.
- Don't: bounce, elastic ou overshoot em movimento.
- Don't: sombra colorida ou azulada; sombra em superfície que não flutua.
- Don't: verde como fundo ou preenchendo superfície; verde acima da cota de 10%.
- Don't: título em caixa alta; ponto final em título isolado.

## Motion

| Papel | Duração | Curva |
|---|---|---|
| `motion-quick` — hover, foco, toggle | 200ms | `ease-standard` `cubic-bezier(.2,0,0,1)` |
| `motion-base` — abrir, fechar, expandir pequeno | 250ms | `ease-standard` |
| `motion-shape` — morfo de canto de cápsula | 400ms | `ease-settle` `cubic-bezier(.32,.72,0,1)` |
| `motion-rotate` — rotação de ícone | 500ms | `ease-standard` |
| `motion-grow` — crescimento de container no lugar | 650ms | `ease-settle` |
| entrada de elemento | — | `ease-enter` `cubic-bezier(.05,.7,.1,1)` |
| saída de folha e véu | — | `ease-exit` `cubic-bezier(.3,0,.8,.15)` |
| peça de arte | — | `ease-brand` `cubic-bezier(0.22,1,0.36,1)` |

Duas curvas por domínio: interface responde a toque e parece imediata; peça de arte é apresentação. **Movimentos que acontecem juntos usam o mesmo relógio** — rolagem que acompanha um container crescendo usa a mesma duração e a mesma curva do container.

## Dataviz — PROPOSTA v0 (fecha a pendência 3 do Manifest)

A Camada 0 não define cor de série de gráfico e "dashboards inventam cor" (pendência 3). Proposta, construída pela fórmula de paleta categórica (banda de luminosidade OKLCH dark 0.48–0.67, croma ≥ 0.10, separação CVD por Machado 2009, piso de visão normal ΔE ≥ 15) e **validada por script, não a olho** — pior par adjacente ΔE 10.0 (deutan), piso normal 20.3, contraste ≥ 3:1 sobre `ink-990` e `ink-960`:

1. `chart-1` ciano `#0099A6` · 2. `chart-2` bronze `#BA823C` · 3. `chart-3` violeta `#6959AE` · 4. `chart-4` teal `#1C8F6E` · 5. `chart-5` magenta `#C86EB0`

- **Ordem fixa, nunca ciclada.** A 6ª série em diante dobra em "Outros" (`chart-other` = `grey-400`). Scatter, bolha, mapa e small multiples: máximo **3 séries** (all-pairs validado até o slot 3); acima disso, facetar.
- **`lime-500` nunca é cor de série.** Ele já é status (`status-live`, `status-success`) e status nunca personifica série; além disso, sua luminosidade (OKLCH L≈0.90) estoura a banda dark. O verde em gráfico marca **estado e destaque funcional** (linha de meta, ponto vivo), contando na cota de 10%.
- `amber-500` e `red-500` idem: reservados a status. Série que *significa* bom/ruim veste status; série que é só "série 4" veste categórica — nunca os dois no mesmo gráfico.
- Texto de gráfico veste tokens de texto, nunca a cor da série. Grid e eixo: `divider`/`grey-400`.
- Direção a fechar depois (não bloqueia): sequencial = rampa neutra `paper-100 → grey-500` (magnitude, monótona); divergente = `chart-2` ↔ `chart-1` com ponto médio `grey-400`.

## Assets & Iconografia

**Asset não se redesenha: copia-se do banco, byte a byte.** Recriar asset existente é erro auditável; asset novo entra no banco **antes** de aparecer em peça.

- **Logos** — repo canônico `Leobullet016/brand-assets/svg/`: 5 lockups (`bullet`, `b` icon, `bulletcash`, `bulletpay`, `bulletpro`) em preto e branco. Os `_white` têm `#fff` fixo; os `_black` não declaram fill (recoloríveis via CSS). Regras de uso na seção Do's and Don'ts.
- **Backgrounds noise** — `brand-assets/backgrounds/`: 14 PNGs 1920×1080 em escala de cinza. Textura: `noise-opacity` 5–15%, sempre transparente sobre `black-pure`.
- **Ícones** — spec: `viewBox="0 0 24 24"` sem width/height, coordenadas 2–22, `stroke-width` 2, linecap/linejoin `round`, `currentColor`, par outline + filled com geometria idêntica, kebab-case, máximo 5 shapes, sem raster/sombra/gradiente/texto. Ativo de navegação usa **filled**; demais, **outline**. Banco: `Identity Source/03 Assets/Icons.md` (31 canônicos + marcas). Bandeiras: `03 Assets/Flags.md`. Em e-mail, ícone é raster por URL.

## Lanes (contextos de aplicação)

Nove lanes em três tipos (P15): **gabarito** (Email, Decks, Materiais Físicos — estrutura fixa, conteúdo variável), **composição** (Social, WhatsApp, Mídia Paga — estrutura variável guiada por restrição) e **sistema** (App, PLT Internas, Website — produto com estado e navegação). Lane declara **só o que difere** da base (P5) e só re-aponta um semântico quando **o meio força** (P16): o renderizador quebra (Gmail inverte fundo verde → botão de e-mail é claro), o substrato é outro (papel → `surface-print`), ou a distância de leitura muda (deck → escala de projeção). "Ficou melhor assim" não é causa. Postura nunca mora em lane. Docs por lane em `Identity Source/01 Lanes/`.

## Pendências e governança

- Este arquivo compila `versao-tokens: v1.15`. Mudança nasce no Manifest; este arquivo regenera e o tema Astryx (`export css-vars`) regenera junto.
- **PROPOSTAS v0 aguardando aprovação do Léo** (entram na seção 9 do Manifest antes de virarem lei): paleta categórica `chart-1…5` + `chart-other` (fecha a pendência 3) · `skeleton` = `surface-elevated` para estado carregando · direção de sequencial/divergente (acima).
- Pendências do Manifest que este arquivo **não** resolve (seguem lá): ferramenta canônica de motion (5), modelo canônico de e-mail (6), link de e-mail (7), superfícies de e-mail (8), `border-box` como quarto fio (9), `text-primary` no Website (10).
- Aprovação de qualquer mudança no Identity Source é do Léo. Fora de `Identity Source/`, não se escreve sem aprovação.
