# ARCHITECTURE.md

Este documento define la arquitectura base que debe respetarse en los proyectos que utilicen este Harness.

## Objetivo

Definir una estructura arquitectónica clara para que humanos y agentes de IA puedan trabajar de forma consistente, mantenible y verificable.

## Principios arquitectónicos

- Separar responsabilidades.
- Evitar mezclar lógica de negocio con interfaz.
- Mantener módulos comprensibles y cohesionados.
- Preferir estructuras simples antes que abstracciones innecesarias.
- Documentar decisiones importantes.
- Diseñar pensando en pruebas y mantenimiento.

## Arquitectura sugerida

Para aplicaciones web, se recomienda una arquitectura modular por capas:

```text
src/
├── modules/
│   └── example/
│       ├── domain/
│       ├── application/
│       ├── infrastructure/
│       └── ui/
```

Esta estructura es una guía, no una obligación rígida. En proyectos pequeños puede simplificarse siempre que se mantenga clara la separación entre reglas de negocio, coordinación técnica e interfaz.

## Capas

### Domain

Contiene reglas de negocio, entidades, value objects y lógica central.

No debe depender de frameworks, UI ni infraestructura.

### Application

Contiene casos de uso y coordinación de operaciones.

Puede depender de `domain`.

### Infrastructure

Contiene detalles técnicos como APIs, base de datos, clientes HTTP, almacenamiento o servicios externos.

Puede implementar contratos definidos por capas superiores.

### UI

Contiene componentes visuales, pantallas, formularios y elementos de interacción.

No debe contener lógica de negocio compleja.

## Reglas de dependencia

- `ui` puede depender de `application`.
- `application` puede depender de `domain`.
- `infrastructure` puede depender de contratos definidos por `application` o `domain`.
- `domain` no debe depender de `ui`, `application` ni `infrastructure`.

## Ejemplos de decisiones permitidas

- Mantener validaciones de negocio en `domain`.
- Mantener casos de uso en `application`.
- Mantener llamadas HTTP, base de datos o almacenamiento en `infrastructure`.
- Mantener formularios, pantallas y componentes visuales en `ui`.

## Ejemplos de decisiones a evitar

- Colocar reglas de negocio complejas dentro de componentes visuales.
- Hacer que `domain` importe librerías de UI, base de datos o HTTP.
- Duplicar la misma lógica en varios componentes.
- Crear capas vacías que no aportan claridad al proyecto.

## Cuándo simplificar

En proyectos personales o académicos pequeños, se puede usar una estructura más simple si:

- El alcance es reducido.
- No hay múltiples módulos funcionales.
- La separación de responsabilidades sigue siendo evidente.
- La decisión queda documentada si afecta la arquitectura.

## Regla crítica

La lógica de negocio debe permanecer fuera de la interfaz visual.

## Cambios arquitectónicos

Todo cambio arquitectónico importante debe registrarse en un documento dentro de `docs/design-docs/`.
