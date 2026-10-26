# Plan: Plantilla HTML común

## Objetivo

Crear una plantilla HTML estática de referencia en `docs/reference/base.html` que sirva como base visual y estructural para las páginas de Café Barrio.

## Alcance

La plantilla incluirá la configuración HTML5, Tailwind CSS v4 mediante CDN, navbar, `main` vacío y footer. No se crearán ni modificarán las páginas Inicio, Menú o Pedido, ni se añadirá un mecanismo para compartir markup.

## Pasos

1. Crear el archivo de referencia en `docs/reference/base.html` con idioma español, codificación y viewport.
2. Cargar Tailwind CSS v4 mediante CDN, sin CSS propio ni JavaScript.
3. Añadir una navbar responsive con la marca Café Barrio y enlaces a Menú y Pedido.
4. Añadir un elemento `main` vacío para el contenido específico de cada página.
5. Añadir un footer con enlace a Pedido y marcadores editables para dirección y horario.
6. Aplicar la guía visual de `DESIGN.md` y verificar semántica, enlaces y diseño responsive.

## Decisiones y límites

- La plantilla será una referencia estática; no se implementará una solución de inclusión o reutilización automática.
- Dirección y horario no están definidos en la documentación, por lo que se representarán con marcadores editables.
- Schema.org y el contenido propio de cada página quedan fuera de alcance.
