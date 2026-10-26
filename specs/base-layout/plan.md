# Plan: plantilla base

Crear `docs/reference/base.html` como plantilla común para Inicio, Menú y Pedido, siguiendo [la especificación](spec.md), `CONTEXT.md` y `DESIGN.md`.

## Pasos

1. Crear `docs/reference/` si no existe y preparar un documento HTML5 en español con metadatos básicos y Tailwind CSS v4 por CDN.
2. Añadir una navbar semántica con la identidad del café y enlaces a `index.html`, `menu.html` y `order.html`.
3. Dejar un `main` semántico vacío y añadir un footer con dirección, horario y enlace a Pedido. No inventar datos que no estén definidos.
4. Aplicar utilidades Tailwind de acuerdo con `DESIGN.md`, sin JavaScript propio ni CSS adicional.
5. Revisar semántica, accesibilidad, enlaces y presentación responsive en móvil y escritorio.

## Límites

- No implementar contenido particular de las páginas, filtros ni procesamiento de pedidos.
- No añadir dependencias o tecnologías fuera de las establecidas en `CONTEXT.md`.

## Verificación

- Confirmar que la plantilla contiene navbar, `main` vacío y footer, y que los enlaces apuntan a los archivos correctos.
- Comprobar visualmente la consistencia con `DESIGN.md` en móvil y escritorio.