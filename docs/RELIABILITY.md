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
- Las respuestas vacías o incompletas deben tratarse como escenarios esperados.

## Reglas

- Toda llamada externa debe considerar manejo de error.
- Toda operación asíncrona debe considerar carga, éxito y fallo.
- Los formularios deben validar entradas antes de procesar.
- Los errores deben registrarse cuando sea necesario.
- No se deben ocultar fallos importantes sin trazabilidad.
- Los mensajes al usuario deben explicar el problema y, cuando sea posible, una acción siguiente.

## Estrategias recomendadas

- Usar estados explícitos para carga, error, vacío y éxito.
- Definir mensajes claros para errores esperables.
- Registrar información suficiente para depurar sin exponer datos sensibles.
- Considerar reintentos o alternativas solo cuando tengan sentido para el flujo.
- Validar respuestas incompletas antes de usarlas.

## Preguntas de revisión

- ¿Qué pasa si falla una API?
- ¿Qué pasa si el usuario ingresa datos inválidos?
- ¿Qué pasa si no hay conexión?
- ¿Qué pasa si la respuesta llega incompleta?
- ¿Qué mensaje verá el usuario?
- ¿Cómo se detecta el error durante desarrollo o producción?
- ¿Existe una forma clara de recuperarse o volver a intentar?

## Criterio mínimo

Un proyecto cumple el mínimo de confiabilidad cuando sus flujos principales manejan errores esperables, comunican estados al usuario y dejan evidencia suficiente para depurar fallos importantes.
