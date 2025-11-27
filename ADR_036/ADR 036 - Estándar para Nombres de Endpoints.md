# ADR 036: Estándar para Nombres de Endpoints
Estado: Aceptado

## Contexto
Se requiere una convención clara para nombres de rutas REST, ya que múltiples equipos consumirán la API.

## Decisión
Usar rutas en plural, minúsculas y basadas en recursos. Ejemplos:
- /users
- /teams
- /reports

## Alternativas Consideradas
1. Endpoints en singular.
2. Rutas mixtas sin convención.

## Consecuencias
- API más clara y estándar.
- Menos confusiones para integraciones externas.
