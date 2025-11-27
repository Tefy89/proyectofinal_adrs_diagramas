# ADR 049: Control de Sesiones Activas por Usuario 
**Estado:** Aceptado

## Contexto
Algunos usuarios iniciaban sesión en múltiples dispositivos, generando inseguridad.

## Decisión
Implementar control opcional de sesiones mediante:
- Lista de tokens válidos por usuario  
- Invalidación de tokens anteriores al generar uno nuevo  

## Alternativas Consideradas
1. Sin control de sesiones  
2. Almacenar sesiones en Redis  

## Consecuencias
- Mayor control administrativo  
- Seguridad reforzada  
- Aumenta el procesamiento durante login  
