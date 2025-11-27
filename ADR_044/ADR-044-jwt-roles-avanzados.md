# ADR 044: Uso de JSON Web Tokens con Roles Avanzados 
**Estado:** Aceptado

## Contexto
El sistema debe manejar diferentes niveles de acceso (Administrador, Empleado, Mantenimiento, Bodega, etc.). Los JWT actuales solo contienen el ID del usuario.

## Decisión
Agregar roles y permisos dentro del token, firmado con claves privadas y públicas (RS256).

## Alternativas Consideradas
1. Roles almacenados en cookies  
2. Roles validados desde base de datos en cada petición  

## Consecuencias
- Mayor seguridad y rapidez  
- Validación simplificada desde middleware  
- Dependencia de refresh tokens para actualización de roles  
