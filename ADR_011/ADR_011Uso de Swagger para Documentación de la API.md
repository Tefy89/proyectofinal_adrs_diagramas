# ADR 011: Uso de Swagger para Documentación de la API
**Estado:** Aceptado

## Contexto
Para MANAGIX, es necesario que el equipo de desarrollo y futuros integradores externos cuenten con una referencia clara y navegable de los endpoints, parámetros, respuestas y permisos requeridos.  
La documentación manual es propensa a errores y difícil de mantener conforme avanza el proyecto.

## Decisión
Implementar **Swagger (OpenAPI)** como herramienta de documentación automática de la API en NestJS.

## Alternativas Consideradas
1. Postman Collections — útil pero requiere mantenimiento manual.  
2. Redoc — buena visualización, pero depende de OpenAPI.  
3. Documentación manual — alto riesgo de desactualización.

## Consecuencias
- Documentación generada automáticamente desde el código.  
- Permite testear endpoints desde la interfaz de Swagger.  
- Facilita onboarding de nuevos desarrolladores.  
- Requiere disciplina para actualizar anotaciones.  
