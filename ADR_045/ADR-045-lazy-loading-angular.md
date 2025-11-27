# ADR 045: Implementación de Lazy Loading en Angular 
**Estado:** Aceptado

## Contexto
La aplicación creció a más de 10 módulos visuales, y el bundle inicial se volvió pesado.

## Decisión
Aplicar Lazy Loading en cada módulo de Angular.

## Alternativas Consideradas
1. Carga total inicial (eager loading)  
2. Separar la app en múltiples aplicaciones  

## Consecuencias
- Mejor rendimiento inicial  
- Carga de secciones solo cuando el usuario las necesita  
- Requiere reorganización de rutas  
