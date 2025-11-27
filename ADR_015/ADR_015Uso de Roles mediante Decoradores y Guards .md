# ADR 015: Uso de Roles mediante Decoradores y Guards 
**Estado:** Aceptado

## Contexto
El sistema incluye diferentes perfiles como Administrador y Empleado, cada uno con permisos específicos.

## Decisión
Implementar control de roles mediante decoradores **@Roles()** y **Guards personalizados**.

## Alternativas Consideradas
1. Validación manual en cada controlador.  
2. Roles almacenados en frontend.  
3. Sistema ACL externo.

## Consecuencias
- Seguridad centralizada.  
- Reducción de código repetido.  
- Fácil implementación de nuevos roles.  
