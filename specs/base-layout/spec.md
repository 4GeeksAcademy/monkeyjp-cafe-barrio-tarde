# Especificación: Plantilla HTML común

## Objetivo

Definir una plantilla HTML de referencia para mantener una estructura y una presentación compartidas entre las páginas Inicio, Menú y Pedido de Café Barrio.

## Alcance

La plantilla se ubicará en `docs/reference/base.html` y contendrá únicamente la estructura común: configuración del documento, carga de Tailwind CSS v4 mediante CDN, navbar, un elemento `main` vacío y footer. Esta especificación describe los requisitos; no incluye la implementación de la plantilla.

## Requisitos

- El documento debe usar HTML5 semántico y definir el idioma español, la codificación de caracteres y el viewport para dispositivos móviles.
- Tailwind CSS v4 debe cargarse mediante CDN. No se debe añadir CSS propio ni JavaScript.
- La navbar debe mostrar la marca Café Barrio a la izquierda y enlaces a Menú y Pedido a la derecha. Su distribución debe adaptarse a móvil y escritorio.
- El elemento `main` debe estar presente y vacío de contenido específico de página, para que cada página pueda incorporar allí su contenido.
- El footer debe incluir la dirección, el horario de atención y un enlace a Pedido, según el contexto del negocio.
- Navbar y footer deben mantener el mismo contenido y estilo en las tres páginas.
- La presentación debe seguir `DESIGN.md`: diseño minimalista y cálido, colores y tipografías definidos, contenedor central y enfoque mobile-first.
- La estructura debe ser accesible: usar landmarks semánticos, enlaces con nombres comprensibles y una jerarquía de documento clara.

## Fuera de alcance

- Contenido de bienvenida, productos destacados, categorías del menú o formulario de pedidos.
- Filtros funcionales, lógica de interacción, procesamiento de pedidos o conexión a backend.
- Componentes o estilos que no formen parte de la estructura común indicada.

## Criterios de aceptación

- Existe la especificación en `specs/base-layout/spec.md` y señala `docs/reference/base.html` como destino de la plantilla.
- La plantilla de referencia prevista comparte navbar y footer entre Inicio, Menú y Pedido.
- El `main` queda reservado para contenido de página y no introduce contenido específico por sí mismo.
- Se respetan las tecnologías y límites del proyecto: HTML5 y Tailwind CSS v4 por CDN, sin CSS adicional ni JavaScript propio.
- La estructura prevista es semántica, accesible y responsive, y mantiene la consistencia visual descrita en `DESIGN.md`.
