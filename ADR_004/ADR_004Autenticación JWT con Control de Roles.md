# ADR 004: Autenticación JWT con Control de Roles
Decisión técnica para seguridad y escalabilidad.  
**Estado:** Aceptado  

## Contexto
MANAGIX requiere autenticación segura y escalable para diferentes tipos de usuario  
(Administrador y Empleado). La solución debe funcionar en aplicaciones web y móviles.

## Decisión
Implementar autenticación con **JWT Access Token + Refresh Token**, incluyendo roles en el payload.

## Alternativas Consideradas
- **Sessions:** Simple pero no escalable para arquitecturas distribuidas.
- **OAuth2 / OpenID:** Muy robusto, pero sobredimensionado.
- **API Keys:** Poco seguro, sin control de sesión.

## Consecuencias
- Arquitectura stateless y escalable.  
- Fácil de integrar con clientes múltiples.  
- Necesidad de manejo cuidadoso de tokens.  
- Logout inmediato más complejo.
