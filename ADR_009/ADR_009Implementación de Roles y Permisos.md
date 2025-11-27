# ADR 009: Implementación de Roles y Permisos
Decisión técnica para controlar accesos y operaciones según perfiles de usuario.  
**Estado:** Aceptado

## Contexto
MANAGIX requiere controlar con precisión qué acciones puede ejecutar cada usuario (Administrador, Empleado, etc.). Sin un sistema de roles y permisos centralizado se corre el riesgo de otorgar accesos indebidos, dificultar auditorías y duplicar lógica de autorización en múltiples controladores.

## Decisión
Establecer un sistema de **Roles y Permisos** centralizado en el backend (NestJS), implementado mediante:
- Entidades para `Role` y `Permission`.
- Relación many-to-many entre `Role` y `Permission`.
- Decoradores y Guards personalizados (`@Roles()`, `RolesGuard`) que validen el acceso a endpoints.
- Gestión administrativa de roles desde el módulo administrativo.

## Alternativas Consideradas
- **Control de acceso por usuario individual:** Gran mantenimiento y difícil de escalar.
- **Permisos codificados en controladores:** Duplicación y riesgo de errores.
- **Uso de un servicio externo de ACL:** Potente, pero agrega complejidad e infraestructura adicional.

## Consecuencias
- Centralización y consistencia en la autorización.  
- Facilidad para auditar y modificar permisos.  
- Posible aumento en la complejidad inicial de implementación.  
- Permite agregar roles nuevos sin tocar la lógica de negocio.
