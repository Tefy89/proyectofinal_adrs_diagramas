# ADR 031: Implementación de Cache con Redis
Estado: Aceptado

## Contexto
El sistema requiere acelerar consultas repetitivas como usuarios, roles o configuraciones generales. Sin un sistema de caché, se sobrecargaría la base de datos y aumentaría el tiempo de respuesta.

## Decisión
Utilizar Redis como motor de caché in-memory para optimizar lecturas frecuentes.

## Alternativas Consideradas
1. Cache en memoria del servidor (no escalable).
2. Cache basado en archivos locales.
3. No usar cache (tiempos de respuesta insuficientes).

## Consecuencias
- Respuestas más rápidas en endpoints críticos.
- Menor carga en PostgreSQL.
- Requiere un contenedor adicional en Docker.
