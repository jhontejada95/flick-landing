# Flick — landing page

Landing standalone del proyecto (separada de la app real en
`flick-uxmaxx.vercel.app`). Un solo archivo, `index.html`, sin build step —
pensado para GitHub Pages.

## Publicar en GitHub Pages

1. Creá un repo nuevo (puede llamarse `flick` o `flick-landing`).
2. Subí `index.html` a la raíz del repo (rama `main`).
3. En el repo: Settings → Pages → Source → "Deploy from a branch" → rama
   `main`, carpeta `/ (root)` → Save.
4. En un par de minutos queda publicado en
   `https://<tu-usuario>.github.io/<nombre-del-repo>/`.

## Qué muestra

- Hook consumer (hero, diferenciales, mockups de las 3 pantallas).
- Sección para jueces: arquitectura del relay vía escrow, hash de una
  transacción real verificable en Basescan, checklist de seguridad.
- Ticker en vivo: consume `GET https://flick-uxmaxx.vercel.app/api/stats/flicks-count`
  (CORS abierto solo en ese endpoint, es un conteo agregado sin PII).
- Todos los botones "Open Flick" / "Try Flick" enlazan directo a
  `https://flick-uxmaxx.vercel.app`.

## Paleta y tipografía

Reutiliza 1:1 los tokens del design system de la app ("Flick Liquid
Convergence", generado en Stitch): fondo `#0B0F19`, azul `#5B8DEF`, ámbar
`#FFB020`, esmeralda `#34D399`; Space Grotesk / DM Sans / JetBrains Mono.
