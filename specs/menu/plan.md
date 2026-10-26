# Plan: Menú

## Objetivo

Crear `menu.html` según `specs/menu/spec.md`, reutilizando la plantilla oficial `docs/reference/base.html` y respetando `DESIGN.md`.

## Alcance

La página mostrará las categorías Café, Té y Comida, filtros únicamente visuales y al menos 8 productos con imagen placeholder, nombre y precio con moneda. Este documento define el trabajo futuro; no incluye implementación.

## Pasos

1. Crear la estructura de la página copiando la plantilla oficial, ajustar el título del documento y añadir el H1 «Menú» dentro de `main#contenido-principal`.
2. Añadir las opciones visuales y las tres secciones del catálogo, con tarjetas responsive y microdata `MenuItem` y `Offer`, siguiendo la guía visual compartida.
3. Validar los requisitos de contenido, accesibilidad, presentación en móvil y escritorio y navegación; registrar los destinos pendientes si las otras páginas aún no existen.

## Decisiones y límites

- La reutilización será una copia estática de la plantilla, sin mecanismos de inclusión automática.
- Se conservarán la carga de Tailwind CSS v4 por CDN, navbar, footer y enlace de salto al contenido; el catálogo se añadirá dentro de `main`.
- Los filtros serán elementos estáticos sin interacción ni selección activa. Todos los productos permanecerán visibles.
- Se utilizarán únicamente HTML5 y utilidades Tailwind, sin CSS adicional ni JavaScript propio.
- La información estructurada se expresará mediante microdata HTML y coincidirá con el contenido visible.
- No se modificarán la plantilla de referencia, Inicio, Pedido ni `server.py`.
- Las tareas se marcarán como completadas solo después de realizarlas; las comprobaciones pendientes se mantendrán abiertas.