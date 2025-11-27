# ADR 021: Implementación de Logs Centralizados con Winston
**Estado:** Aceptado

## Contexto
MANAGIX requiere almacenar logs que permitan rastrear errores, auditorías, excepciones y eventos críticos del sistema.  
Sin un sistema de logging estructurado, la depuración sería complicada, especialmente en entornos productivos y distribuidos.  
Además, se necesitan logs en formato JSON para integrarse con servicios externos como Loki, ELK o Grafana.

## Decisión
Utilizar **Winston** como biblioteca principal de logging en el backend.

## Alternativas Consideradas
1. Logger nativo de NestJS: simple pero limitado.  
2. Morgan: centrado en HTTP, no cubre todo el sistema.  
3. Pino: rápido pero requiere mayor configuración inicial.

## Consecuencias
- Logs estructurados en JSON.  
- Integración con servicios externos.  
- Mejor capacidad de monitoreo.  
- Ligero overhead en rendimiento.
