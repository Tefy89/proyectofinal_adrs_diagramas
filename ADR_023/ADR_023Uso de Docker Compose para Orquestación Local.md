# ADR 023: Uso de Docker Compose para Orquestación Local
**Estado:** Aceptado

## Contexto
El proyecto requiere levantar varios servicios localmente (backend, base de datos, frontend, nginx).  
Hacerlo manualmente es costoso y propenso a errores.

## Decisión
Utilizar **Docker Compose** como orquestador para entornos de desarrollo.

## Alternativas Consideradas
1. Ejecutar servicios manualmente.  
2. Usar Swarm local (excesivo para desarrollo).

## Consecuencias
- Reproducibilidad completa del entorno local.  
- Inicio automático de todos los contenedores.  
- Facilita onboarding de nuevos desarrolladores.
