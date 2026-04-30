# FRONTEND.md

Este documento define reglas para proyectos con interfaz frontend.

## Principios

- Separar componentes visuales de lógica de negocio.
- Mantener componentes pequeños y reutilizables.
- Evitar duplicación de lógica.
- Usar nombres claros.
- Mantener consistencia con el sistema de diseño del proyecto.
- Diseñar para estados de carga, error, vacío y éxito.

## Relación con la arquitectura

`ARCHITECTURE.md` propone una estructura modular por capas. En proyectos frontend, esa estructura puede convivir con carpetas comunes como `components`, `pages`, `services`, `hooks`, `styles` y `utils`.

La regla principal es mantener clara la responsabilidad:

- La lógica de negocio pertenece a `domain` o `application`.
- Las llamadas externas pertenecen a `infrastructure`, `services` o adaptadores equivalentes.
- La interfaz pertenece a `ui`, `components` o `pages`.
- Las utilidades compartidas no deben convertirse en un lugar para esconder reglas de negocio.

## Estructura sugerida

Para proyectos pequeños:

```text
src/
├── components/
├── pages/
├── services/
├── hooks/
├── styles/
└── utils/
```

Para proyectos con más dominio funcional:

```text
src/
├── modules/
│   └── example/
│       ├── domain/
│       ├── application/
│       ├── infrastructure/
│       └── ui/
└── shared/
```

## Reglas

- Los componentes visuales no deben contener lógica de negocio compleja.
- Las llamadas a APIs deben estar en servicios, adaptadores o infraestructura.
- Los formularios deben validar entradas antes de enviar datos.
- Toda pantalla debe manejar estados de carga, error y vacío cuando correspondan.
- No crear componentes duplicados si ya existe uno reutilizable.
- Evitar archivos demasiado grandes o con múltiples responsabilidades.
- Mantener textos de interfaz claros para el usuario final.

## Accesibilidad y responsive design

Como mínimo:

- Usar contraste suficiente entre texto y fondo.
- Mantener navegación comprensible con teclado cuando aplique.
- Asociar etiquetas visibles o accesibles a campos de formulario.
- Evitar que textos, botones o paneles se superpongan en pantallas pequeñas.
- Probar los flujos principales en al menos un tamaño móvil y uno de escritorio.

## Criterios de revisión

Antes de considerar terminado un cambio frontend, revisar:

- ¿La pantalla es clara?
- ¿El componente tiene una sola responsabilidad?
- ¿Se manejan errores?
- ¿Se manejan estados vacíos?
- ¿Hay nombres comprensibles?
- ¿Se evitó duplicación?
- ¿La interfaz es usable en móvil y escritorio?
- ¿La lógica de negocio quedó fuera de la UI?
