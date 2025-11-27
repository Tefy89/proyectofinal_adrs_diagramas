# ADR 012: Validación de Datos con Class-Validator
**Estado:** Aceptado

## Contexto
Los datos enviados por usuarios y por el frontend deben ser validados para evitar inconsistencias, errores y datos corruptos, especialmente en operaciones como creación de órdenes, clientes e inventarios.

## Decisión
Utilizar **class-validator + class-transformer** dentro de NestJS para validar todos los DTOs.

## Alternativas Consideradas
1. Joi  
2. Zod  
3. Validación manual en controladores  

## Consecuencias
- Centraliza validaciones en los DTOs.  
- Reduce errores de entrada.  
- Evita duplicación de reglas.  
- Agrega dependencias extra, pero son estándar en NestJS.  
