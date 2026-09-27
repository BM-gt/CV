# Proyecto CV — Bautista Maloneay
> Documento para retomar el proyecto en cualquier cuenta de Claude sin perder nada.

---

## Estado actual

- **CV público y visible en:** https://bm-gt.github.io/CV/
- **Ese link no depende de Claude ni de esta cuenta** — está en GitHub y sigue funcionando siempre.
- **Repositorio:** https://github.com/BM-gt/CV (público)
- **Branch de trabajo:** `claude/confident-ride-ve7zwf`
- **Archivos en el repo:**
  - `bautistamaloneay.html` — el CV completo (único archivo, todo embebido)
  - `index.html` — redirige automáticamente al CV desde la raíz
  - `PROYECTO_CV.md` — este archivo

---

## Cómo retomar en una nueva sesión de Claude

1. Abrir nueva sesión en claude.ai/code
2. Conectar el repo `BM-gt/CV` de GitHub
3. Compartir este archivo `.md` al inicio
4. El archivo a editar siempre es: `bautistamaloneay.html`
5. Branch: `claude/confident-ride-ve7zwf`
6. Cada cambio commiteado y pusheado se refleja en https://bm-gt.github.io/CV/ en 1-2 minutos

---

## Descripción del CV

Archivo HTML único, **completamente autocontenido** (sin dependencias externas):
- Todas las imágenes y video embebidos como base64 dentro del HTML
- Fuentes externas: Space Grotesk, Inter, Space Mono, Playfair Display (Google Fonts)
- Fondo animado de estrellas (`#starsCanvas`, `z-index:0`, fixed)
- **Bilingüe:** español / inglés con toggle (botones en el gate de entrada y en nav)
- Tema oscuro con acento rosa

---

## Variables CSS

```css
:root {
  --bg: #050505;
  --s1: #0d0d0d;
  --s2: #141414;
  --a:  #D63B7F;   /* rosa acento — usado en todo */
  --w:  #F0F0F0;   /* blanco texto */
  --mid: #777;
  --faint: #1c1c1c;
}
```

---

## Estructura del CV — secciones

| Sección | Descripción |
|---|---|
| Gate | Pantalla de entrada con selección ES / EN, animación de orbs |
| Hero | Foto (base64), nombre animado (typewriter), título, quote, stats +9/+40, scroll hint |
| Trayectoria | 4 empresas con logos SVG, roles y descripciones |
| Marcas trabajadas | 22 categorías / 48 marcas, layout masonry `column-count:3` |
| Herramientas · Idiomas | AI Tools + Idiomas en grid 2 columnas |
| Datos de interés | 3 ítems en grid 3 columnas |
| Portafolio | 4 casos con modales (Sensus, Agua SELTZ, SHAQ, Diablo Pisco) |
| Contacto | Email/teléfono con tooltip de copia, LinkedIn, orbs animados |

---

## Trayectoria (contenido exacto)

### WTF¿ Agency — Brief Destroyers · 3 años · 2023 — Actualidad
- **2025 — Actualmente** · Head of Social Media · Coordinador Digital
  - Liderazgo del área digital con integración de IA. Coordinación de cuentas en Argentina, Chile, Perú y Paraguay.
- **2024 — 2025** · Jefe de Coordinación Operativa
  - Cabeza del equipo creativo. Gestión de tiempos, briefs y recursos. Me postulé al puesto al quedar vacante.
- **2023 — 2025** · Social Media Manager
  - Entré para armar el equipo digital de WTF. Lideré a cuatro CMs. Marcas: Sensus, Hydrate, SHAQ, Starter, Morelli, Agua SELTZ, Timberland, Grupo Capel, IPONE, entre otras.

### CraveroLanis — 2016 — 2026 · Freelance
- **2021 — 2026 · Freelance** · Ejecutivo de Cuentas
  - Consultoría estratégica, creativa y gestión de la cuenta Cerro Castor.
- **2021 — 2023** · Community Manager
  - La Serenísima, Patrick, Ibupirac, Medincare, Champ Frère. Mayor caso: Campaña Schneider Mundial Qatar 2022.
- **2016 — 2017** · Asistente de Gerencia
  - Primera experiencia profesional. Soporte directo a la gerencia.

### CECCa — 2019 — 2024 · ONG
- **2019 — 2024** · CM · Coordinador general de Staff
  - Gestión de redes y coordinación del stand en Expo Cannabis Argentina (La Rural), primeras 3 ediciones.

