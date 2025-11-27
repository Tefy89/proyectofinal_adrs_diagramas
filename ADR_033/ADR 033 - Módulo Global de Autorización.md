# ADR 033: Utilización de Módulo Global de Autorización
Estado: Aceptado

## Contexto
Los módulos del sistema requieren validaciones de permisos. Implementarlos manualmente en cada módulo genera redundancia y riesgo de inconsistencias.

## Decisión
Crear un módulo global de autorización para gestionar roles, permisos y políticas centralizadas.

## Alternativas Consideradas
1. Autorización separada por módulo.
2. Manejo de permisos dentro de cada controlador.

## Consecuencias
- Reutilización de lógica de seguridad.
- Mayor consistencia en permisos.
- Mejor mantenibilidad del código.
