# UD5. Detección y documentación de incidentes de ciberseguridad

<p align="center">
  <img src="https://images.unsplash.com/photo-1552664730-d307ca884978?auto=format&fit=crop&w=1400&q=80" alt="Documentación y notificación de incidentes" width="100%" />
</p>

<div align="center">

![Unidad](https://img.shields.io/badge/Unidad-UD5-0A84FF?style=for-the-badge)
![Resultado](https://img.shields.io/badge/Resultado-RA5-34D399?style=for-the-badge)
![Enfoque](https://img.shields.io/badge/Enfoque-Notificación%20y%20documentación-8B5CF6?style=for-the-badge)

</div>

> La detección y la documentación son esenciales para asegurar que los incidentes no se conviertan en pérdidas ocultas. La organización debe notificar de forma adecuada, comunicar con criterio y dejar constancia de lo ocurrido para aprender y mejorar.

## 1. Introducción

La última unidad se centra en la fase final del ciclo de vida del incidente: identificar con claridad la situación, documentarla con rigor y comunicarla según corresponda. Un incidente bien documentado facilita la respuesta, el aprendizaje y la verificación del cumplimiento normativo.

Los contenidos principales son:

- detección y análisis de la notificación,
- procedimientos de notificación interna,
- comunicación a autoridades, afectados y medios,
- documentación del caso,
- cierre del incidente.

## 2. Resultado de aprendizaje y criterios

### Resultado de aprendizaje 5

Detecta y documenta incidentes de ciberseguridad siguiendo procedimientos de actuación establecidos.

### Criterios de evaluación

1. Desarrolla procedimientos de actuación para la notificación de incidentes.
2. Notifica internamente los incidentes.
3. Notifica a quienes corresponda según el tipo de incidente.

## 3. Proceso de detección y notificación

### 3.1. Detección

La detección puede venir de:

- alertas de seguridad,
- informes de usuarios,
- logs de sistemas,
- avisos del SIEM,
- anomalías de red,
- eventos físicos o de seguridad.

### 3.2. Validación inicial

Antes de notificar, debe confirmarse si el evento es un incidente real y si requiere respuesta formal.

Se debe valorar:

- nivel de impacto,
- alcance,
- criticidad del activo afectado,
- posible propagación,
- prioridad de resolución.

### 3.3. Notificación interna

La comunicación interna debe seguir una cadena clara:

- responsable inmediato,
- equipo de seguridad,
- dirección o coordinación,
- responsables de sistemas y continuidad,
- servicio legal o de cumplimiento si procede.

## 4. Tipos de notificación

### 4.1. Notificación interna

Incluye:

- descripción breve,
- impacto,
- sistema afectado,
- fecha y hora,
- evidencia,
- responsables,
- medidas iniciales adoptadas.

### 4.2. Notificación a autoridades competentes

Se activa cuando el incidente afecta a:

- datos personales,
- servicios críticos,
- seguridad de infraestructuras relevantes,
- requisitos normativos.

### 4.3. Notificación a afectados

Se comunica si existe riesgo para:

- confididencialidad,
- integridad,
- disponibilidad,
- derechos y libertades de personas afectadas.

### 4.4. Comunicación a medios

Cuando el impacto es público, institucional o de gran trascendencia, puede requerirse una estrategia de comunicación externa para gestionar la reputación y la transparencia.

## 5. Documentación del incidente

La documentación debe responder a la verdad técnica y a la trazabilidad del caso.

### Elementos recomendados

- cronología del evento,
- sistemas afectados,
- activos y datos involucrados,
- evidencias recogidas,
- decisiones tomadas,
- medidas de contención,
- medidas de recuperación,
- impacto técnico y organizativo,
- responsables,
- lecciones aprendidas.

### Plantilla de informe breve

```text
Nombre del incidente:
Fecha de detección:
Sistema afectado:
Tipo de incidente:
Impacto inicial:
Severidad:
Evidencia:
Acciones realizadas:
Notificaciones emitidas:
Estado:
Lecciones aprendidas:
```

## 6. Comunicación efectiva

### 6.1. Principios de la comunicación

- claridad,
- precisión,
- veracidad,
- tratamiento del impacto,
- respuesta oportuna,
- coordinación entre equipos.

### 6.2. Comunicación en crisis

Cuando la organización está bajo presión, la comunicación debe ser:

- breve,
- informada,
- coherente,
- adaptada al público receptor,
- centrada en medidas adoptadas y continuidad.

## 7. Casos prácticos

### Caso 1. Exposición de datos personales

Un sistema de gestión contiene información personal de empleados y clientes. Tras una revisión se confirma acceso no autorizado. El procedimiento debe incluir:

- notificación interna,
- análisis de alcance,
- notificación a la autoridad competente si procede,
- comunicación a afectados,
- revisión de controles y acceso,
- cierre del caso.

### Caso 2. Ataque de phishing masivo

Se detectan varios usuarios que han abierto correos fraudulentos. La respuesta incluye:

- notificación interna,
- bloqueo de dominios o campañas,
- revisión de credenciales comprometidas,
- aviso a responsables,
- campaña de concienciación,
- registro del incidente.

## 8. Ejercicios de consolidación

### Ejercicio 1. Reacción ante un incidente

¿Qué pasos harías para notificar un incidente de exfiltración de datos desde un servicio interno?

### Ejercicio 2. Comunicación interna

Redacta un mensaje breve para la dirección explicando qué ha ocurrido, el impacto y las medidas ya tomadas.

### Ejercicio 3. Notificación a afectados

¿Qué criterios considerarías para comunicar el incidente a personas afectadas?

### Ejercicio 4. Cierre del caso

¿Qué elementos deben aparecer en el cierre del incidente para que la organización aprenda de la situación?

## 9. Actividades recomendadas

- elaborar un protocolo de notificación interna,
- diseñar una plantilla de comunicación a afectados,
- preparar un plan de respuesta ante filtración,
- realizar una prueba de notificación a la dirección.

## 10. Resumen

La detección y la documentación son la parte final del ciclo de respuesta, pero no menos importante que la contención o la recuperación. Informar bien y registrar con rigor permite evitar dudas, cumplir requisitos y cerrar con aprendizaje real.

## 11. Recursos recomendados

- Documentación del módulo y materiales adjuntos.
- Procedimientos internos de notificación y comunicación.
- Guías de notificación de incidentes y seguridad de la información.

## 12. Autoevaluación

1. ¿Qué debe incluir una notificación interna?
2. ¿Cuándo se activa una notificación a autoridades o afectados?
3. ¿Qué es una buena documentación de incidente?
4. ¿Qué función tiene la comunicación externa?
5. ¿Por qué el cierre del caso es importante para la mejora continua?

---

<p align="center">
  <strong>La mejor respuesta no termina con la recuperación técnica: termina con una comunicación correcta y una documentación sólida.</strong>
</p>
