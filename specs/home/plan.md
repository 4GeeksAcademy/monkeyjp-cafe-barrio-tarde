# Plan: Página de Inicio

## Objetivo

Crear `index.html` a partir de `docs/reference/base.html`, añadiendo únicamente el contenido específico de Inicio dentro de `main` y conservando los componentes compartidos.

## Pasos

1. Copiar la plantilla base como `index.html`, manteniendo la configuración del documento, Tailwind, navbar y footer.
2. Añadir dentro de `main` un hero de bienvenida con un enlace a `menu.html`.
3. Añadir dos productos destacados, cada uno con nombre, descripción y precio.
4. Añadir datos Schema.org `CafeOrCoffeeShop` y `MenuItem` coherentes con el contenido visible. Si no hay productos definidos, usar datos demostrativos consistentes.
5. Aplicar `DESIGN.md` y comprobar semántica, accesibilidad, enlaces y presentación responsive en móvil y escritorio.

## Alcance y límites

- No modificar `docs/reference/base.html`, la navbar ni el footer.
- No añadir CSS propio, JavaScript ejecutable, backend ni funciones fuera de `specs/home/spec.md`.
- La prueba real del enlace a Menú dependerá de que exista `menu.html`.
