# ADR 034: Definición de un Pipeline de Testing Automatizado
Estado: Aceptado

## Contexto
Para mantener calidad y estabilidad, los módulos deben contar con pruebas automáticas que garanticen su correcto funcionamiento en cada cambio.

## Decisión
Configurar Jest como herramienta principal de pruebas y ejecutarlo automáticamente mediante GitHub Actions.

## Alternativas Consideradas
1. Mocha.
2. Jasmine.

## Consecuencias
- Mayor calidad y estabilidad del código.
- Detección temprana de errores antes de llegar a producción.
