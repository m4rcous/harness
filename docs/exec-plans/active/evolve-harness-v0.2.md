# Execution Plan: Evolve Harness v0.1 to v0.2

## Estado

- Estado actual: Activo, listo para revisión humana
- Versión origen: v0.1
- Versión objetivo: v0.2
- Responsable: Bat Point
- Fecha de creación: 2026-04-30

## Objetivo

Evolucionar el Harness Engineering template de `v0.1` a `v0.2`, mejorando su claridad, consistencia y accionabilidad para proyectos académicos de ingeniería de software, sin cambiar la estructura principal del repositorio.

## Alcance

Este plan incluye:

- Revisar y ajustar la documentación existente para que sea más clara y fácil de aplicar.
- Fortalecer las especificaciones de producto para que funcionen como contrato funcional inicial.
- Agregar criterios más accionables para calidad, seguridad, confiabilidad y frontend.
- Definir una plantilla base para futuros execution plans.
- Alinear la documentación de arquitectura y frontend para evitar instrucciones contradictorias.
- Mejorar la utilidad académica del Harness mediante criterios de aceptación, evidencias y trazabilidad.

## Fuera de alcance

Este plan no incluye:

- Cambiar la estructura principal de carpetas.
- Introducir dependencias, frameworks o herramientas externas.
- Implementar una aplicación de ejemplo.
- Reescribir el Harness como producto final cerrado.
- Eliminar documentos existentes sin justificación.

## Pasos

1. [x] Revisar codificación y consistencia textual.
   - Verificar que los documentos se lean correctamente como UTF-8.
   - Corregir tildes, signos y términos inconsistentes si aparecen problemas reales en los archivos.
   - Unificar idioma, tono y nombres de conceptos.

2. [x] Mejorar `README.md`.
   - Explicar con mayor claridad para quién es el Harness.
   - Agregar una tabla breve con documentos principales y propósito.
   - Incluir una guía corta para adaptar la plantilla a un proyecto nuevo.
   - Alinear la estructura documentada con los archivos reales del repositorio.

3. [x] Mejorar `AGENTS.md`.
   - Aclarar el flujo esperado antes de modificar archivos.
   - Incluir criterios sobre cuándo revisar `QUALITY_SCORE.md`.
   - Aclarar cuándo crear, actualizar o cerrar execution plans.
   - Reforzar que el agente debe proponer actualizaciones documentales cuando falte contexto.

4. [x] Fortalecer `docs/product-specs/index.md`.
   - Agregar secciones para requisitos funcionales y no funcionales.
   - Incluir usuarios, stakeholders, restricciones, supuestos y criterios de aceptación.
   - Mantenerlo breve, pero suficientemente accionable para proyectos académicos.

5. [x] Alinear `ARCHITECTURE.md` y `docs/FRONTEND.md`.
   - Explicar cómo conviven una arquitectura por capas y una estructura frontend clásica.
   - Agregar reglas de simplificación para proyectos pequeños.
   - Mantener la separación entre lógica de negocio, aplicación, infraestructura e interfaz.

6. [x] Mejorar documentos de diseño, seguridad y confiabilidad.
   - Agregar checklists breves y verificables.
   - Incluir criterios mínimos de accesibilidad y estados de interfaz.
   - Agregar preguntas de revisión para errores, datos sensibles y fallos externos.

7. [x] Mejorar `docs/QUALITY_SCORE.md`.
   - Convertir la escala de calidad en una rúbrica más clara.
   - Incluir evidencia, observaciones y acciones recomendadas.
   - Relacionar puntajes bajos con deuda técnica cuando corresponda.

8. [x] Mejorar `docs/exec-plans/tech-debt-tracker.md`.
   - Marcar el registro actual como ejemplo removible.
   - Agregar campos útiles para seguimiento académico y técnico.
   - Definir estados y prioridades permitidas.

9. [x] Crear una plantilla de execution plan.
   - Agregar un formato reutilizable dentro de `docs/exec-plans/`.
   - Incluir objetivo, alcance, fuera de alcance, pasos, riesgos, validación y criterios de aceptación.

10. [x] Revisar coherencia final.
    - Confirmar que los documentos no se contradigan.
    - Confirmar que los cambios respeten la estructura principal.
    - Actualizar estado de versión a `v0.2` cuando se completen los cambios.

## Criterios de aceptación

La evolución a `v0.2` se considera completa cuando:

- `README.md` describe con claridad el propósito, uso y estructura real del Harness.
- `AGENTS.md` orienta al agente antes, durante y después de una tarea.
- `docs/product-specs/index.md` permite documentar requisitos académicos básicos.
- `ARCHITECTURE.md` y `docs/FRONTEND.md` están alineados y no dan instrucciones contradictorias.
- `docs/DESIGN.md`, `docs/SECURITY.md` y `docs/RELIABILITY.md` contienen criterios verificables.
- `docs/QUALITY_SCORE.md` incluye una rúbrica clara o criterios suficientes para justificar puntajes.
- `docs/exec-plans/` contiene una plantilla reutilizable para nuevos planes.
- La deuda técnica puede registrarse con estado, prioridad, impacto y acción recomendada.
- No se cambió la estructura principal del repositorio.
- La documentación sigue siendo breve, mantenible y fácil de usar por estudiantes y agentes.

## Riesgos

- Sobredocumentar la plantilla y volverla pesada para proyectos pequeños.
- Crear reglas demasiado rígidas para proyectos académicos simples.
- Duplicar criterios entre documentos y generar mantenimiento innecesario.
- Dejar inconsistencias entre la arquitectura sugerida y las guías frontend.
- Tratar el Harness como una aplicación concreta en lugar de una plantilla reutilizable.
- Actualizar documentos sin mantener un hilo claro entre producto, arquitectura, calidad y ejecución.

## Validación

Antes de cerrar este plan:

- [x] Revisar todos los documentos principales siguiendo el orden de `AGENTS.md`.
- [x] Confirmar que cada documento responde a una pregunta práctica del proyecto.
- [x] Confirmar que los placeholders sean útiles y fáciles de reemplazar.
- [x] Confirmar que el Harness siga siendo adecuado para proyectos personales y académicos.
- [x] Confirmar que no quedan caracteres mojibake detectables con búsqueda textual.
- Mover este plan a `docs/exec-plans/completed/` cuando los cambios de `v0.2` estén terminados y revisados.
