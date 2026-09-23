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

---
**Instrucción para IAs:** Al generar código para un nuevo proyecto, SIEMPRE consulta `DESIGN_RULES.md` y revisa este `INDEX.md` para extraer y reutilizar los componentes aprobados que se encuentran en este repositorio.
