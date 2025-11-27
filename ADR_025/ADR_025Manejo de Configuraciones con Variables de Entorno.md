# ADR 025: Manejo de Configuraciones con Variables de Entorno
**Estado:** Aceptado

## Contexto
Es necesario separar configuraciones entre ambientes (dev, test, prod).  
Exponer valores sensibles en el código representa un riesgo de seguridad.

## Decisión
Utilizar variables de entorno junto con **ConfigModule** de NestJS.

## Alternativas Consideradas
1. Configuración manual por archivo.  
2. Hardcode en el código (inseguro).

## Consecuencias
- Seguridad mejorada.  
- Configuración flexible por ambiente.  
- Integración simple con Docker.
