# AGENTS.md

Este repositorio está preparado para trabajo asistido por agentes de IA.

El objetivo de este archivo no es contener toda la documentación del proyecto, sino orientar al agente hacia los documentos correctos antes de modificar código o documentación.

## Orden de lectura recomendado

Antes de realizar una tarea, el agente debe revisar:

1. `README.md` para entender el propósito general del repositorio.
2. `ARCHITECTURE.md` para comprender la arquitectura base.
3. `docs/product-specs/index.md` para revisar el contexto funcional.
4. `docs/design-docs/core-beliefs.md` para entender los principios del proyecto.
5. `docs/DESIGN.md` si la tarea afecta experiencia de usuario o diseño visual.
6. `docs/FRONTEND.md` si la tarea afecta frontend.
7. `docs/SECURITY.md` si la tarea afecta datos, permisos, autenticación o exposición de información.
8. `docs/RELIABILITY.md` si la tarea afecta errores, disponibilidad, logs o comportamiento ante fallos.
9. `docs/exec-plans/active/` si existe un plan de ejecución vigente relacionado con la tarea.

## Reglas generales para agentes

- No modificar archivos fuera del alcance de la tarea.
- No eliminar documentación sin justificarlo.
- No introducir nuevas dependencias sin explicar el motivo.
- No cambiar decisiones arquitectónicas sin actualizar la documentación correspondiente.
- Si una tarea es compleja, crear o actualizar un execution plan en `docs/exec-plans/active/`.
- Si se identifica deuda técnica, registrarla en `docs/exec-plans/tech-debt-tracker.md`.
- Mantener la documentación clara, breve y accionable.
- Priorizar soluciones simples, mantenibles y verificables.

## Criterio de finalización

Una tarea se considera terminada cuando:

- El cambio solicitado fue realizado.
- La documentación relacionada fue actualizada.
- No se rompieron reglas arquitectónicas.
- Se dejó registro de decisiones relevantes.
- Se explicó brevemente qué se cambió y por qué.

## Estilo de trabajo esperado

El agente debe actuar como asistente de ingeniería de software, no solo como generador de texto o código.

Debe razonar sobre:

- Requisitos.
- Arquitectura.
- Mantenibilidad.
- Seguridad.
- Confiabilidad.
- Calidad.
- Claridad para futuros desarrolladores.