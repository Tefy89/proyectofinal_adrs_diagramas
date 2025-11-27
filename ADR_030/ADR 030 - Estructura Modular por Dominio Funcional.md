# ADR 030: Estructura Modular por Dominio Funcional
Estado: Aceptado

## Contexto
Para mantener organizado MANAGIX, cada módulo debe corresponder a un dominio funcional (usuarios, roles, equipos, reportes, etc.). Esto evita mezclar responsabilidades y asegura que la arquitectura crezca de manera controlada conforme el sistema evolucione.

## Decisión
Adoptar arquitectura modular basada en dominios funcionales, separando cada módulo según su propósito dentro del negocio.

## Alternativas Consideradas
1. Módulos por capas técnicas (controllers, services, etc.).
2. Módulos mezclados sin separación formal por dominio.

## Consecuencias
- Separación clara entre responsabilidades.
- Facilita escalar y mantener el sistema.
- Reduce dependencias cruzadas.
