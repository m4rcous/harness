# SECURITY.md

Este documento define reglas básicas de seguridad para proyectos personales y académicos.

## Principios

- No confiar únicamente en el frontend.
- Validar entradas del usuario.
- Proteger datos sensibles.
- Evitar exponer secretos.
- Aplicar permisos según rol cuando corresponda.
- Mantener dependencias bajo revisión.

## Reglas

- No guardar claves, tokens o contraseñas en el repositorio.
- Usar variables de entorno para configuración sensible.
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

