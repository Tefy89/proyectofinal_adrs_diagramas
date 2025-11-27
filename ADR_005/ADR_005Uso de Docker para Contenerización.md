# ADR 005: Uso de Docker para Contenerización
Decisión técnica para despliegues reproducibles y aislados.  
**Estado:** Aceptado  

## Contexto
El proyecto debe desplegarse de forma estandarizada en distintos entornos.  
La contenerización simplifica el mantenimiento, actualizaciones y portabilidad.

## Decisión
Utilizar **Docker** para empaquetar el backend, frontend y base de datos.

## Alternativas Consideradas
- **Instalación manual en servidor:** Propensa a errores.
- **Máquinas virtuales completas:** Más pesadas y lentas.
- **Podman:** Alternativa interesante, pero menos estándar.

## Consecuencias
- Misma configuración en todos los entornos.  
- Aislamiento entre servicios.  
- Autodependencias explícitas.  
- Requiere aprendizaje básico de Docker.