### Audi Argentina — 2017 — 2019 · Varios puestos
- **2017 — 2019** · De limpieza a asesor comercial · 2 ediciones en Summer Experience Cariló
  - Operario → logística → administración → asesor comercial → representación de marca en Cariló.

---

## Casos de portafolio

### 01 — Sensus (Espumante)
- **Título ES:** El brindis, resignificado.
- **Título EN:** The toast, redefined.
- **Tipo:** Dirección creativa · Rebranding · Best Branding Awards Chile · WTF¿ Agency
- **Video:** YouTube embed `3iMdnmVZQpk`
- **Desc ES:** Sensus necesitaba renovar su fee en WTF¿. El pitch se ganó resignificando el "brindis". El concepto se convirtió en la dirección creativa completa incluyendo rebranding de etiquetas. Participamos en dos categorías de los Best Branding Awards Chile.
- **Rol ES:** Instalé la idea base en el brainstorming. Ejecutivo de cuentas de Sensus.

### 02 — Agua SELTZ
- **Título ES:** Seamos más transparentes.
- **Título EN:** Be more transparent.
- **Tipo:** GLUP! · Campaña 360° · 5 comerciales · WTF¿ Agency
- **Videos:** 5 YouTube embeds (uwe_INppX4M / 04TUOAU0z3Q / W2jJ5yDaOxI / d65ULYGAgXw / GOer1Slgz78)
- **Desc ES:** 5 comerciales con el insight "GLUP" — ese momento incómodo en que no sabés cómo decir algo difícil. Situaciones: amigos, entrevista, cita, clasificación de Paraguay al Mundial 2026.
- **Rol ES:** Guiones iniciales, lideré estrategia digital de lanzamiento y plan de medios.

### 03 — SHAQ Footwear
- **Título ES:** Hablar sin hablar.
- **Título EN:** Talking without talking.
- **Tipo:** SHAQ Footwear en OLGA · Publicidad indirecta · Estrategia de presencia
- **Video:** Local, embebido como base64 (~4.5MB), vertical (`verticalVideo:true`)
- **Desc ES:** Estrategia no convencional: llevar SHAQ Footwear a OLGA a través de publicidad indirecta. Visibilidad orgánica en contexto de alto alcance.
- **Rol ES:** Concepto estratégico, desarrollo de la idea y coordinación de la ejecución.

### 04 — Diablo Pisco (numerado como 05 en el JS)
- **Título ES:** Revela tu esencia.
- **Título EN:** Reveal your essence.
- **Tipo:** Concepto de marca · Spot · Estrategia digital · WTF¿ Agency
- **Video:** YouTube embed `vsDNnfPoSdg`
- **Desc ES:** Nuevo concepto creativo "Revela tu esencia". Concepto, guion del spot y acompañamiento en ejecución audiovisual. Estrategia de lanzamiento en redes.
- **Rol ES:** Pensamiento creativo del concepto y spot. Estrategia digital post producción.

---

## Herramientas · Idiomas

### AI Tools
| Herramienta | Rol |
|---|---|
| Claude | Principal |
| ChatGPT | Estrategia |
| Gemini | Análisis |
| ImageFX · Magnific | Visual |
| Freepik AI · Nano Banana | Imagen |

### Idiomas
| Idioma | Nivel |
|---|---|
| Español | Nativo |
| Inglés | B2 Alto · B2 First |
| Portugués | Básico |

---

## Datos de interés

- Psicología · UCA (hasta 4to año)
- Carnet de conducir B1 · Vehículo propio
- Ciudadanía italiana vigente · Visa EE.UU vigente

---

## Marcas trabajadas (22 categorías)

