# AI Context & Component Index

Este repositorio actúa como una **biblioteca de referencias de diseño y código (UI/UX)**. Su propósito es ser consumido por modelos de Inteligencia Artificial (IAs) para mantener un estándar de diseño visual y de código consistente en todos los proyectos futuros.

## Estructura del Repositorio

- `/components/`: Fragmentos de código, componentes UI individuales (botones, tarjetas, secciones, etc.) listos para implementarse.
- `/templates/`: Plantillas completas de sitios web y secciones enteras.
- `/assets/`: Imágenes, videos o archivos multimedia que sirven de referencia visual.
- `DESIGN_RULES.md`: Las reglas principales que se deben respetar en cualquier diseño (ej. nada de mayúsculas fijas, uso de Smooth Scroll, etc.).

## Índice de Componentes (AI Index)

Este índice está diseñado para que una IA localice rápidamente el código adecuado para la necesidad del proyecto. Se actualizará cada vez que se agregue una nueva referencia.

### 🧩 Moléculas (Componentes Simples)
*(Ej: Botones, Loaders, Inputs, Badges. Vacío por ahora)*

### 🏗️ Organismos (Componentes Complejos)
- **Menú MOSS (Sidebar animado)**: [`components/menu-moss-demo.html`](components/menu-moss-demo.html)
  - **Descripción**: Un menú lateral completo estilo MOSS. Animaciones suaves `cubic-bezier`, overlay oscuro y botón hamburguesa circular fijo. Tipografía Manrope.
  - **Tags**: Sidebar, Menu, Vanilla JS, CSS Animations.
- **Texto 3D en perspectiva con scroll**: [`components/texto-3d-perspectiva-scroll.html`](components/texto-3d-perspectiva-scroll.html)
  - **Descripción**: Sección fija a pantalla completa con un párrafo grande centrado. Al hacer scroll cada línea gira sobre su eje Y como la cara de un cubo y el siguiente párrafo entra girando, escalonado línea por línea (efecto 053 de Made With GSAP). Venía del home de Miiles ("Unifica tus ideas en un solo lugar"). Solo escritorio; en móvil y con movimiento reducido queda el primer párrafo estático. Manrope.
  - **Tags**: Scroll, 3D, GSAP, ScrollTrigger, SplitText, Pin, Landing, Vanilla JS.
- **Texto sobre curva con scroll**: [`components/texto-curvo-scroll.html`](components/texto-curvo-scroll.html)
  - **Descripción**: Sección fija muy alta con un SVG gigante y una curva ondulada. Al hacer scroll la frase se escribe letra por letra sobre la curva (textPath) y la cámara (viewBox) sigue la punta del texto con un quickTo suave (efecto 059 de Made With GSAP). Venía del home de Miiles ("Es horaaaaaa de crearrrrrrrrr"). Solo escritorio; en móvil y con movimiento reducido se muestra la frase como título estático. Manrope.
  - **Tags**: Scroll, SVG, textPath, GSAP, ScrollTrigger, Pin, Landing, Cierre, Vanilla JS.

### 📄 Plantillas (Templates & Pages)
- **Amber (landing editorial con scroll animado)**: [`templates/amber/`](templates/amber/index.html)
  - **Descripción**: Landing completa inspirada en amber-template.webflow.io. Hero con wordmark gigante en marquee, párrafos que se encienden con el scroll, imágenes a todo el ancho con parallax, splits 2:3, menú con tabs y footer oscuro. Preloader, smooth scroll (Lenis), animaciones de entrada de texto, menú móvil a pantalla completa. Paleta crema `#faf6f0` / `#282828` / `#93876e`, Belleza + Hanken Grotesk. HTML/CSS/JS Vanilla (GSAP + ScrollTrigger + Lenis por CDN). Tokens en `:root` de `styles.css`; más detalle en su `README.md`.
  - **Tags**: Landing, Editorial, Parallax, Smooth Scroll, GSAP, Mobile-first, Restaurante.

## 🎬 Skills de Animación (obligatorio al diseñar sitios web)

Toda transición o microinteracción debe hacerse con la skill **transitions.dev**. Incluye 32 transiciones CSS listas para usar (botones, dropdowns, modales, toasts, tabs, tooltips, acordeones, toggles, loaders, estados de "pensando" de IA, etc.), todas con soporte para `prefers-reduced-motion`.

- **Repositorio**: [Jakubantalik/transitions.dev](https://github.com/Jakubantalik/transitions.dev)
- **Instalación**:
  - Skill principal: `npx skills add Jakubantalik/transitions.dev`
  - Complemento de pulido: `npx skills add Jakubantalik/transitions.dev -s transitions-polish`
- **Cuándo usar cada una**:
  - `transitions-dev`: para **agregar** transiciones nuevas.
  - `transitions-polish`: para **ajustar** animaciones que ya existen (duración, distancia, escala, blur y *easing*) a la escala de tokens.
- **Prompts útiles**:
  - "Update dropdowns transition based on transitions-dev skill"
  - "Update all icon swap transitions based on transitions-dev skill"
  - "Update all modals transitions based on transitions-dev skill"
- **Referencia visual**: [Amicro](https://amicro.vercel.app) ([código en GitHub](https://github.com/Subhan-code/Amicro--Micro-transitions-), licencia MIT): botones, más de 130 loaders y efectos de texto, hover, cursor y scroll, hechos en React y basados en transitions.dev. Se pueden agregar a un proyecto con `npx @subhanhq/amicro add`, pero recuerda convertirlos a HTML/CSS/JS Vanilla según `DESIGN_RULES.md`.

---
**Instrucción para IAs:** Al generar código para un nuevo proyecto, SIEMPRE consulta `DESIGN_RULES.md` y revisa este `INDEX.md` para extraer y reutilizar los componentes aprobados que se encuentran en este repositorio.
