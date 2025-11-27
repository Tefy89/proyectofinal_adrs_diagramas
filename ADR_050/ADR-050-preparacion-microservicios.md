# ADR 050: Preparación para Migración a Microservicios
**Fecha:** 2024  
**Estado:** Aceptado

## Contexto
Aunque MANAGIX usa un monolito modular, se proyecta crecimiento que puede requerir microservicios.

## Decisión
Aplicar principios que faciliten la futura migración:
- Separación por dominios  
- DTOs y servicios independientes  
- Tablas organizadas por contextos  
- Interfaces claras entre módulos  

## Alternativas Consideradas
1. Microservicios desde el inicio  
2. Monolito totalmente acoplado  

## Consecuencias
- Migración futura más simple  
- Menor riesgo técnico  
- Sin aumentar la complejidad actual  
