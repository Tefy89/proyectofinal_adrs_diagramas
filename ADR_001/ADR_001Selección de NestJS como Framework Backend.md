# ADR 001: Selección de NestJS como Framework Backend
Decisión técnica para una arquitectura modular, escalable y mantenible.  
**Estado:** Aceptado  

## Contexto
Para MANAGIX se requiere un framework backend que sea escalable, mantenible y que soporte TypeScript nativamente.  
El sistema debe poder crecer con nuevos módulos (Órdenes, Proformas, Inventario, Clientes) y necesita una estructura clara basada en módulos, inyección de dependencias y organización empresarial.

## Decisión
Utilizar **NestJS** como framework principal para el backend, implementando TypeScript y arquitectura modular.

## Alternativas Consideradas
- **Express.js + TypeScript:** Flexible, pero requiere mucha configuración manual.
- **Django (Python):** Robusto, pero no ideal para aplicaciones real-time.
- **Spring Boot (Java):** Potente, pero con mayor complejidad y curva de aprendizaje.

## Consecuencias
- Arquitectura modular lista desde el inicio.  
- Inyección de dependencias integrada.  
- Soporte nativo para TypeScript.  
- Ecosistema sólido y documentación clara.  
- Mayor curva de aprendizaje comparado con Express.  
- Pequeño overhead respecto a frameworks minimalistas.
