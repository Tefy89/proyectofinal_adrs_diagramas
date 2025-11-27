# ADR 003: Selección de PostgreSQL como Base de Datos
Decisión técnica para datos críticos: confiabilidad, ACID y reporting avanzado.  
**Estado:** Aceptado  

## Contexto
MANAGIX gestionará datos transaccionales críticos (órdenes, inventario, clientes).  
Se requiere una base de datos con integridad referencial, transacciones ACID y soporte para reportes complejos.

## Decisión
Utilizar **PostgreSQL 15+** como base de datos relacional principal.

## Alternativas Consideradas
- **MySQL:** Similar pero con menos funciones avanzadas.
- **MongoDB:** Flexible, pero sin transacciones ACID completas inicialmente.
- **SQL Server:** Potente, pero con costos de licencia elevados.

## Consecuencias
- Transacciones ACID completas.  
- Uso de JSONB para datos semiestructurados.  
- Alto rendimiento en consultas complejas.  
- Ecosistema estable y open source.  
- Esquema rígido comparado con NoSQL.
