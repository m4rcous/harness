# Harness

Este repositorio contiene una estructura base de **Harness Engineering** para proyectos personales y académicos de ingeniería de software.

El objetivo es disponer de un entorno documentado, organizado y reutilizable para trabajar con agentes de IA como asistentes de desarrollo, manteniendo control sobre el contexto, la arquitectura, la calidad, la seguridad, la confiabilidad y los planes de ejecución.

## Para quién es

Este Harness está pensado para:

- Estudiantes que necesitan desarrollar y justificar proyectos de ingeniería de software.
- Proyectos personales que requieren orden sin una carga documental excesiva.
- Equipos pequeños que usan agentes de IA para acelerar análisis, implementación y revisión.
- Repositorios que necesitan mantener decisiones, requisitos y criterios de calidad dentro del propio proyecto.

## Propósito

Este Harness busca que una persona o agente de IA pueda:

- Entender el propósito del proyecto.
- Consultar la arquitectura definida.
- Identificar requisitos y alcance funcional.
- Respetar reglas de diseño, frontend, seguridad y confiabilidad.
- Seguir planes de ejecución para tareas complejas.
- Registrar deuda técnica y decisiones relevantes.
- Evaluar la calidad con criterios observables.

## Estructura

```text
AGENTS.md
ARCHITECTURE.md
docs/
├── design-docs/
│   ├── core-beliefs.md
│   └── index.md
├── exec-plans/
│   ├── active/
│   ├── completed/
│   ├── execution-plan-template.md
│   └── tech-debt-tracker.md
├── product-specs/
│   └── index.md
├── references/
│   └── llm-notes.md
├── DESIGN.md
├── FRONTEND.md
├── QUALITY_SCORE.md
├── RELIABILITY.md
└── SECURITY.md
```

## Documentos principales

| Documento | Propósito |
|---|---|
| `AGENTS.md` | Punto de entrada para agentes de IA. Define orden de lectura, reglas y criterio de finalización. |
| `ARCHITECTURE.md` | Define la arquitectura base, capas sugeridas y reglas de dependencia. |
| `docs/product-specs/index.md` | Centraliza problema, usuarios, alcance y requisitos del producto. |
| `docs/design-docs/` | Guarda decisiones técnicas, alternativas evaluadas y consecuencias. |
| `docs/exec-plans/` | Organiza planes de trabajo activos, completados y deuda técnica. |
| `docs/DESIGN.md` | Define criterios mínimos de experiencia de usuario e interfaz. |
| `docs/FRONTEND.md` | Define reglas para proyectos con interfaz frontend. |
| `docs/SECURITY.md` | Define controles básicos para proteger datos, secretos y permisos. |
| `docs/RELIABILITY.md` | Define criterios para manejar errores, fallos y estados inesperados. |
| `docs/QUALITY_SCORE.md` | Permite evaluar calidad con criterios y evidencias. |

## Uso recomendado

1. Copiar esta estructura en un nuevo proyecto.
2. Completar `docs/product-specs/index.md` con el problema, usuarios, alcance y requisitos.
3. Ajustar `ARCHITECTURE.md` según el tipo de sistema, sin perder las reglas de separación de responsabilidades.
4. Usar `AGENTS.md` como punto de entrada para cualquier agente de IA.
5. Crear un execution plan para tareas complejas en `docs/exec-plans/active/`.
6. Registrar decisiones importantes en `docs/design-docs/`.
7. Actualizar calidad, deuda técnica y documentación al cerrar fases relevantes.

## Adaptación a proyectos pequeños

No todos los proyectos necesitan usar todos los documentos con el mismo nivel de detalle. En proyectos personales o académicos simples, basta con mantener claros:

- Problema y alcance.
- Arquitectura o estructura elegida.
- Requisitos principales.
- Riesgos técnicos relevantes.
- Criterios de aceptación.
- Evidencia de pruebas o validación.

## Estado

Versión candidata: `v0.2-rc1`
