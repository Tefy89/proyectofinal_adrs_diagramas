# ADR 016: Uso de Encriptación Bcrypt para Contraseñas 
**Estado:** Aceptado

## Contexto
Las contraseñas deben almacenarse de forma segura bajo normas modernas para evitar ataques como rainbow tables y filtraciones.

## Decisión
Utilizar **bcrypt** con sal aleatoria para hashear contraseñas.

## Alternativas Consideradas
1. Argon2 (más seguro pero más costoso)  
2. SHA256 (inseguro sin sal)  
3. Scrypt  

## Consecuencias
- Aumenta la seguridad del sistema.  
- Estándar probado ampliamente.  
- Impacto mínimo en velocidad de registro o login.  
