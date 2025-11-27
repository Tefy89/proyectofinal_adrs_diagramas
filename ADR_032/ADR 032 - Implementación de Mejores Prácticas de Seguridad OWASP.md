# ADR 032: Implementación de Mejores Prácticas de Seguridad OWASP
Estado: Aceptado

## Contexto
MANAGIX maneja datos sensibles como usuarios, credenciales y reportes internos. Es obligatorio adoptar medidas estándar de seguridad para mitigar riesgos comunes.

## Decisión
Aplicar prácticas OWASP:
- Sanitización de entradas.
- Protección contra XSS.
- Rate limiting.
- Hash seguro de contraseñas.
- Validaciones estrictas de entrada.

## Alternativas Consideradas
1. Seguridad mínima.
2. Depender únicamente del framework.

## Consecuencias
- Mayor protección contra ataques comunes.
- Aumento moderado en la complejidad de implementación.
