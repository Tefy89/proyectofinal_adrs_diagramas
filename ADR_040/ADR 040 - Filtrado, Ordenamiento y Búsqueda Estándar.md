# ADR 040: Implementación de Filtrado, Ordenamiento y Búsqueda Estándar
Estado: Aceptado

## Contexto
Muchos módulos necesitan listados con filtros avanzados. Repetir la misma lógica en cada módulo genera duplicación y errores.

## Decisión
Crear un módulo utilitario central para filtros, ordenamiento, paginación y búsqueda.

## Alternativas Consideradas
1. Repetir la lógica en cada módulo.
2. Librerías externas no diseñadas para NestJS.

## Consecuencias
- Reutilización de lógica.
- Mejor rendimiento y calidad en consultas.
