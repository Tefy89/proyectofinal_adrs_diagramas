# ADR 042: Uso de DTOs Estrictos en Todo el Backend 
**Estado:** Aceptado

## Contexto
El flujo de datos entre frontend, backend y la base de datos debe validarse y estandarizarse. Aunque NestJS soporta DTOs, el equipo no los estaba aplicando en todos los módulos.

## Decisión
Implementar DTOs estrictos con `class-validator` y `class-transformer` en cada endpoint.

## Alternativas Consideradas
1. Validación manual en controladores  
2. Validación únicamente en el frontend  

## Consecuencias
- Mayor consistencia de datos  
- Menos errores en producción  
- Aumenta ligeramente el tiempo de desarrollo inicial  
