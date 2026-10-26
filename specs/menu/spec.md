# Especificación: Menú

## Objetivo

Definir la página `menu.html` de Café Barrio para consultar la oferta de café, té y comida ligera, según los requisitos de `CONTEXT.md` y las reglas visuales de `DESIGN.md`.

## Alcance

La página debe partir de la plantilla oficial `docs/reference/base.html`. El contenido específico del menú se incorporará dentro de `main`, conservando su identificador `contenido-principal` y el enlace para saltar al contenido. No se modificará la plantilla de referencia ni se alterarán su carga de Tailwind, navbar o footer. Esta especificación no incluye implementación.

## Requisitos

### Estructura y contenido

- La página debe usar HTML5 semántico, idioma español, codificación UTF-8 y viewport para dispositivos móviles.
- Debe incluir un título de documento identificable como Menú de Café Barrio y un único H1, «Menú», dentro de `main`.
- Debe mostrar las tres categorías: Café, Té y Comida, con productos en cada una y encabezados H2 para identificarlas.
- Debe incluir un mínimo de 8 productos en total. Cada producto debe mostrar una imagen placeholder, un nombre y un precio con moneda explícita.
- Las imágenes deben tener texto alternativo adecuado, sin atribuir a una imagen genérica detalles del producto que no representa.
- Debe mostrar las opciones visuales Café, Té y Comida como filtros sin funcionamiento. Todos los productos permanecerán visibles; las opciones no filtrarán, navegarán ni simularán una selección activa.
- Los filtros deben representarse como elementos estáticos o controles deshabilitados con nombres comprensibles, sin ofrecer interacciones que no se puedan completar.
- Navbar y footer deben conservar el contenido, los enlaces y las clases de la plantilla oficial, manteniendo la consistencia entre Inicio, Menú y Pedido.

### Diseño y responsive

- Se debe respetar el estilo minimalista, cálido y acogedor de `DESIGN.md`, sin colores llamativos, efectos complejos ni animaciones.
- Colores: principal `#63452F`, fondo `#FAF7F2`, acento `#A6AD89`, texto `#30241D` y tarjetas blancas `#FFFFFF`.
- Tipografía: Georgia para títulos y Arial para texto. H1 con `text-4xl md:text-5xl`, H2 con `text-2xl md:text-3xl` y texto normal con `text-base`.
- El contenido debe usar el contenedor `max-w-6xl mx-auto px-4` y separación de secciones `py-12 md:py-16`.
- Los productos deben distribuirse en una cuadrícula mobile-first con `grid-cols-1 sm:grid-cols-2 lg:grid-cols-4`.
- Las tarjetas deben tener fondo blanco, esquinas `rounded-xl` y borde suave, siguiendo la guía compartida.
- Imágenes, textos y opciones visuales deben adaptarse al ancho disponible sin solapamientos ni desplazamiento horizontal.

### Accesibilidad y límites técnicos

- Se deben conservar los landmarks semánticos de la plantilla y una jerarquía de encabezados coherente.
- Los enlaces deben mantener nombres comprensibles, navegación por teclado e indicación de foco visible. Los filtros estáticos no deben introducir paradas de teclado innecesarias.
- Los productos deben incluir datos estructurados Schema.org de tipo `MenuItem`, con nombre y precio coherentes con el contenido visible. Se usará microdata HTML para respetar la ausencia de JavaScript propio.
- Solo se permite HTML5 y Tailwind CSS v4 mediante el CDN de la plantilla. No se añadirá CSS adicional, otra configuración de Tailwind, React ni JavaScript propio.

## Fuera de alcance

- Filtros funcionales, búsquedas, ordenación o actualización dinámica del catálogo.
- Carrito, selección de productos, procesamiento o almacenamiento de pedidos, backend y base de datos.
- Implementación o modificación de Inicio, Pedido, `docs/reference/base.html` o `server.py`.
- Estilos o componentes que se aparten de `DESIGN.md`.
- Implementación de código y creación de `plan.md` o `tasks.md` en esta entrega.

## Criterios de aceptación

- Existe `specs/menu/spec.md` y define `menu.html` como página que se construirá a partir de `docs/reference/base.html`, sin modificar la plantilla.
- La página prevista mantiene la navbar, el footer, la carga de Tailwind y el enlace de salto al contenido de la plantilla; el catálogo se ubica dentro de `main#contenido-principal`.
- Se muestran Café, Té y Comida, cada categoría con productos, y al menos 8 productos en total con imagen placeholder, nombre y precio con moneda.
- Las tres opciones de filtro son únicamente visuales: no cambian el catálogo, no activan navegación y todos los productos permanecen visibles.
- La presentación respeta los colores, tipografías, espaciados y tarjetas de `DESIGN.md`; la cuadrícula muestra una columna en móvil, dos desde `sm` y cuatro desde `lg`.
- En móvil y escritorio, el contenido se lee sin solapamientos ni desbordamiento horizontal.
- Se comprueba que la marca enlaza a `index.html`, Menú a `menu.html` y los enlaces de Pedido a `order.html`. La comprobación completa de navegación queda pendiente si esas páginas todavía no existen.
- La revisión de accesibilidad confirma el H1 único, las categorías con H2, los textos alternativos, el salto al contenido y el foco visible en los enlaces.
- Cada producto incorpora microdata `MenuItem` y su precio mediante una oferta con moneda, coincidentes con la información visible.
- La implementación futura utiliza solo HTML5 y Tailwind CSS v4 por CDN, sin CSS adicional ni JavaScript propio.
- Esta entrega añade únicamente la especificación, sin implementar la página ni modificar otros archivos.