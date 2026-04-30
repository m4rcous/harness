# RELIABILITY.md

Este documento define criterios de confiabilidad para los proyectos que usen este Harness.

## Objetivo

Asegurar que el sistema se comporte de manera controlada ante errores, fallos, entradas inválidas o condiciones inesperadas.

## Principios

- Los errores deben manejarse explícitamente.
- El usuario no debe ver errores técnicos internos.
- Las operaciones críticas deben ser verificables.
- El sistema debe evitar fallos silenciosos.
- Los estados de error deben ser comprensibles.

## Reglas

- Toda llamada externa debe considerar manejo de error.
- Toda operación asíncrona debe considerar carga, éxito y fallo.
- Los formularios deben validar entradas antes de procesar.
- Los errores deben registrarse cuando sea necesario.
- No se deben ocultar fallos importantes sin trazabilidad.

## Preguntas de revisión

- ¿Qué pasa si falla una API?
- ¿Qué pasa si el usuario ingresa datos inválidos?
- ¿Qué pasa si no hay conexión?
- ¿Qué pasa si la respuesta llega incompleta?
- ¿Qué mensaje verá el usuario?
- ¿Cómo se detecta el error durante desarrollo o producción?