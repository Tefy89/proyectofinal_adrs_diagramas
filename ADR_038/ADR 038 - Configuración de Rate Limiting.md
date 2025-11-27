# ADR 038: Configuración de Rate Limiting
Estado: Aceptado

## Contexto
Es necesario evitar ataques de fuerza bruta, abuso de solicitudes y saturación de la API.

## Decisión
Implementar rate limiting global mediante ThrottlerModule de NestJS.

## Alternativas Consideradas
1. Sin límites de petición.
2. Reglas manuales por ruta.

## Consecuencias
- Mejor protección ante abuso.
- Prevención de saturación del servicio.
