# Especificación: Página de Inicio

## Objetivo

Definir los requisitos de `index.html`, la página de Inicio de Café Barrio, para presentar la cafetería y destacar dos productos.

## Alcance

La página debe partir de `docs/reference/base.html`. El contenido específico de Inicio se añadirá únicamente dentro de `main`; la navbar, el footer y la configuración compartida de Tailwind no deben modificarse.

## Requisitos

- Mostrar una sección hero con un mensaje de bienvenida y un enlace visible al menú (`menu.html`).
- Mostrar exactamente dos productos destacados. Cada uno debe incluir nombre, descripción y precio.
- Incluir datos estructurados Schema.org para la cafetería (`CafeOrCoffeeShop`) y para los productos destacados (`MenuItem`), con datos coherentes con el contenido visible.
- Mantener el diseño mobile-first, semántico y accesible.
- Seguir `DESIGN.md`: estilo minimalista y cálido, colores definidos, títulos en Georgia, texto en Arial, contenedor central y espaciado establecido.
- Mantener sin cambios el navbar y el footer de la plantilla de referencia, incluida la navegación a Menú y Pedido.
- Usar únicamente HTML5 y Tailwind CSS v4 por CDN; no añadir JavaScript propio, CSS adicional, backend ni procesamiento de pedidos.

## Fuera de alcance

- El catálogo completo, las categorías y los filtros de la página Menú.
- El formulario de pedidos y su procesamiento.
- Cambios a `docs/reference/base.html`, a la navbar o al footer compartidos.
- Interacciones o funcionalidades no descritas en esta especificación.

## Criterios de aceptación

- Existe `index.html` y conserva la estructura común de `docs/reference/base.html`.
- El contenido específico de Inicio está dentro de `main` e incluye el hero con bienvenida y enlace funcional a `menu.html`.
- Se muestran dos productos destacados; cada uno tiene nombre, descripción y precio.
- Los datos estructurados representan la cafetería y los dos productos de forma coherente con el contenido visible.
- La página mantiene los estilos, la semántica, la accesibilidad y el comportamiento responsive establecidos por el proyecto.
- No se modifican los componentes compartidos ni se introducen tecnologías fuera de los límites del proyecto.
