# ADR 024: Estructura del Repositorio con Monorepo Controlado
**Estado:** Aceptado

## Contexto
El sistema tiene múltiples módulos que comparten dependencias y librerías internas.  
Repositorios separados complicarían la coordinación.

## Decisión
Organizar el backend en un **monorepo estructurado**.

## Alternativas Consideradas
1. Multi-repo con repos individuales.  
2. Microservicios totalmente aislados.

## Consecuencias
- Código organizado y centralizado.  
- Mejor colaboración entre módulos.  
- Mayor simplicidad en CI/CD.
