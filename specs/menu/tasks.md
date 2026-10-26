# Tareas: Menú

- [x] Crear `menu.html` copiando `docs/reference/base.html`, sin modificar la plantilla ni su carga de Tailwind, navbar o footer.
- [x] Ajustar el título del documento y añadir un único H1 «Menú» dentro de `main#contenido-principal`, conservando el enlace de salto al contenido.
- [x] Añadir las opciones visuales Café, Té y Comida como elementos estáticos, sin interacción ni selección activa.
- [x] Crear las tres secciones con encabezados H2 y cuadrículas `grid-cols-1 sm:grid-cols-2 lg:grid-cols-4`.
- [x] Incorporar al menos 8 productos en total, con productos en cada categoría, imagen placeholder, texto alternativo adecuado, nombre y precio con moneda.
- [x] Aplicar a contenido y tarjetas los colores, tipografías, contenedor, espaciados y bordes definidos en `DESIGN.md`.
- [x] Añadir microdata `MenuItem` y `Offer` a cada producto, con nombre, precio y moneda coherentes con la información visible.
- [x] Revisar HTML semántico, jerarquía de encabezados y ausencia de CSS adicional o JavaScript propio.
- [ ] Comprobar en navegador la navegación por teclado, el foco visible y el salto al contenido; verificar que los filtros no introducen interacción.
- [ ] Revisar en navegador móvil y escritorio: cuadrícula de una, dos y cuatro columnas, imágenes y textos sin solapamientos ni desbordamiento horizontal.
- [ ] Comprobar los enlaces a `index.html`, `menu.html` y `order.html`; registrar como pendiente la navegación a páginas que todavía no existan.

## Validación realizada y pendientes

- La comprobación estructural del HTML confirma las partes compartidas de la plantilla, las tres categorías, los ocho productos y la coherencia de precios y microdata. El editor no detecta errores en `menu.html`.
- Las clases responsive están revisadas en el código; la presentación real, la carga de imágenes y el teclado no se han podido verificar. Chromium headless no arranca porque falta `libatk-1.0.so.0` en el entorno.
- Los destinos de los enlaces coinciden con la plantilla. `menu.html` existe; la navegación completa a Inicio y Pedido queda pendiente porque `index.html` y `order.html` todavía no existen.