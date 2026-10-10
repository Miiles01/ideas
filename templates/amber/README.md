# Plantilla Amber

Estructura rescatada de amber-template.webflow.io, en HTML/CSS/JS plano (sin build).

## Secciones (de arriba abajo)
1. **Hero**: imagen a pantalla completa + overlay, nav en 3 columnas, titular que sube por líneas, botón glass y wordmark gigante en marquee.
2. **Intro**: párrafo serif grande que se "llena" con el scroll + lista de valores (etiqueta | texto).
3. **Imagen a todo el ancho**: titular, numeral y miniatura inset.
4. **Split 2:3**: texto + imagen vertical, dos bloques alternados.
5. **Menú**: título XL en dos líneas, tabs en píldora y lista de platos.
6. **Valores**: lista etiqueta | frase grande.
7. **Footer oscuro**: columnas de enlaces, CTA y wordmark en marquee.

## Personalizar
- Colores, fuentes y tamaños: variables en `:root` de `styles.css`.
- Imágenes: `<div data-img="x" data-src="img/foto.webp">` (sin `data-src` queda un degradado).
- Fuentes: Amber usa Bdogrotesk (de pago); aquí se usa Hanken Grotesk + Belleza (Google Fonts).
