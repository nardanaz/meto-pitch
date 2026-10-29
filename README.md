# MeTo · Pitch BAC IAE

Deck interactivo para el Business Angels' Club del IAE Business School.

**Live:** se completará al deploy en Vercel.

## Contenido

- Hero + isotipo animado
- Problema, insight, solución
- Demo interactivo del producto (mockups del MVP)
- Mercado (TAM/SAM/SOM), competencia, modelo de negocio
- Tracción + roadmap
- Dashboard financials con 4 charts (Recharts)
- Equipo, ask (USD 300k pre-seed), visión, contacto

## Stack

HTML + React 18 (via CDN UMD) + Recharts 2.12 + Inter (Google Fonts).
Self-contained: imágenes embebidas como data URIs base64.

## Build

Regenerar desde los mockups del repo principal:

```bash
cd ../
python scripts/build-pitch-html.py
cp legal/pitch/pitch-interactive.html pitch-site/index.html
git -C pitch-site add -A && git -C pitch-site commit -m "update deck" && git -C pitch-site push
```

Vercel re-deploya automáticamente al push.

---
Avalon Agency SRL · hola@meto.com.ar
