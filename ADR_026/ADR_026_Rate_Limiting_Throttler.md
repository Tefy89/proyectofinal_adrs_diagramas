# ADR 026: Implementación de Rate Limiting para Proteger la API
**Estado:** Aceptado

## Contexto
La API será utilizada por múltiples módulos internos y potencialmente integraciones externas.  
Sin limitación de solicitudes, la API queda vulnerable a ataques de fuerza bruta, abuso, congestión y caídas del servicio.

## Decisión
Implementar **@nestjs/throttler** como sistema de rate limiting global y por rutas.

## Alternativas Consideradas
- No implementar limitación: API expuesta a abuso.  
- Control a nivel de infraestructura (Nginx, Traefik): robusto pero más complejo.  
- WAF externo (Cloudflare, AWS WAF): profesional pero costoso.

## Consecuencias
- Protección contra ataques de fuerza bruta.  
- Estabilidad bajo alta carga.  
- Prevención de consumo excesivo.  
- Implementación simple dentro del stack NestJS.
