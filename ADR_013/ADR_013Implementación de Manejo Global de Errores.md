# ADR 013: Implementación de Manejo Global de Errores
**Estado:** Aceptado

## Contexto
El backend requiere una forma consistente de manejar errores para que el frontend reciba respuestas uniformes, con mensajes claros y códigos HTTP apropiados.

## Decisión
Crear un **Global Exception Filter** personalizado en NestJS.

## Alternativas Consideradas
1. Manejo de errores en cada controlador.  
2. Middleware específico.  
3. Uso exclusivo de excepciones nativas sin filtro global.

## Consecuencias
- Todas las respuestas de error siguen el mismo formato.  
- Mejora la depuración y lectura de logs.  
- Código más limpio al eliminar try/catch repetidos.  
