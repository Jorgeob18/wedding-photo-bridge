# Wedding Photo Bridge - AGENTS.md

## Project Context
Landing page para boda de Abdiel & Abigahil. El objetivo es redirigir a los invitados (vía QR físico) a `https://knipsmig.com/Z3749o5k` para subir fotos/videos del evento.

## Tech Stack
- HTML5 + Tailwind CSS (CDN)
- Google Fonts: `Noto Serif` (display), `Manrope` (body)
- Icons: Google Material Symbols Outlined

## Critical Constants (Never Change)
- **URL**: `https://knipsmig.com/Z3749o5k` - Toda acción de "compartir/subir" debe redirigir aquí
- **Nombres**: "Abdiel & Abigahil" o "Abdiel & Abigail"
- **Fecha**: 14 de junio de 2026
- **Ubicación**: Tapalpa, Jalisco

## Design System
--follow `docs/design.md` ("Editorial Romance")
- No hard borders - usa tonal shifts y glassmorphism
- Primary gradient: `primary-container` → `primary` (#c05178)
- Mobile-first: 95% de usuarios vienen de móvil

## Source Code
- Entrada: `src/index.html` (a crear)
- PWA: `src/manifest.json` (a crear)

## Commands
```bash
# Preview local
npx serve src

# Deploy (Netlify/Vercel)
git push origin master
```