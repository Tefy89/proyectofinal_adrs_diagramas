# ADR 037: Manejo de Pagos Simulado para Pruebas
Estado: Aceptado

## Contexto
Aunque los pagos reales no están implementados, se necesitan pruebas y simulaciones para futuros desarrollos.

## Decisión
Crear un módulo simulado de pagos con respuestas mockeadas para pruebas internas.

## Alternativas Consideradas
1. Integrar Stripe de inmediato.
2. Implementar un sistema de pagos real sin necesidad actual.

## Consecuencias
- Pruebas sin depender de servicios externos.
- Base preparada para futura integración real.
