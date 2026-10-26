# Especificación: plantilla HTML común

## Objetivo

Definir una plantilla de referencia compartida para las páginas de Café Barrio. El archivo de referencia se guardará en `docs/reference/base.html` y servirá como estructura inicial para Inicio, Menú y Pedido.

## Alcance

La plantilla establece el documento HTML común, la carga de Tailwind CSS v4 por CDN, la navegación principal, un elemento `main` vacío y el pie de página compartido. No define el contenido específico de cada página.

## Requisitos

### Estructura del documento

- El archivo de referencia debe ser un documento HTML5 válido y usar el idioma español.
- Debe incluir metadatos básicos para el juego de caracteres y el viewport.
- Debe cargar Tailwind CSS v4 por CDN para los estilos.
- No debe depender de React, JavaScript propio, backend, base de datos ni hojas de estilo adicionales.
- La plantilla debe mantener el contenido de página dentro de un `main` semántico, inicialmente vacío.

### Navegación

- Debe incluir una navegación semántica común a las páginas del sitio.
- Debe mostrar la identidad de Café Barrio y enlaces a Inicio, Menú y Pedido.
- Los enlaces deben apuntar a las páginas correspondientes (`index.html`, `menu.html` y `order.html`).
- La navegación debe ser usable con teclado y tener nombres accesibles.

### Pie de página

- Debe incluir un pie semántico común a las páginas del sitio.
- Debe reservar contenido para la dirección y el horario del café, según los datos definidos para el sitio.
- Debe incluir un enlace a Pedido que apunte a `order.html`.

### Presentación y responsive

- La estructura debe permitir el diseño mobile-first establecido en `DESIGN.md`.
- Debe seguir la paleta, tipografías, contenedor y estilo visual establecidos en `DESIGN.md`, usando utilidades de Tailwind.
- La navegación y el pie deben conservar una presentación consistente entre las tres páginas.
- El HTML debe usar elementos semánticos y mantener contraste y foco visibles para la interacción accesible.

## Fuera de alcance

- Contenido del hero, productos destacados, menú o formulario de pedidos.
- Comportamiento funcional de filtros o procesamiento de pedidos.
- Datos de productos o valores concretos de dirección y horario no especificados por el proyecto.
- Implementación de páginas completas o cambios al servidor.

## Criterios de aceptación

- Existe una especificación para la plantilla común en `specs/base-layout/spec.md` y establece `docs/reference/base.html` como destino de la plantilla.
- La plantilla de referencia, cuando se implemente, tendrá una estructura HTML5 en español con Tailwind CSS v4 por CDN.
- La plantilla incluirá navbar, `main` vacío y footer, con enlaces válidos entre las tres páginas.
- La estructura compartida será semántica, accesible y apta para móvil y escritorio, sin añadir tecnologías fuera de los límites del proyecto.