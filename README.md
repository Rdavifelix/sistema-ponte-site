# Site — mercado brasileiro nos EUA

Site estático, sem build e sem dependência: é só abrir o HTML ou subir os arquivos em qualquer host.

## Páginas

| Arquivo | O que é |
|---|---|
| `index.html` | Página de produto **"Site que funciona"** — sistema claro com faixas escuras alternadas (navy + dourado, Sora). |
| `landing-vsl.html` | Landing de aquisição para tráfego pago — modelo escuro de funil VSL (Geist + Instrument Serif, CTA com glow). |
| `DESIGN-SYSTEM.md` | Os tokens e as regras de uso dos dois sistemas visuais. |

## Antes de subir

1. **`MARCA`** e **`WHATSAPP`** — duas constantes no `<script>` no fim de cada HTML. Enquanto não trocar, todos os botões apontam para um número fictício.
2. **Pixel do Meta** — há um slot comentado no `<head>` de `landing-vsl.html`. O clique em qualquer botão de WhatsApp já dispara `fbq('track','Contact')`.
3. **`privacidade.html` e `termos.html`** — não existem ainda e são exigidos na revisão de anúncio do Meta.
4. **Mídia** — os blocos entre colchetes (`[PRINT: …]`, `[VSL DE 5 MINUTOS…]`) são slots. Se for subir antes de produzir a mídia, apague o bloco em vez de deixar a caixa vazia.

## Duas decisões que parecem erro e não são

**Não há depoimento de cliente.** Onde normalmente fica a parede de depoimentos, há um bloco dizendo em voz alta que ainda não existe cliente, com os slots esperando os vídeos reais. É decisão de projeto: neste mercado todo mundo se conhece, e depoimento inventado é descoberto em uma semana.

**Todo número tem fonte no nome.** BrightLocal, Hook Agency, Jobber. Número sem fonte foi cortado, mesmo quando ajudava o argumento.
