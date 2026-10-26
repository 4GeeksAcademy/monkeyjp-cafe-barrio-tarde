
# Instrucciones para agentes

## Proyecto
Sitio web estático de una cafetería local.

Antes de implementar, consultar:
- CONTEXT.md para los requisitos y límites.
- DESIGN.md para los criterios visuales.
- specs/ para la funcionalidad correspondiente.

## Tecnologías
- HTML5 semántico.
- Tailwind CSS v4 por CDN.
- Sin React, JavaScript propio ni CSS adicional.
- No modificar server.py salvo necesidad justificada.

## Forma de trabajar
- Seguir SDD: spec.md, plan.md y tasks.md.
- No implementar funcionalidades fuera de la spec.
- Implementar tareas pequeñas.
- Actualizar tasks.md al finalizar cada tarea.
- Mantener consistencia visual entre páginas.
- No modificar archivos ajenos a la tarea sin avisar.

## Validación
- Comprobar navegación entre páginas.
- Revisar responsive en móvil y escritorio.
- Verificar labels y estructura semántica.
- No afirmar que algo se probó sin haberlo verificado.

## Git
- Usar ramas feature/.
- No trabajar directamente sobre main.
- No realizar commits, push ni merges sin confirmación.


## Diseño compartido

- DESIGN.md define las reglas visuales del proyecto.
- docs/reference/base.html es la plantilla HTML oficial.
- Toda página nueva debe partir de esa plantilla.
- Mantener Tailwind, navbar y footer sin modificaciones.
- Añadir el contenido específico dentro de main.
- No crear otro diseño o configuración de Tailwind.
- No modificar base.html sin autorización.