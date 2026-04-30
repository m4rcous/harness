# FRONTEND.md

Este documento define reglas para proyectos frontend.

## Principios

- Separar componentes visuales de lógica de negocio.
- Mantener componentes pequeños y reutilizables.
- Evitar duplicación de lógica.
- Usar nombres claros.
- Mantener consistencia con el sistema de diseño del proyecto.

## Estructura sugerida

```text
src/
├── components/
├── modules/
├── pages/
├── services/
├── hooks/
├── styles/
└── utils/
```

## Reglas

- Los componentes visuales no deben contener lógica de negocio compleja.
- Las llamadas a APIs deben estar en servicios o funciones separadas.
- Los formularios deben validar entradas.
- Toda pantalla debe manejar estados de carga y error.
- No crear componentes duplicados si ya existe uno reutilizable.
- Evitar archivos demasiado grandes.

## Criterios de revisión

Antes de considerar terminado un cambio frontend, revisar:

- ¿La pantalla es clara?
- ¿El componente tiene una sola responsabilidad?
- ¿Se manejan errores?
- ¿Se manejan estados vacíos?
- ¿Hay nombres comprensibles?
- ¿Se evitó duplicación?