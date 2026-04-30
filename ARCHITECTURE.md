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

## Capas
### Domain

Contiene reglas de negocio, entidades, value objects y lógica central.

No debe depender de frameworks, UI ni infraestructura.

### Application

Contiene casos de uso y coordinación de operaciones.

Puede depender de `domain`.

### Infraestructure

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