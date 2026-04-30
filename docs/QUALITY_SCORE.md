# QUALITY_SCORE.md

Este documento permite evaluar la calidad del proyecto o de sus módulos.

## Escala

| Puntaje | Significado | Criterio general |
|---:|---|---|
| 5 | Excelente | Cumple el criterio de forma clara, verificable y mantenible. |
| 4 | Bueno | Cumple el criterio con observaciones menores. |
| 3 | Aceptable | Cumple lo mínimo, pero requiere mejoras. |
| 2 | Débil | Tiene problemas relevantes que afectan mantenimiento o evaluación. |
| 1 | Crítico | Incumple el criterio o genera riesgo alto para el proyecto. |

## Criterios de evaluación

| Área | Qué se evalúa |
|---|---|
| Arquitectura | Separación de responsabilidades, dependencias y decisiones documentadas. |
| Claridad del código | Nombres, estructura, legibilidad y ausencia de complejidad innecesaria. |
| Separación de responsabilidades | Ubicación correcta de lógica de negocio, UI, infraestructura y casos de uso. |
| Pruebas | Evidencia de validación manual o automatizada de flujos relevantes. |
| Documentación | Requisitos, arquitectura, decisiones y uso del proyecto. |
| Seguridad | Manejo de secretos, validación de entradas, permisos y errores internos. |
| Confiabilidad | Manejo de errores, estados vacíos, fallos externos y trazabilidad. |
| Mantenibilidad | Facilidad para modificar, extender y revisar el proyecto. |

## Evaluación inicial

| Área | Puntaje | Evidencia | Observación | Acción recomendada |
|---|---:|---|---|---|
| Arquitectura | Pendiente | Pendiente | Aún no evaluado | Pendiente |
| Documentación | Pendiente | Pendiente | Aún no evaluado | Pendiente |
| Seguridad | Pendiente | Pendiente | Aún no evaluado | Pendiente |
| Confiabilidad | Pendiente | Pendiente | Aún no evaluado | Pendiente |
| Pruebas | Pendiente | Pendiente | Aún no evaluado | Pendiente |
| Mantenibilidad | Pendiente | Pendiente | Aún no evaluado | Pendiente |

## Reglas de uso

- Actualizar este documento al cerrar una fase importante.
- Registrar observaciones concretas.
- No usar puntajes sin justificación.
- Incluir evidencia: pruebas, revisión manual, capturas, commits o documentos relacionados.
- Relacionar problemas detectados con deuda técnica si corresponde.

## Guía rápida de interpretación

- Puntajes `4` o `5`: el área está en buen estado para una entrega académica.
- Puntaje `3`: el área puede entregarse, pero debe tener acciones recomendadas.
- Puntajes `1` o `2`: registrar deuda técnica o abrir un execution plan si el impacto es alto.
