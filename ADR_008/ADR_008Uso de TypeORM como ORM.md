# ADR 008: Uso de TypeORM como ORM
Decisión técnica para comunicación con PostgreSQL usando TypeScript.  
**Estado:** Aceptado  

## Contexto
Se requiere un ORM que integre de manera natural con NestJS y PostgreSQL.

## Decisión
Utilizar **TypeORM** como ORM principal del proyecto.

## Alternativas Consideradas
- **Prisma:** Muy moderno, pero menos integrado en NestJS.  
- **Sequelize:** Madura, pero con API menos intuitiva para TS.  

## Consecuencias
- Integración directa con NestJS.  
- Migraciones estructuradas.  
- Decoradores y entidades claras.  
- Menor rendimiento en casos extremos comparado con SQL crudo.
