# ADR 039: Estandarización del Formato de Respuestas API
Estado: Aceptado

## Contexto
El frontend y las integraciones externas necesitan un formato homogéneo para interpretar las respuestas.

## Decisión
Definir formato estándar:

{
"status": boolean,
"message": string,
"data": object
}


## Alternativas Consideradas
1. Respuestas distintas en cada módulo.
2. Respuestas sin estructura definida.

## Consecuencias
- Mejor comunicación entre equipos.
- Facilita el manejo de errores y depuración.
