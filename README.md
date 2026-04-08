# 🚗 Mercedes-Benz — Landing Page

<div align="center">

![Estado](https://img.shields.io/badge/estado-en%20desarrollo-yellow?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![Sin JS](https://img.shields.io/badge/JavaScript-sin%20uso-lightgrey?style=for-the-badge&logo=javascript)
![Licencia](https://img.shields.io/badge/licencia-MIT-green?style=for-the-badge)
![Rock The Code](https://img.shields.io/badge/práctica-Rock%7BTheCode%7D-black?style=for-the-badge)

<br/>

> **Práctica frontend** perteneciente al programa formativo **Rock{TheCode} — Desarrollo Web V2** de **ThePower**.
> Maquetación completa de una landing page inspirada en Mercedes-Benz a partir de un diseño Figma,
> construida **únicamente con HTML semántico y CSS puro** — sin una sola línea de JavaScript.

<br/>

> **Frontend practice** from the **Rock{TheCode} — Web Development V2** program at **ThePower**.
> Full landing page layout inspired by Mercedes-Benz based on a Figma design,
> built **exclusively with semantic HTML and pure CSS** — zero JavaScript.

</div>

---

## 📋 Índice / Table of Contents

- [Vista previa / Preview](#️-vista-previa--preview)
- [Descripción / Description](#-descripción--description)
- [Características / Features](#-características--features)
- [Tecnologías / Technologies](#️-tecnologías--technologies)
- [Estructura del proyecto / Project Structure](#-estructura-del-proyecto--project-structure)
- [Instalación y uso / Installation & Usage](#-instalación-y-uso--installation--usage)
- [Decisiones técnicas / Technical Decisions](#-decisiones-técnicas--technical-decisions)
- [Errores conocidos / Known Issues](#-errores-conocidos--known-issues)
- [Mejoras futuras / Future Improvements](#-mejoras-futuras--future-improvements)
- [Contribución / Contributing](#-contribución--contributing)
- [Licencia / License](#-licencia--license)
- [Transparencia de IA / AI Transparency](#-transparencia-de-ia--ai-transparency)

---

## 🖥️ Vista previa / Preview

<div align="center">

| Desktop | Mobile |
|:---:|:---:|
| ![Desktop preview](https://i.postimg.cc/C5VdV5bQ/Web_Mecedes.png) | ![Mobile preview](https://i.postimg.cc/QCrVrCcT/Movail_web_Mercedez.png) |

> ⚠️ **Nota:** Sustituir estas imágenes de placeholder por capturas reales del proyecto antes de publicar.
> ⚠️ **Note:** Replace these placeholder images with real screenshots before publishing.

</div>

---

## 📖 Descripción / Description

### 🇪🇸 Español

Este proyecto es una **landing page inspirada en Mercedes-Benz** desarrollada como práctica del programa formativo **Rock{TheCode} — Desarrollo Web V2** de **ThePower**. El objetivo principal es trasladar fielmente un diseño de Figma a código real, aplicando buenas prácticas de maquetación moderna.

El reto principal fue **construir una página completamente interactiva y responsive sin utilizar JavaScript**, usando únicamente técnicas CSS avanzadas como el truco del checkbox para el menú hamburguesa, `scroll-snap` para el carrusel horizontal, y Flexbox + Grid para los layouts.

### 🇬🇧 English

This project is a **Mercedes-Benz–inspired landing page** developed as a practice exercise for the **Rock{TheCode} — Web Development V2** program at **ThePower**. The main goal is to faithfully translate a Figma design into real code, applying modern layout best practices.

The main challenge was **building a fully interactive and responsive page without using JavaScript**, relying solely on advanced CSS techniques such as the checkbox trick for the hamburger menu, `scroll-snap` for the horizontal carousel, and Flexbox + Grid for layouts.

---

## ✨ Características / Features

| Característica / Feature | Descripción / Description |
|---|---|
| 📱 **Responsive — Mobile First** | Diseño adaptado a móvil, tablet y desktop con una sola media query / Layout adapted for mobile, tablet, and desktop with a single breakpoint |
| 🍔 **Menú hamburguesa sin JS** | Funcional mediante el truco CSS del checkbox / Functional via the CSS checkbox trick |
| 🎨 **Variables CSS / CSS Custom Properties** | Sistema de diseño consistente definido en `:root` / Consistent design system defined in `:root` |
| ♿ **Accesibilidad / Accessibility** | Atributos ARIA, roles semánticos y clase `.sr-only` / ARIA attributes, semantic roles, and `.sr-only` class |
| 🔍 **SEO básico / Basic SEO** | Meta etiquetas, `fetchpriority="high"` en hero, `loading="lazy"` en el resto / Meta tags, `fetchpriority="high"` on hero, `loading="lazy"` on the rest |
| 📜 **HTML semántico / Semantic HTML** | Uso correcto de `header`, `main`, `section`, `nav`, `footer` / Correct use of semantic elements |
| 🖱️ **Carrusel sin JS / JS-free Carousel** | Scroll horizontal nativo con `scroll-snap-type` / Native horizontal scroll with `scroll-snap-type` |
| 🎠 **Tarjetas de producto / Product Cards** | Grid de 4 tarjetas con colores y botones interactivos / Grid of 4 cards with color swatches and interactive buttons |
| 🗺️ **Sección Dealer** | Tarjeta superpuesta con `backdrop-filter: blur` sobre imagen de mapa / Overlaid card with `backdrop-filter: blur` on map image |
| 🖤 **Sección Maybach** | Hero dividido + layout split texto/imagen / Split hero + text/image split layout |
| 📧 **Footer completo / Full Footer** | CTA banner + formulario newsletter + links + redes sociales + botón scroll-to-top / CTA banner + newsletter form + links + social icons + scroll-to-top button |

---

## 🛠️ Tecnologías / Technologies

```
HTML5        ──── Estructura semántica y accesible / Semantic and accessible structure
CSS3         ──── Flexbox, Grid, Custom Properties, Media Queries, scroll-snap
Google Fonts ──── Roboto (pesos 300, 400, 500, 700) / weights 300, 400, 500, 700
Figma        ──── Diseño de referencia (solo consulta) / Reference design (consultation only)
```

> **Sin frameworks. Sin librerías. Sin JavaScript. / No frameworks. No libraries. No JavaScript.**

---

## 📁 Estructura del proyecto / Project Structure

```
mercedes-benz-landing/
│
├── index.html      ← Estructura HTML completa con 7 secciones / Full HTML with 7 sections
├── style.css       ← Estilos globales, Mobile First + 1 breakpoint desktop / Global styles, Mobile First + 1 desktop breakpoint
└── README.md       ← Documentación del proyecto / Project documentation
```

### Secciones de la página / Page Sections

```
┌──────────────────────────────────┐
│             HEADER               │  Nav sticky + menú hamburguesa CSS (checkbox trick)
├──────────────────────────────────┤
│              HERO                │  Imagen full-width + overlay gradiente + texto
├──────────────────────────────────┤
│            PRODUCTS              │  Grid 1→2 col · 4 tarjetas · selector de colores
├──────────────────────────────────┤
│             DEALER               │  Texto + mapa oscuro + tarjeta con backdrop-filter
├──────────────────────────────────┤
│            FEATURES              │  Carrusel horizontal · scroll-snap · 3 tarjetas
├──────────────────────────────────┤
│            MAYBACH               │  Hero imagen · layout split texto/imagen
├──────────────────────────────────┤
│             FOOTER               │  CTA banner · newsletter · links · redes · top btn
└──────────────────────────────────┘
```

### Arquitectura CSS

```
style.css
│
├── :root              → Variables globales (colores, tipografía, espaciado, radios)
├── Reset              → * { margin: 0; padding: 0; box-sizing: border-box; }
├── Accesibilidad      → .sr-only
├── Checkbox trick     → .nav-toggle (oculto) + selector ~ para abrir sidebar
│
├── Mobile First (base)
│   ├── header / nav (sidebar)
│   ├── hero
│   ├── products / cards
│   ├── dealer
│   ├── features (carrusel)
│   ├── maybach
│   └── footer (cta + main)
│
└── @media (min-width: 769px)
    └── Overrides para desktop de todas las secciones anteriores
```

---

## 🚀 Instalación y uso / Installation & Usage

### 🇪🇸 Este proyecto no tiene dependencias ni proceso de build. Solo necesitas un navegador.

### 🇬🇧 This project has no dependencies or build process. You only need a browser.

---

### Opción 1 / Option 1 — Abrir directamente / Open directly

```bash
# Clona el repositorio / Clone the repository
git clone https://github.com/tu-usuario/mercedes-benz-landing.git

# Entra en la carpeta / Enter the folder
cd mercedes-benz-landing

# Abre index.html en tu navegador / Open index.html in your browser
# macOS
open index.html
# Windows
start index.html
# Linux
xdg-open index.html
```

### Opción 2 / Option 2 — Servidor local recomendado / Recommended local server

```bash
# ── VS Code + Live Server (recomendado / recommended) ──────────────────────
# Clic derecho en index.html → "Open with Live Server"
# Right-click index.html → "Open with Live Server"

# ── Python ─────────────────────────────────────────────────────────────────
python -m http.server 3000
# Abre / Open: http://localhost:3000

# ── Node.js ────────────────────────────────────────────────────────────────
npx serve .
# Abre / Open: http://localhost:3000
```

> 💡 **Tip:** Se recomienda un servidor local para evitar restricciones CORS en imágenes externas.
> 💡 **Tip:** A local server is recommended to avoid CORS restrictions with external images.

---

## 💡 Decisiones técnicas / Technical Decisions

### 1. Menú hamburguesa sin JavaScript / Hamburger Menu without JavaScript

El menú lateral se controla mediante un `<input type="checkbox">` oculto. El `<label>` actúa como disparador, y el selector CSS `~` (sibling) permite reaccionar al estado `:checked` desde el CSS.

The sidebar menu is controlled via a hidden `<input type="checkbox">`. The `<label>` acts as trigger, and the CSS `~` (sibling) selector reacts to the `:checked` state.

```html
<!-- Checkbox oculto / Hidden checkbox -->
<input type="checkbox" id="nav-toggle" class="nav-toggle" aria-hidden="true">

<!-- Botón hamburguesa (label vinculado) / Hamburger button (linked label) -->
<label for="nav-toggle" class="nav-hamburger">☰</label>

<!-- Overlay que también cierra el menú / Overlay that also closes the menu -->
<label for="nav-toggle" class="sidebar-overlay"></label>
```

```css
/* Sidebar cerrada por defecto / Sidebar closed by default */
#nav-menu {
    transform: translateX(100%);
    transition: transform 0.3s ease;
}

/* Se abre al marcar el checkbox / Opens when checkbox is checked */
.nav-toggle:checked ~ header #nav-menu {
    transform: translateX(0);
}

/* Overlay visible al abrir / Overlay visible when open */
.nav-toggle:checked ~ .sidebar-overlay {
    display: block;
}
```

---

### 2. Estrategia Mobile First

Los estilos base están escritos para móvil. Un único breakpoint `@media (min-width: 769px)` adapta el layout a desktop, siguiendo la filosofía de **mejora progresiva**.

Base styles are written for mobile. A single `@media (min-width: 769px)` breakpoint adapts the layout to desktop, following **progressive enhancement**.

```css
/* Móvil (base) / Mobile (base) */
.products__grid {
    grid-template-columns: 1fr;
    gap: 16px;
}

/* Desktop / Desktop */
@media (min-width: 769px) {
    .products__grid {
        grid-template-columns: 1fr 1fr;
        gap: 24px;
    }
}
```

---

### 3. Carrusel horizontal nativo / Native Horizontal Carousel

Sin librerías externas. El scroll horizontal se logra con `overflow-x: auto` y `scroll-snap-type`, obteniendo un comportamiento de carrusel fluido y accesible.

No external libraries. Horizontal scroll is achieved with `overflow-x: auto` and `scroll-snap-type`, providing a smooth, accessible carousel behavior.

```css
.features__track {
    display: flex;
    overflow-x: auto;
    scroll-snap-type: x mandatory;
    -webkit-overflow-scrolling: touch; /* iOS momentum scroll */
    scrollbar-width: thin;            /* Scrollbar sutil / Subtle scrollbar */
}

.feature-card {
    flex: 0 0 80vw;          /* Móvil: 80% del viewport */
    scroll-snap-align: start;
}

@media (min-width: 769px) {
    .feature-card {
        flex: 0 0 300px;     /* Desktop: ancho fijo / Fixed width */
    }
}
```

---

### 4. Sistema de diseño con Variables CSS / Design System with CSS Variables

Todas las decisiones visuales están centralizadas en `:root`, facilitando el mantenimiento y la consistencia.

All visual decisions are centralized in `:root`, making maintenance and consistency easier.

```css
:root {
    /* Colores / Colors */
    --primary-color:   #000000;
    --secondary-color: #ffffff;
    --accent-color:    #cccccc;
    --text-color:      #333333;

    /* Tipografía / Typography */
    --font-family: 'Roboto', sans-serif;
    --font-serif:  Georgia, 'Times New Roman', serif;

    /* Layout */
    --header-height:          64px;
    --sidebar-width:          280px;
    --section-padding-mobile: 24px 16px;
    --section-padding-desktop: 40px 32px;

    /* UI */
    --radius-card: 12px;
    --radius-pill: 20px;
    --transition:  0.3s ease;
}
```

---

### 5. Accesibilidad / Accessibility

```html
<!-- Texto oculto visualmente para lectores de pantalla / Visually hidden text for screen readers -->
<label for="newsletter-email" class="sr-only">Tu dirección de email</label>

<!-- Iconos SVG decorativos marcados como ocultos / Decorative SVGs marked as hidden -->
<svg aria-hidden="true">...</svg>

<!-- Navegación con label descriptivo / Navigation with descriptive label -->
<nav aria-label="Navegación principal">

<!-- Colores con etiquetas de texto / Color swatches with text labels -->
<span class="card__color" aria-label="Plata"></span>
```

```css
/* Clase .sr-only — estándar de la industria / Industry-standard .sr-only class */
.sr-only {
    position: absolute;
    width: 1px;
    height: 1px;
    padding: 0;
    margin: -1px;
    overflow: hidden;
    clip: rect(0, 0, 0, 0);
    white-space: nowrap;
    border-width: 0;
}
```

---

## 🐛 Errores conocidos / Known Issues

| # | Descripción / Description | Impacto / Impact | Prioridad / Priority |
|---|---|---|---|
| 1 | **Typo en nombres de modelos** — "Merces" en lugar de "Mercedes" en las 4 tarjetas de producto | Visual, profesional | 🔴 Alta |
| 2 | **Footer — texto de marca incorrecto** — El checkbox de newsletter dice "Velaretti" (otra marca) en vez de Mercedes-Benz | Confusión de marca | 🔴 Alta |
| 3 | **Footer — categorías incorrectas** — Los links del footer ("Electric bikes", "Kids' bikes") corresponden a otra landing page, no a Mercedes | Contenido erróneo | 🔴 Alta |
| 4 | **Hero — imagen incorrecta** — La imagen referenciada muestra un Mercedes-AMG C63, no el CLS mencionado en el título | Incoherencia de contenido | 🟡 Media |
| 5 | **Imágenes externas** — Todas las imágenes son URLs externas; podrían dejar de funcionar en el futuro | Fragilidad del proyecto | 🟡 Media |
| 6 | **`<title>` básico** — El `<title>` del documento solo dice "Mercedes-Benz", podría ser más descriptivo para SEO | SEO menor | 🟢 Baja |

> 💡 **Consejo de mentor:** Los errores #1, #2 y #3 son los más importantes de corregir antes de presentar el proyecto. Afectan directamente a la percepción de calidad y atención al detalle.

---

## 🔭 Mejoras futuras / Future Improvements

Estas mejoras son **opcionales** y van más allá del alcance de la práctica, pero son buenas ideas para seguir aprendiendo:

These improvements are **optional** and go beyond the scope of the exercise, but are great ideas for continued learning:

- [ ] **Imágenes locales** — Descargar y servir las imágenes desde el propio repositorio para mayor estabilidad
- [ ] **Favicon** — Añadir un favicon con el logo de Mercedes
- [ ] **`<title>` SEO** — Mejorar a: `"Mercedes-Benz | Descubre nuestros modelos eléctricos y Maybach"`
- [ ] **Open Graph** — Meta tags para compartir en redes sociales (`og:title`, `og:image`, etc.)
- [ ] **Animaciones de entrada** — Usar `@keyframes` o `animation` para animar secciones al hacer scroll (CSS puro)
- [ ] **Tema oscuro** — Implementar con `@media (prefers-color-scheme: dark)` y las variables CSS ya definidas
- [ ] **Focus visible** — Añadir estilos `:focus-visible` para mejorar la navegación por teclado

---

## 🤝 Contribución / Contributing

Este proyecto es una práctica educativa de **Rock{TheCode} — ThePower**, pero las sugerencias son bienvenidas.

This is an educational practice project for **Rock{TheCode} — ThePower**, but suggestions are welcome.

```bash
# 1. Haz un fork del repositorio / Fork the repository
# 2. Crea una rama / Create a branch
git checkout -b mejora/nombre-de-la-mejora

# 3. Haz tus cambios y commit / Make changes and commit
git commit -m "Añade: descripción del cambio / Add: description of change"

# 4. Sube los cambios / Push changes
git push origin mejora/nombre-de-la-mejora

# 5. Abre un Pull Request / Open a Pull Request
```

---

## 📄 Licencia / License

Este proyecto está bajo la licencia **MIT**.

This project is under the **MIT** license.

```
MIT License — puedes usar, copiar, modificar y distribuir este código
siempre que mantengas el aviso de copyright original.

MIT License — you may use, copy, modify, and distribute this code
as long as you keep the original copyright notice.
```

---

## 🤖 Transparencia de IA / AI Transparency

> Este README fue **analizado y mejorado con asistencia de Inteligencia Artificial** (Claude by Anthropic).
> This README was **analyzed and improved with Artificial Intelligence assistance** (Claude by Anthropic).

### Base del análisis / Basis of the analysis

| Fuente / Source | Qué se extrajo / What was extracted |
|---|---|
| `index.html` | Estructura de secciones, semántica, atributos ARIA, técnicas CSS aplicadas, errores de contenido |
| `style.css` | Sistema de variables, estrategia Mobile First, breakpoints, técnicas avanzadas (checkbox, scroll-snap, backdrop-filter) |
| `README.md` original | Información declarada por el autor, punto de partida para mejoras |

### Nivel de certeza / Confidence level

| Afirmación / Statement | Certeza / Confidence |
|---|---|
| Tecnologías usadas (HTML5, CSS3, Google Fonts) | 🟢 Alta — evidente en el código |
| Estrategia Mobile First | 🟢 Alta — confirmada en el CSS |
| Truco del checkbox para el menú | 🟢 Alta — código explícito |
| Diseño basado en Figma | 🟡 Media — declarado en el README original, no verificable sin acceso al Figma |
| Errores de contenido detectados | 🟢 Alta — extraídos directamente del HTML |
| Audiencia (evaluadores del máster) | 🟡 Media — informado por el autor |

### Qué es inferencia vs. evidencia / What is inference vs. evidence

- ✅ **Evidencia directa:** estructura de secciones, clases CSS, atributos HTML, variables, breakpoints
- 🔍 **Inferencia:** propósito educativo, referencia al diseño Figma, audiencia del proyecto
- ✏️ **Aportación de la IA:** sección de errores conocidos, mejoras futuras, diagramas ASCII, versión bilingüe

---

<div align="center">

Desarrollado con 🖤 como práctica de **Rock{TheCode} — Desarrollo Web V2 · ThePower**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![Rock The Code](https://img.shields.io/badge/Rock%7BTheCode%7D-ThePower-black?style=flat-square)

</div>
