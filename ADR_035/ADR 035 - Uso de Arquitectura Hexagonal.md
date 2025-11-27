# ADR 035: Uso de Arquitectura Hexagonal en Módulos Nuevos
Estado: Aceptado

## Contexto
El sistema crece y puede requerir que algunos módulos evolucionen hacia microservicios. Se requiere un diseño desacoplado y modular.

## Decisión
Adoptar arquitectura hexagonal (ports & adapters) en módulos nuevos para mejorar escalabilidad y facilidad de pruebas.

## Alternativas Consideradas
1. Arquitectura tradicional por capas.
2. Microservicios desde el inicio.

## Consecuencias
- Menor acoplamiento.
- Facilita pruebas unitarias e integración.
- Permite migración futura hacia microservicios.
