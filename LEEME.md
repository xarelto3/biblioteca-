# Biblioteca flipbook (Jean José)

Visor de ebooks con efecto de pasar página. Sin publicidad, sin límite de libros, gratis.

## Agregar un libro
1. Pon el PDF en la carpeta `libros/` (ej: `libros/la-moneda-invisible.pdf`).
2. Abre `books.json` y copia un bloque dentro de `"books"`:
   - `id`: nombre corto sin espacios (va en el link: tusitio.com/#la-moneda-invisible)
   - `title`, `tagline`: título y frase gancho
   - `pdf`: ruta del PDF
   - `sample`: cuántas páginas se leen gratis (borra esta línea para mostrar el libro completo)
   - `buyUrl`: link de pago (Mercado Pago, etc.)
   - `accent`: color del libro (ej: "#c0392b")
3. La portada se toma sola de la página 1 del PDF.

## Publicar gratis
- Vercel: sube esta carpeta como proyecto (framework "Other"). Listo.
- O GitHub Pages / Netlify Drop (arrastras la carpeta).
- No abre con doble clic en el computador (necesita un servidor): para probar local usa `python3 -m http.server`.

## Tip de venta
Con `sample` solo se cargan esas páginas, pero el PDF viaja completo al navegador.
Para vender de verdad, sube a `libros/` una versión recortada (solo las páginas de muestra)
y entrega el PDF completo por correo después del pago.
