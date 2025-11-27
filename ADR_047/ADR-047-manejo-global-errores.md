# ADR 047: Estándar para Manejo Global de Errores
**Estado:** Aceptado

## Contexto
Los errores se manejaban de forma inconsistente entre módulos, dificultando el debugging.

## Decisión
Crear un Global Exception Filter en NestJS que maneje:
- Errores de validación  
- Errores de negocio  
- Errores inesperados  

## Alternativas Consideradas
1. Manejo de errores dentro de cada controlador  
2. Middleware personalizado  

## Consecuencias
- Respuestas estandarizadas  
- Menos código repetido  
- Facilita debugging  
