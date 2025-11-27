# ADR 027: Uso de Prisma como ORM Alternativo para Nuevos Módulos
**Estado:** Aceptado

## Contexto
Aunque TypeORM se usa inicialmente, algunos módulos requieren consultas optimizadas y migraciones más estables.

## Decisión
Agregar **Prisma** como ORM para módulos modernos del sistema.

## Alternativas Consideradas
1. Mantener solo TypeORM.  
2. Migrar todo a Prisma.

## Consecuencias
- Modelos más robustos.  
- Migraciones más simples.  
- Arquitectura híbrida ORM.
