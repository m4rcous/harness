# Technical Debt Tracker

Este documento registra deuda técnica identificada durante el desarrollo.

## Estados permitidos

- `pendiente`
- `en progreso`
- `resuelta`
- `aceptada`

## Prioridades permitidas

- `alta`
- `media`
- `baja`

## Formato

```text
ID:
Título:
Estado:
Prioridad:
Severidad:
Módulo:
Descripción:
Impacto:
Acción recomendada:
Fecha detectada:
Fecha objetivo:
Relacionado con:
```

## Deuda técnica registrada

El siguiente registro es un ejemplo removible. Reemplazarlo cuando exista deuda técnica real.

```text
ID: TD-001
Título: Ejemplo de deuda técnica
Estado: pendiente
Prioridad: baja
Severidad: baja
Módulo: documentación
Descripción: Este es un ejemplo inicial para mostrar el formato de registro.
Impacto: Permite entender cómo documentar deuda técnica.
Acción recomendada: Eliminar este ejemplo cuando se registre la primera deuda técnica real.
Fecha detectada: 2026-04-30
Fecha objetivo: Pendiente
Relacionado con: docs/QUALITY_SCORE.md
```

## Reglas de uso

- Registrar deuda técnica cuando un problema no se resolverá en la misma tarea.
- Mantener descripciones breves y accionables.
- Relacionar deuda relevante con execution plans, módulos, commits o criterios de calidad.
- Cerrar o actualizar registros cuando la deuda sea resuelta o aceptada conscientemente.
