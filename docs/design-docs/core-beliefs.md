# Core Beliefs

Este documento define los principios centrales que guían el uso de este Harness.

## Principios

### 1. El repositorio es la fuente de verdad

Las decisiones importantes deben estar documentadas dentro del repositorio, no solo en conversaciones, chats o memoria personal.

Aplicación práctica: si una decisión cambia requisitos, arquitectura o calidad, debe reflejarse en el documento correspondiente.

### 2. El agente necesita contexto claro

Un agente de IA trabaja mejor cuando puede consultar producto, arquitectura, reglas, planes y restricciones.

Aplicación práctica: antes de pedir implementación, mantener actualizados los documentos mínimos del proyecto.

### 3. La documentación debe ser accionable

La documentación debe ayudar a tomar decisiones y ejecutar tareas, no solo describir el sistema de forma pasiva.

Aplicación práctica: cada documento debe responder qué hacer, qué evitar o cómo validar.

### 4. La arquitectura debe ser respetada

Los cambios deben alinearse con la estructura definida. Si la arquitectura cambia, debe actualizarse la documentación.

Aplicación práctica: registrar cambios arquitectónicos en `docs/design-docs/`.

### 5. La calidad debe poder observarse

La calidad no debe depender solo de opinión. Debe evaluarse mediante criterios, pruebas, revisión y documentación.

Aplicación práctica: usar `docs/QUALITY_SCORE.md` al cerrar fases relevantes.

### 6. La seguridad y confiabilidad son parte del diseño

No deben tratarse como aspectos finales. Deben considerarse desde el inicio del proyecto.

Aplicación práctica: revisar `docs/SECURITY.md` y `docs/RELIABILITY.md` cuando haya datos, errores o llamadas externas.

### 7. El Harness evoluciona

Esta estructura puede adaptarse según el tamaño, complejidad y tipo de proyecto.

Aplicación práctica: simplificar cuando el proyecto sea pequeño, pero dejar registro de decisiones relevantes.
