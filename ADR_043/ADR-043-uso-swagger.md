# ADR 043: Uso de Swagger para Documentar la API  
**Estado:** Aceptado

## Contexto
Los módulos están creciendo y se necesita documentar los endpoints para facilitar el consumo desde frontend y clientes externos.

## Decisión
Integrar Swagger en NestJS para documentar toda la API.

## Alternativas Consideradas
1. Documentación manual en PDF  
2. Postman Collections  
3. No documentar (no viable)

## Consecuencias
- Documentación automática  
- Mejor comunicación entre equipos  
- Requiere mantener decoradores actualizados  
