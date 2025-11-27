# ADR 014: Uso de Middleware para Logging de Requests
**Estado:** Aceptado

## Contexto
Se necesita monitorear qué peticiones se reciben, cuánto demoran, qué status code devuelven y qué módulo las procesa, para debugging y auditoría.

## Decisión
Implementar un middleware de logging usando **morgan** o el Logger propio de NestJS.

## Alternativas Consideradas
1. Logging manual en controladores.  
2. Logs en base de datos.  
3. Uso de herramientas externas únicamente.

## Consecuencias
- Seguimiento claro del flujo de peticiones.  
- Mejora la detección de fallas.  
- Impacto mínimo en rendimiento.  
