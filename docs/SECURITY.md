# SECURITY.md

Este documento define reglas básicas de seguridad para proyectos personales y académicos.

## Principios

- No confiar únicamente en el frontend.
- Validar entradas del usuario.
- Proteger datos sensibles.
- Evitar exponer secretos.
- Aplicar permisos según rol cuando corresponda.
- Mantener dependencias bajo revisión.
- Mostrar errores útiles sin revelar detalles internos.

## Reglas

- No guardar claves, tokens o contraseñas en el repositorio.
- Usar variables de entorno para configuración sensible.
- Incluir `.env.example` cuando sea útil documentar variables necesarias sin exponer secretos.
- Validar datos en backend cuando exista backend.
- No mostrar errores internos al usuario final.
- No exponer información sensible en logs.
- Revisar permisos antes de operaciones críticas.
- No agregar dependencias desconocidas sin justificación.

## Archivos sensibles

No subir al repositorio:

```text
.env
.env.local
*.pem
*.key
credentials.json
```

## Checklist antes de entregar

- ¿Hay secretos, tokens o credenciales en el repositorio?
- ¿Las entradas del usuario se validan antes de procesarse?
- ¿Los errores visibles evitan detalles internos?
- ¿Los logs evitan datos sensibles?
- ¿Las operaciones críticas revisan permisos o condiciones previas?
- ¿Las variables de entorno necesarias están documentadas sin exponer valores reales?

## Criterio mínimo

Un proyecto cumple el mínimo de seguridad cuando no expone secretos, valida entradas relevantes y evita revelar información interna al usuario final.
