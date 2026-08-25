# Sistema visual

Dois sistemas convivem neste repositório, um por página. Os valores abaixo são os que estão de fato no CSS — servem como referência para manter consistência ao criar páginas novas.

---

## A. `landing-vsl.html` — escuro, funil de aquisição

| Token | Valor |
|---|---|
| Fundo | `#04070f` + grid de 58px a 2,8% de branco + brilho radial azul no topo |
| Card | `radial-gradient(120% 90% at 50% -10%, rgba(59,130,246,.16), transparent 62%)` sobre `linear-gradient(160deg,#131b2c,#070b15)` |
| Borda | `1px solid rgba(255,255,255,.09)` · raio `13px` |
| Sombra de card | `inset 0 1px 0 rgba(255,255,255,.08), inset 0 0 60px rgba(255,255,255,.03), 0 40px 90px -50px rgba(0,0,0,.9)` |
| Texto | branco `#fff` · corpo `#b3b8c2` · fino `#9aa2b2` |
| Azul | `#3b82f6` · claro `#93c5fd` · fundo `rgba(37,99,235,.1)` |
| Tipografia | **Geist** 400/500/600/800 + **Instrument Serif** itálico nos destaques |
| H1 | `clamp(30px,4.4vw,48px)` · 800 · lh 1.1 · ls -.02em · centralizado |
| Rótulo de seção | 11,5px · 600 · uppercase · ls .16em · azul claro |
| Badge do topo | pill, borda 1px, 11,5px, uppercase, ls .13em, com ponto luminoso |
| CTA | altura 52px · raio 12px · peso 600 · gradiente azul com 5 sombras empilhadas (anel + glow) |

**Regras de uso**

- **Um destaque só por título.** O sublinhado azul marca uma frase por H1 — no caso, o preço. O itálico serifado marca uma palavra por H2. Dois sublinhados no mesmo título anulam os dois.
- **Serifado itálico só em título.** Em corpo de texto e em letra miúda ele lê como defeito de fonte.
- **O verde do WhatsApp saiu dos botões.** Quebrava o sistema cromático; o canal continua legível pelo ícone dentro do botão. Para voltar ao verde, trocar as 4 linhas de `--cta-*` no `:root` (estão comentadas no arquivo).
- **Nada de estrela, contagem de review ou logo de cliente** enquanto não houver cliente. No lugar entram as pílulas de fato (`$297/mês`, `Sem contrato`, `No ar em 10 dias úteis`) e os blocos de vazio declarado.

**Ordem das seções:** logo → badge → H1 → sub-linha → CTA → pílulas de fato → card de vídeo → marquee de ferramentas → as 5 tábuas → serve / não serve → prova → processo → FAQ → fecho com glow → rodapé.

---

## B. `index.html` — claro, página de produto

| Token | Valor |
|---|---|
| Fundo | `#F1F1F1` com cards brancos |
| Faixas escuras | `#1F2236` |
| Destaque | dourado `#E8A743` — números, H3 das features, botões |
| Texto | `#000` no claro · `#C4C6CD` no escuro · secundário `#5B5F6B` |
| Tipografia | **Sora** 400/600/700/800/900 |
| H1 | `clamp(28px,4.4vw,48px)` · 900 · centralizado, navy |
| Raios | `10px` em botão e card pequeno · `12px` em card grande |
| CTA | altura 50px · raio 10px · fundo dourado · texto `#1a1205` |

**Regras de uso**

- **Nav branca fixa** com logotipo à esquerda e botão dourado à direita.
- **Features alternam lado** (`.feat` / `.feat.rev`): texto de um lado, mídia do outro, com H3 dourado precedido de ícone em quadrado de fundo âmbar.
- **Todo número tem fonte nomeada embaixo** (`<cite>`). Número sem fonte não entra.

**Ordem das seções:** nav → H1 → [3 cards de estatística | card de demonstração] → faixa escura com 4 features → faixa de CTA → 3 passos → prova → fecho → rodapé escuro em 4 colunas.

---

## O que vale para as duas

- Mobile primeiro: o tráfego chega pelo celular, muitas vezes pelo navegador de dentro do Instagram, onde a altura útil fica entre 560 e 620px. O botão principal tem que caber aí.
- Preço visível acima da dobra, sempre.
- Nenhuma promessa de número de lead, de job ou de posição no Google, em nenhuma peça.
- Slots de mídia entre colchetes são para preencher ou apagar — nunca para publicar como estão.