| Categoría | Marcas |
|---|---|
| Espumantes | Sensus · Broccato · Grupo Valdivieso · DIVA · MUM Argentina |
| Piscos | Alto del Carmen · Diablo Pisco · Estrella del Elqui · Hacienda la Torre · Monte Fraile · Mal Paso · Cooperativa Capel |
| Whisky | Cutty Sark · Old Virginia |
| Mezcal | Ojo de Tigre |
| Tequila | José Cuervo Chile |
| Mixología & coctelería | Master of Mixes |
| Sidras | Sidra 1888 |
| Bebidas | Agua SELTZ Paraguay |
| Cervezas | Schneider · Kozel · Pilsner Urquell · Rural |
| Calzado | Shaq Footwear · Starter Argentina · Timberland Argentina |
| Electrodomésticos | Morelli Cocinas · Patrick |
| Productos isotérmicos premium | HYDRATE Argentina |
| Automotriz | MAHLE · AUDI |
| Motociclismo | IPONE Argentina · Alpinestars Argentina |
| Lácteos y alimentos | La Serenísima · Sembrasol · Kapi |
| Farmacéutica | Ibupirac / Pfizer |
| Salud y cuidado | Medincare · Senior Care |
| Programas internos | Motounplugged Motorola Argentina |
| Centros de ski | Cerro Castor |
| Sector inmobiliario y de la construcción | Champ Frère |
| Textil / Hogar | Miremos para Adentro · Media Naranja · Grupo Fibransur |
| Cannabis, educación y ONG | Expo Cannabis Argentina (3 ediciones) · CECCa · Clon Factory |

---

## Datos de contacto (en el CV)

- **Email:** baumaloneay@gmail.com
- **Teléfono:** 011 · 3191 · 1403
- **LinkedIn:** https://www.linkedin.com/in/bautista-maloneay-b5483721b/
- **CV web:** https://bm-gt.github.io/CV/

> Email y teléfono NO son links — abren un tooltip con botón "Copiar" para proteger scraping.

---

## Detalles técnicos importantes

### Bilingüismo
- Atributos `data-es` y `data-en` en cada elemento de texto
- `applyLang(l)` usa `innerHTML` (no `textContent`) para soportar `<br>` dentro de los atributos
- Toggle visible en nav como botón `ES` / `EN`

### Fondo estrellado
- `#starsCanvas` fixed, `z-index:0`, `opacity:.5`
- Las secciones deben tener fondos **transparentes o semi-transparentes** para que se vea
- `.cv-section.alt` usa `background: rgba(13,13,13,.55)` — NO sólido

### Scroll reveal
- Clase `.rv` + `IntersectionObserver` con `threshold: 0.07`

### Favicon
- SVG inline en `<link rel="icon">`: monograma **BM** rosa `#D63B7F` sobre fondo oscuro `#050505`

### Contadores hero
- `animCount('stat-exp', 9, 1800)` → +9 años
- `animCount('stat-brands', 40, 2400)` → +40 marcas

### Logos de empresas
- **WTF¿:** SVG inline, texto "WTF¿" con ¿ en rosa
- **CraveroLanis:** SVG inline, texto "Cravero / Lanis" sobre blanco
- **CECCa:** SVG inline, wordmark real — fondo blanco, "CECCa" negro bold, subtítulo teal `#1C8F6E`, `viewBox="0 0 128 64"`
- **Audi:** SVG inline, 4 círculos entrelazados sobre blanco

---

## PDFs (pendiente — a hacer en nueva sesión)

Los PDFs se generaron y luego se eliminaron del historial a pedido. Para regenerarlos:

```python
# Requiere: pip install playwright
# Chromium disponible en: /opt/pw-browsers/chromium-1194/chrome-linux/chrome
# Variable: PLAYWRIGHT_BROWSERS_PATH=/opt/pw-browsers

# Estrategia: renderizar el HTML real con Playwright
# 1. Abrir bautistamaloneay.html con file://
# 2. Clickear botón de idioma para entrar al sitio
# 3. Mostrar solo la tab deseada (cv o portfolio)
# 4. Exportar a PDF con print_background=True
```

Separar en:
- `CV_BautistaM_ES.pdf` — tabs CV + Contacto
- `CV_BautistaM_EN.pdf`
- `Portfolio_BautistaM_ES.pdf` — tab Portfolio + Contacto
- `Portfolio_BautistaM_EN.pdf`

---

## GitHub Pages

- Repo público: **obligatorio** para GitHub Pages gratuito
- Source: branch `claude/confident-ride-ve7zwf`, carpeta `/`
- URL final: https://bm-gt.github.io/CV/
- `index.html` redirige con `<meta http-equiv="refresh">` a `bautistamaloneay.html`
- Tiempo de propagación tras un push: **1-2 minutos**

---

## Workflow de trabajo establecido

1. Usuario pide cambios en este chat
2. Claude edita `bautistamaloneay.html`
3. Commit + push al branch `claude/confident-ride-ve7zwf`
4. En 1-2 min el link https://bm-gt.github.io/CV/ muestra la versión nueva
5. El link nunca cambia — siempre el mismo para compartir
