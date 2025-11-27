# ADR 018: Separación del Entorno en Archivos .env 
**Estado:** Aceptado

## Contexto
Las credenciales y configuraciones del sistema no deben estar hardcodeadas en el código fuente.

## Decisión
Crear archivos .env separados:
- .env.development  
- .env.production  
- .env.test  

## Alternativas Consideradas
1. Variables definidas dentro de Docker.  
2. Configuración en el código.  
3. JSON con credenciales (inseguro).  

## Consecuencias
- Mayor seguridad.  
- Facilita despliegue.  
- Menor riesgo de exposición accidental.  
