# Reglas Principales de Diseño

1. **Aplicación de Habilidades de UI/UX**: Aplica siempre los principios y directrices de la guía de UI/UX enviada (disponible en: [ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill)). Considérala siempre para el diseño y construcción de interfaces.
2. **Uso de Smooth Scroll**: Implementa *smooth scroll* (usando ScrollSmoother de GSAP) **únicamente** en landing pages y sitios de e-commerce de productos. **No lo apliques en dashboards**, paneles administrativos, páginas de login ni módulos de gestión, ya que puede afectar su comportamiento.
3. **Uso de Plantillas**: Utiliza las plantillas disponibles en la carpeta «Plantillas Web» (ubicada en tus documentos). Dado que vienen en Next.js, **conviértelas a un código más ligero e independiente (HTML, CSS y JavaScript Vanilla)**, ideal para desplegar en Hostinger bajo la modalidad de sitio web Custom PHP/HTML.
4. **Uso de Mayúsculas**: **Evita el uso de textos en mayúsculas fijas** (por ejemplo: HOLA, MENÚ, ACERCA DE). Utiliza una tipografía con mayúsculas y minúsculas adecuadas (Sentence case o Title case).
5. **Uso Moderado de Divisores**: No abuses de los elementos divisores (dividers). Respeta los que ya vienen en las plantillas y agrega nuevos únicamente cuando sean estrictamente necesarios. Preferir el uso de espacios en blanco (`padding`, `margin`, `gap`).
6. **Flujo de Despliegue en Hostinger**: Organiza el trabajo pensando en el despliegue final en Hostinger. Envía el código al repositorio de GitHub proporcionado y **genera la rama `deploy`** para que Hostinger pueda sincronizar y mostrar el sitio sin inconvenientes.
7. **Diseño Responsivo**: Garantiza que la web se visualice correctamente en todos los dispositivos (escritorio, tablet y móvil), manteniendo siempre la calidad del diseño y la usabilidad.
8. **Visualización Local**: Siempre despliega un *localhost* para visualizar la página cuando se esté trabajando.
