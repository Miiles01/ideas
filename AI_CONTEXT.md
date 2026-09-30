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

### 📄 Plantillas (Templates & Pages)
*(Ej: Sitios completos, Landing Pages. Vacío por ahora)*

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
