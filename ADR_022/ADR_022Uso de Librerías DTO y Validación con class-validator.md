# ADR 022: Uso de Librerías DTO y Validación con class-validator
**Estado:** Aceptado

## Contexto
Se necesita garantizar que todo dato recibido por los controladores sea validado con reglas estrictas (tipos, tamaños, formatos).  
Esto evita datos corruptos y reduce errores en la base de datos.

## Decisión
Usar **class-validator** junto con **class-transformer** para validar DTOs en NestJS.

## Alternativas Consideradas
1. Validación manual: más trabajo y menos consistencia.  
2. Yup: funcional pero no tan integrado con NestJS.

## Consecuencias
- Validación automática de datos.  
- Mayor consistencia entre módulos.  
- Reducción de errores en producción.
