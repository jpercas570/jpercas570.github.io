---
title: UD3 - Investigación del incidente
layout: default
---

# UD3. Investigación del incidente

> La investigación permite pasar de la sospecha a la comprensión: qué ocurrió, cómo ocurrió, qué impacto tuvo y qué medidas deben adoptarse.

## 1. Resultado de aprendizaje

Investiga incidentes de ciberseguridad analizando los riesgos implicados y definiendo posibles medidas de actuación.

### Criterios

- Recopila y custodia evidencias.
- Analiza pruebas y reconstruye el incidente.
- Intercambia información con proveedores y organismos.
- Aplica medidas de contención.

## 2. Evidencia digital

La evidencia debe preservarse de forma íntegra. Los elementos clave son:

- logs y trazas,
- memoria RAM,
- archivos y hashes,
- tráfico capturado en red,
- registros de firewall,
- autenticación y eventos de acceso,
- dispositivos afectados.

## 3. Cadena de custodia

La evidencia debe registrarse con:

- autor,
- fecha y hora,
- tipo de evidencia,
- procedimiento de obtención,
- persona responsable,
- almacenamiento y protección.

## 4. Análisis forense

Se investiga:

- procesos,
- conexiones,
- archivos ejecutables,
- cambios en la configuración,
- comportamiento del malware,
- rutas de acceso y persistencia.

## 5. Intercambio de información

Cuando el incidente afecta a terceros o a infraestructuras compartidas, suele ser recomendable intercambiar indicadores de compromiso y trazas con proveedores, organismos y equipos internos.

## 6. Contención

Se aíslan equipos, se bloquean rutas de propagación y se reducen riesgos antes de continuar con la recuperación.

## 7. Ejemplo práctico

Si un equipo presenta procesos sospechosos y conexiones a dominios no autorizados, se aisla el equipo, se preserva la evidencia, se extraen hashes y luego se decide si se elimina o se restaura desde una imagen limpia.

## 8. Resumen

La investigación del incidente permite entender la amenaza, evitar su repetición y decidir las medidas más eficaces de contención y recuperación.

- [Apuntes completos](../../ud3-investigacion-incidente/README.md)
- [Volver al módulo](../)
