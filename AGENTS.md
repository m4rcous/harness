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
9. `docs/QUALITY_SCORE.md` si la tarea afecta evaluación, cierre de fase o entrega académica.
10. `docs/exec-plans/active/` si existe un plan de ejecución vigente relacionado con la tarea.

## Flujo de trabajo esperado

Antes de modificar:

- Identificar el objetivo de la tarea.
- Revisar los documentos relacionados.
- Identificar archivos probablemente afectados.
- Confirmar si existe un execution plan activo aplicable.
- Proponer actualización documental si falta contexto funcional, técnico o académico.

Durante la tarea:

- Mantener los cambios dentro del alcance solicitado.
- Preferir soluciones simples, mantenibles y verificables.
- Actualizar el execution plan activo si la tarea forma parte de uno.
- Registrar deuda técnica si se detecta un problema que no se resolverá en la misma tarea.

Al finalizar:

- Verificar que el cambio solicitado fue realizado.
- Actualizar documentación relacionada cuando corresponda.
- Explicar brevemente qué cambió, por qué y cómo se validó.
- Indicar riesgos, pendientes o decisiones relevantes.

## Reglas generales para agentes

- No modificar archivos fuera del alcance de la tarea.
- No eliminar documentación sin justificarlo.
- No introducir nuevas dependencias sin explicar el motivo.
- No cambiar decisiones arquitectónicas sin actualizar la documentación correspondiente.
- Si una tarea es compleja, crear o actualizar un execution plan en `docs/exec-plans/active/`.
- Si se identifica deuda técnica, registrarla en `docs/exec-plans/tech-debt-tracker.md`.
- Mantener la documentación clara, breve y accionable.
- Priorizar soluciones simples, mantenibles y verificables.
- No asumir reglas de negocio que no estén documentadas.

## Uso de execution plans

Crear o actualizar un execution plan cuando:

- La tarea tenga varios pasos o afecte varios documentos o módulos.
- Existan riesgos técnicos, académicos o de alcance.
- Sea necesario dejar trazabilidad para revisión posterior.
- La tarea implique una decisión relevante de arquitectura, producto o calidad.

Un plan activo debe mantenerse en `docs/exec-plans/active/`. Cuando la tarea esté revisada y aceptada, puede moverse a `docs/exec-plans/completed/`.

## Criterio de finalización

Una tarea se considera terminada cuando:

- El cambio solicitado fue realizado.
- La documentación relacionada fue actualizada.
- No se rompieron reglas arquitectónicas.
- Se dejó registro de decisiones relevantes.
- Se explicó brevemente qué se cambió y por qué.
- Se indicaron validaciones realizadas o limitaciones pendientes.

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
