# Política de seguridad

## Versiones con soporte

| Versión | Soporte |
|---------|---------|
| 1.x     | Sí      |
| < 1.0   | No      |

## Cómo reportar una vulnerabilidad

Si encuentras un fallo de seguridad, **no abras un issue público**.

Usa el reporte privado de GitHub: pestaña **Security** → **Report a vulnerability**.

Incluye, si puedes:

- Descripción del problema y su impacto.
- Pasos para reproducirlo.
- Versión o commit afectado.

## Qué esperar

- Acuse de recibo en un plazo de 7 días.
- Información sobre el estado de la corrección cuando se haya analizado.
- Reconocimiento en la release que lo corrija, si lo deseas.

## Controles automáticos del proyecto

- Escaneo de la imagen Docker con Trivy en cada build; bloquea la publicación ante vulnerabilidades HIGH o CRITICAL con parche disponible.
- Dependabot para dependencias npm, acciones de GitHub y la imagen base.
- Contenedor sin privilegios de root y sin gestor de paquetes en la imagen final.