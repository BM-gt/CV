# Proyecto CV — Bautista Maloneay

## Links principales

| Recurso | URL |
|---|---|
| CV público (web) | https://bm-gt.github.io/CV/ |
| Repositorio GitHub | https://github.com/BM-gt/CV |
| Branch de trabajo | `claude/confident-ride-ve7zwf` |
| Archivo principal | `bautistamaloneay.html` |
| Redirect raíz | `index.html` |

---

## Estructura del repositorio

```
BM-gt/CV
├── bautistamaloneay.html   ← CV completo (único archivo, self-contained)
└── index.html              ← Redirige automáticamente al CV
```

---

## Descripción del CV

Archivo HTML único, completamente autocontenido:
- Sin dependencias externas (imágenes y video embebidos como base64)
- Fuentes: Space Grotesk, Inter, Space Mono, Playfair Display (Google Fonts)
- Fondo animado de estrellas (`#starsCanvas`)
- Bilingüe: español / inglés con toggle (botones `ES` / `EN` en nav)
- Animaciones: scroll-reveal (IntersectionObserver), typewriter, counters, rings, orbs

### Secciones del CV
1. **Gate de entrada** — pantalla de bienvenida con selección de idioma
2. **Hero** — foto, nombre animado, título, quote, stats (+9 años / +40 marcas), scroll hint
3. **Trayectoria** — WTF¿ Agency / CraveroLanis / CECCa / Audi Argentina
4. **Marcas trabajadas** — 22 categorías, 48 marcas en layout masonry 3 columnas
5. **Herramientas · Idiomas** — AI Tools + Idiomas
6. **Datos de interés** — 3 ítems en grid
7. **Portafolio** — 4 casos (Sensus, Agua SELTZ, SHAQ, Diablo Pisco) con modales
8. **Contacto** — email/teléfono (copy tooltip), LinkedIn, orbs animados

---

## Variables CSS principales

```css
--bg: #050505
--s1: #0d0d0d
--s2: #141414
--a:  #D63B7F   /* rosa acento */
--w:  #F0F0F0   /* blanco texto */
--mid: #777
--faint: #1c1c1c
```

---

## Trayectoria (contenido actual)

### WTF¿ Agency — Brief Destroyers · 3 años · 2023 — Actualidad
- **2025 — Actualmente** · Head of Social Media · Coordinador Digital
- **2024 — 2025** · Jefe de Coordinación Operativa
- **2023 — 2025** · Social Media Manager

### CraveroLanis — 2016 — 2026 · Freelance
- **2021 — 2026** · Ejecutivo de Cuentas
- **2021 — 2023** · Community Manager
- **2016 — 2017** · Asistente de Gerencia

### CECCa — 2019 — 2024 · ONG
- CM · Coordinador general de Staff

### Audi Argentina — 2017 — 2019 · Varios puestos
- De limpieza a asesor comercial · 2 ediciones en Summer Experience Cariló

---

## Casos de portafolio (objeto CASES en JS)

| ID | Título ES | Tipo |
|---|---|---|
| `sensus` | El brindis, resignificado. | Dirección creativa · Rebranding · Best Branding Awards Chile |
| `seltz` | Seamos más transparentes. | GLUP! · Campaña 360° · 5 comerciales |
| `shaq` | Hablar sin hablar. | SHAQ Footwear en OLGA · Publicidad indirecta |
| `diablo` | Revela tu esencia. | Concepto de marca · Spot · Estrategia digital |

El caso SHAQ incluye video embebido como base64 (vertical, modal `verticalVideo:true`).

---

## Datos de contacto (en el CV)

- **Email:** baumaloneay@gmail.com
- **Teléfono:** 011 · 3191 · 1403
- **LinkedIn:** https://www.linkedin.com/in/bautista-maloneay-b5483721b/
- **CV web:** https://bm-gt.github.io/CV/

> Email y teléfono no son links directos — abren un tooltip con botón "Copiar" para proteger el scraping.

---

## Funcionalidades JS clave

```
enter(lang)         → entra al sitio desde el gate
applyLang(lang)     → aplica ES/EN a todos los data-es/data-en
openModal(id)       → abre modal de caso de portafolio
closeModal()        → cierra modal
switchTab(tab)      → navega entre CV / Portafolio / Contacto
initStars()         → inicia canvas de estrellas
startTypewriter()   → animación de nombre en hero
countUpStats()      → anima contadores +9 / +40
initReveal()        → IntersectionObserver para .rv (scroll reveal)
showCopyTip(e,val)  → tooltip de copia para email/teléfono
```

---

## GitHub Pages

- **Activado en:** branch `claude/confident-ride-ve7zwf`, carpeta `/`
- **URL:** https://bm-gt.github.io/CV/
- El `index.html` redirige automáticamente a `bautistamaloneay.html`
- Repo **público** (requerido para GitHub Pages gratuito)
- Favicon: SVG inline con monograma **BM** en rosa `#D63B7F`

---

## Historial de commits relevantes

```
2707518  Add favicon: BM monogram in pink on dark background
bd91080  Rename CV file: remove version suffix from filename
116fb26  Add index.html redirect for GitHub Pages
c694229  Scroll hint: 'Bajá' en español, más grande, centrado en mobile
5173beb  Marcas: column-count masonry layout
efa888d  Animación de respiración rosa en Contacto + fondo estrellado
02fc8a6  Fondo estrellado continuo, contador marcas a +40
7860901  Restaurar Herramientas·Idiomas y revertir colores de marcas
5d24861  Iconos de contacto con vibración continua
ecda1b9  Email/teléfono con tooltip de copia (sin links directos)
```

---

## Para retomar en una nueva sesión

1. Clonar o abrir el repo: `github.com/BM-gt/CV`
2. Branch de trabajo: `claude/confident-ride-ve7zwf`
3. Archivo a editar: `bautistamaloneay.html`
4. El CV live siempre se actualiza en: https://bm-gt.github.io/CV/
5. Cada cambio que se commitee y pushee al branch se refleja en 1-2 minutos en la web

---

## PDFs (pendiente)

Los PDFs (CV ES/EN y Portfolio ES/EN) fueron generados y luego eliminados del historial a pedido. Cuando se retome, regenerarlos con Playwright renderizando el HTML directamente para preservar fondo, imágenes y tipografías.

```python
# Comando base para regenerar
PLAYWRIGHT_BROWSERS_PATH=/opt/pw-browsers python3 generate_pdfs.py
# Chromium path: /opt/pw-browsers/chromium-1194/chrome-linux/chrome
```
