# ADR 010: Modularización del Backend por Dominio
Decisión técnica para organizar el código por contextos de negocio y facilitar mantenimiento.  
**Estado:** Aceptado

## Contexto
MANAGIX engloba varias áreas funcionales (Auth, Clientes, Órdenes, Inventario, Proformas, etc.). Una estructura desordenada dificulta la escalabilidad, onboarding y mantenimiento. Se necesita una organización que refleje los contextos del dominio y permita evolución independiente de cada área.

## Decisión
Organizar el backend en **módulos por dominio** (Domain Modules) en NestJS. Cada módulo contendrá:
- Controladores (API surface)
- Servicios (lógica de negocio)
- Repositorios/Entity (acceso a datos)
- DTOs y validaciones
Ejemplos de módulos: `auth`, `users`, `clients`, `orders`, `inventory`, `proformas`, `reports`.

## Alternativas Consideradas
- **Organización por tipo técnico (controllers/, services/, repositories/):** Menos clara y provoca acoplamientos entre dominios.
- **Monolito sin modularizar:** Rápido inicialmente, pero difícil de mantener.
- **Microservicios desde el inicio:** Complejo y costoso para el alcance y el equipo actual.

## Consecuencias
- Claridad en responsabilidades por dominio.  
- Facilita testing, despliegue y posible extracción a microservicios.  
- Mejora el onboarding de nuevos desarrolladores.  
- Requiere disciplina para mantener límites de responsabilidades entre módulos.
