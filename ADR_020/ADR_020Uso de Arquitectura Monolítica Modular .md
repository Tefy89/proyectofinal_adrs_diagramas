# ADR 020: Uso de Arquitectura Monolítica Modular 
**Estado:** Aceptado

## Contexto
MANAGIX planea crecer en módulos, pero el equipo y los recursos actuales son reducidos.

## Decisión
Adoptar una **arquitectura monolítica modular**, preparada para separar servicios a futuro.

## Alternativas Consideradas
1. Microservicios desde el inicio.  
2. Arquitectura sin modularización.  
3. Serverless.  

## Consecuencias
- Reduce complejidad en el equipo.  
- Acelera el desarrollo inicial.  
- Permite extraer módulos críticos más adelante.  
