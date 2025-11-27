# ADR 048: Separación de Variables de Entorno por Ambiente  
**Estado:** Aceptado

## Contexto
El sistema tendrá entornos distintos: desarrollo, staging y producción.

## Decisión
Crear archivos independientes:
- .env.development  
- .env.staging  
- .env.production  

## Alternativas Consideradas
1. Un solo archivo .env  
2. Variables hardcodeadas  

## Consecuencias
- Menor riesgo de errores  
- Despliegues más limpios  
- Mayor seguridad  
