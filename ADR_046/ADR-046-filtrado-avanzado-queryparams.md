# ADR 046: Inclusión de Filtrado Avanzado desde Query Params
**Estado:** Aceptado

## Contexto
Los módulos como Inventario y Órdenes requieren filtros complejos: fechas, rangos, estado, cliente, empleado.

## Decisión
Crear un motor unificado que interprete filtros desde la URL usando Query Params estandarizados.

## Alternativas Consideradas
1. Filtros individuales por módulo  
2. Filtros manuales por cada controlador  

## Consecuencias
- Consultas más potentes  
- Menos repetición de código  
- Requiere documentación clara  
