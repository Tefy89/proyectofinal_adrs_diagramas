# ADR 007: Arquitectura Monolítica Modular
Decisión técnica para simplicidad inicial y escalabilidad progresiva.  
**Estado:** Aceptado  

## Contexto
El equipo es pequeño y el sistema está en fase inicial.  
Se requiere modularidad interna pero sin la complejidad de microservicios.

## Decisión
Adoptar un **monolito modular en NestJS**, con módulos independientes y capacidad de dividir en microservicios en el futuro.

## Alternativas Consideradas
- **Microservicios puros:** Complejos para un equipo pequeño.  
- **Arquitectura tradicional monolítica:** Menor modularidad.

## Consecuencias
- Desarrollo más rápido.  
- Menor complejidad de despliegue.  
- Preparado para escalar a microservicios.  
- Mayor acoplamiento inicial entre módulos.
