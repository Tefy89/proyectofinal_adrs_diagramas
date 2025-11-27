# ADR 029: Estándares de Manejo de Errores Centralizados
**Estado:** Aceptado

## Contexto
Los errores deben manejarse de forma homogénea para mejorar logging, debugging y claridad de respuestas.

## Decisión
Implementar un **filtro global de excepciones** en NestJS.

## Alternativas Consideradas
1. Manejo manual en cada controlador.  
2. Respuestas sin estructura.

## Consecuencias
- API consistente.  
- Respuestas claras para el frontend.  
- Mejor control durante fallas.
