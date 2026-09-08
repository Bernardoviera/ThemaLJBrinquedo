# LJ Brinquedos — tema Shopify

Tema da loja LJ Brinquedos, baseado no [Dawn](https://github.com/Shopify/dawn) (Shopify, licença MIT — ver `LICENSE.md`), Online Store 2.0.

## Estrutura

- Locale padrão: `pt-BR` (`locales/pt-BR.default.json`, `locales/pt-BR.default.schema.json`)
- Paleta e estilo: `config/settings_data.json` (5 esquemas de cor, cantos arredondados, cart drawer)
- Seções próprias: `sections/shop-by-age.liquid` (compra por faixa etária), `sections/gift-finder-banner.liquid` (banner de presentes)
- Home: `templates/index.json`

## Skill instalada

`.claude/skills/caveman/SKILL.md` — modo de resposta compacto do Claude Code (via `CLAUDE.md`), sem efeito no tema em si.

## Desenvolvimento

Precisa da [Shopify CLI](https://shopify.dev/docs/api/shopify-cli):

```
shopify theme dev --store <sua-loja>.myshopify.com
```

Validação estática (sem loja conectada):

```
npx @shopify/cli theme check
```

## Pendências antes de publicar

- Conectar a loja Shopify real e rodar `theme dev`/`theme push`.
- Cadastrar collections reais e apontar os links de `shop_by_age`/`gift_finder_banner` (hoje usam `shopify://collections/all` como placeholder).
- Subir logo e imagens de produto/banner (hoje usam os placeholders SVG do Dawn).
