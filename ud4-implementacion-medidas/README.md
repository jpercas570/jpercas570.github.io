# UD5. Detección y documentación de incidentes de ciberseguridad

<p align="center">
  <img src="https://images.unsplash.com/photo-1552664730-d307ca884978?auto=format&fit=crop&w=1400&q=80" alt="Documentación y notificación de incidentes" width="100%" />
</p>

<div align="center">

![Unidad](https://img.shields.io/badge/Unidad-UD5-0A84FF?style=for-the-badge)
![Resultado](https://img.shields.io/badge/Resultado-RA5-34D399?style=for-the-badge)
![Enfoque](https://img.shields.io/badge/Enfoque-Notificación%20y%20documentación-8B5CF6?style=for-the-badge)

</div>

> La detección y la documentación son esenciales para asegurar que los incidentes no se conviertan en pérdidas ocultas. Una organización puede contener un ataque con éxito y recuperar sus servicios, pero si no documenta lo ocurrido ni comunica adecuadamente el impacto, pierde la oportunidad de aprender, mejorar sus controles y cumplir con sus obligaciones legales y regulatorias. Esta unidad aborda la fase final del ciclo de vida del incidente: la validación, la notificación, la evidencia documental y la comunicación de la respuesta.

## 1. Introducción a la unidad

La detección y documentación de incidentes de ciberseguridad constituye una de las fases más relevantes del tratamiento de un incidente, porque permite convertir la actividad técnica en información útil para la organización y para terceros. Detectar un problema es necesario, pero no suficiente: la organización debe saber qué ha ocurrido, qué impacto tiene, quién debe ser informado, qué decisiones se han tomado y qué lecciones se extraen del caso para evitar que se repita.

La fase de documentación influye directamente en la continuidad del negocio, la capacidad de coordinación interna y la nivelación de las respuestas futuras. Cuando un incidente queda bien registrado, se facilita la evaluación de riesgos, la revisión de controles, la preparación para auditorías y la posible respuesta ante reclamaciones, sanciones o conflictos legales. La documentación técnica y la comunicación eficaz no son actividades accesorias: son parte esencial del proceso de gestión de incidentes.

En esta unidad se aborda la relación entre tres dimensiones: la detección del incidente, la notificación del mismo y la documentación de la respuesta. Estas tres dimensiones están conectadas. La detección puede surgir de alertas tecnológicas, informes del personal o anomalías de negocio; la validación permite distinguir entre un evento menor y un incidente con impacto real; la notificación garantiza que los responsables adecuados conozcan la situación; y la documentación crea un registro fiable para la toma de decisiones futuras. Sin esta coordinación, la organización puede reaccionar de forma aislada, insatisfactoria o incompleta.

La gestión de incidentes de ciberseguridad no puede basarse solo en la resolución técnica del caso. La organización debe mantener un registro objetivo que permita:

- analizar la cadena de hechos;
- comunicar de forma clara el alcance del daño;
- mantener la trazabilidad de las decisiones;
- demostrar cumplimiento de procedimientos y normativas;
- preparar informes para responsables, autoridades o clientes;
- identificar qué controles fallaron y cómo corregirlos.

## 2. Resultado de aprendizaje y criterios

### Resultado de aprendizaje 5

Detecta y documenta incidentes de ciberseguridad siguiendo procedimientos de actuación establecidos.

### Criterios de evaluación

1. Desarrolla procedimientos de actuación para la notificación de incidentes.
2. Notifica internamente los incidentes.
3. Notifica a quienes corresponda según el tipo de incidente.

## 3. Proceso de detección y notificación

### 3.1. Detección

La detección del incidente puede surgir de múltiples fuentes y no siempre ocurre a través de herramientas de seguridad sofisticadas. En muchas organizaciones, la primera señal llega por el propio usuario, por un análisis del negocio o por una anomalía puntual en un sistema. Por ello, la detección debe contemplar fuentes tanto tecnológicas como humanas.

Las principales fuentes de detección incluyen:

- alertas de seguridad generadas por SIEM, EDR, firewall o antivirus;
- informes de usuarios sobre comportamientos extraños o accesos inusuales;
- registros de sistema, autenticación y red;
- cambios de configuración no previstos;
- anomalías de rendimiento o disponibilidad;
- indicadores de compromiso (IOCs) detectados por monitorización;
- eventos de seguridad física o accesos no autorizados.

La detección no solo implica “ver una alarma”, sino entender si esa alarma es relevante. En un entorno real, una señal puede corresponder a una prueba de seguridad, una regresión operativa, un problema de configuración o un incidente real. Por eso la detección debe ir acompañada de validación.

### 3.2. Validación inicial

Antes de notificar un incidente, la organización debe comprobar si el evento es real y si exige respuesta formal. Esta validación comprende varios criterios: gravedad, alcance, criticidad del activo, posibilidad de propagación y prioridad de resolución. Un incidente puede empezar como una actividad sospechosa y, tras analizar logs y evidencia, convertirse en un problema grave de seguridad.

Se debe valorar, como mínimo:

- nivel de impacto en servicios y datos;
- alcance de los activos afectados;
- criticidad del sistema o servicio involucrado;
- posible propagación lateral o persistencia;
- impacto potencial sobre continuidad del negocio;
- necesidad de notificación legal o regulatoria.

La validación inicial evita dos errores contrapuestos: la reacción excesiva ante una anomalía menor y la inacción frente a un incidente real. Una decisión bien fundada mejora la eficiencia de la respuesta y la calidad del siguiente nivel de comunicación.

### 3.3. Notificación interna

La notificación interna debe seguir una cadena clara y documentada. No debe depender de un único contacto ni de la improvisación. La estructura de notificación suele seguir una jerarquía operativa y de responsabilidad, que incluye:

- responsable inmediato del servicio o activo afectado;
- equipo de seguridad o SOC;
- dirección o coordinación de incidentes;
- responsables de sistemas y continuidad operativa;
- servicio legal, cumplimiento o privacidad, cuando se requiere;
- persona responsable de comunicación institucional externa.

La notificación interna debe ser rápida, precisa y restringida a los actores que necesitan actuar. Debe facilitar información esencial, como:

- descripción breve del problema;
- impacto inicial estimado;
- servicio o sistema comprometido;
- fecha y hora de detección;
- evidencia disponible;
- medidas adoptadas provisionalmente;
- responsables de la respuesta.

La notificación interna es especialmente importante cuando el incidente tiene implicaciones operativas, reputacionales o legales. Si no se comunica bien, la organización puede actuar con retraso o inconsistencia.

## 4. Tipos de notificación

### 4.1. Notificación interna

La notificación interna es la primera capa de la comunicación del incidente. Tiene como objetivo poner en conocimiento de las personas adecuadas la existencia de un problema, su alcance inicial y las medidas adoptadas. Debe permitir a la organización coordinar su respuesta, asumir responsabilidades y decidir el nivel de escalado necesario.

Una notificación interna bien construida suele incluir:

- descripción breve del incidente;
- impacto inicial y potencial;
- sistema o servicio afectado;
- evidencia disponible o indicios observados;
- fecha y hora de detección;
- responsables de la respuesta;
- medidas iniciales aplicadas;
- reputación o riesgo de continuidad objetivo;
- necesidades de soporte externo o de escalado.

La notificación interna debe mantenerse actualizada según evolucione el caso. Es decir, no se trata de un aviso único, sino de un flujo dinámico de información para la toma de decisiones.

### 4.2. Notificación a autoridades competentes

En algunos incidentes, la organización debe notificar a autoridades competentes. Esta obligación surge cuando se afectan datos personales, servicios críticos, infraestructuras relevantes o se incumplen requisitos normativos. La notificación puede ser obligatoria por ley o por regulación sectorial, y su ausencia puede tener consecuencias legales, sancionadoras o reputacionales.

Los casos en los que suele producirse esta notificación son los siguientes:

- exposición accidental de datos personales;
- acceso no autorizado a sistemas con información sensible;
- incidentes que afectan a servicios esenciales o infraestructuras críticas;
- brechas que implican obligaciones legales de comunicación;
- incidentes con un impacto significativo en la integridad o disponibilidad de sistemas.

El contenido de la notificación a autoridades puede variar en función del marco regulador, pero normalmente incluye el tipo de incidente, el alcance, el impacto, las medidas tomadas y la identificación de los responsables.

### 4.3. Notificación a afectados

La notificación a personas o entidades afectadas es una práctica esencial cuando el incidente supone riesgo para derechos, privacidad o seguridad. Se comunica a quienes han podido ver comprometida su información, su cuenta, su acceso o sus datos personales.

La notificación a afectados debe ser clara, serena y útil. Debe explicar, en lenguaje inteligible, qué ha ocurrido, qué riesgo existe, qué medidas se están tomando y qué puede hacer la persona afectada para protegerse. La notificación debe evitar alarmas innecesarias, pero tampoco ocultar riesgos relevantes.

Se suele activar cuando:

- se han visto comprometidos datos personales;
- se ha producido una brecha de privacidad;
- un usuario o cliente puede necesitar tomar medidas inmediatas;
- existe riesgo para la confidencialidad o seguridad de la información.

### 4.4. Comunicación a medios y a la opinión pública

En incidentes de gran relevancia, la organización puede necesitar comunicar la situación al exterior mediante note o comunicación institucional. Este tipo de comunicación se produce, por ejemplo, cuando el incidente afecta a una gran cantidad de usuarios, tiene impacto reputacional o puede afectar a la confianza pública. En ese caso, la organización debe gestionar la información con gran rigor y con una estrategia de comunicación coherente.

La comunicación externa debe:

- ser veraz y concreta;
- evitar especulaciones o afirmaciones no confirmadas;
- explicar las medidas tomadas y la situación actual;
- mantener la confianza con los afectados y con la sociedad;
- coordinarse con la dirección, seguridad y comunicación corporativa.

El error más frecuente en estas situaciones es comunicar demasiado pronto o sin suficiente evidencia. Esto genera incertidumbre y reduce la confianza en la organización.

## 5. Documentación del incidente

La documentación del incidente es una herramienta esencial para la trazabilidad, la responsabilidad y el aprendizaje. Cuando la información se documenta con rigor, la organización puede reconstruir una narrativa técnica y operativa del caso, justificar sus decisiones y preparar la mejora de sus controles.

Una documentación efectiva debe reflejar la realidad del caso y no simplemente el relato subjetivo de quienes participaron. Debe responder a la verdad técnica y a la historia de los hechos, siendo objetiva, clara y verificable.

### 5.1. Elementos recomendados en la documentación

La documentación del incidente debe incluir, al menos:

- cronología del evento;
- sistemas, servicios o activos afectados;
- impacto técnico y organizativo;
- datos o información comprometidos;
- evidencias recogidas;
- decisiones tomadas en cada fase;
- medidas de contención, erradicación y recuperación;
- responsables de cada actuación;
- notificaciones internas y externas emitidas;
- lecciones aprendidas y recomendaciones;
- cierre del caso y estado final.

Además, la documentación debe ser coherente con el análisis realizado. Una concordancia clara entre el informe, los logs, las evidencias y las decisiones sustentadas es un indicador de calidad en la gestión del incidente.

### 5.2. Plantilla de informe breve

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

Esta plantilla puede ampliarse con campos adicionales según el tipo de incidente, como “vector de ataque”, “causa raíz”, “servicios afectadas”, “riesgo residual” o “medidas de corrección”. La clave es que el documento tenga una estructura útil para la resolución y para la mejora organizativa.

### 5.3. Valor de la trazabilidad

La trazabilidad es fundamental en la documentación del incidente. Un caso bien documentado permite:

- reconstruir la secuencia cronológica de los hechos;
- justificar decisiones técnicas y de negocio;
- valorar si la respuesta fue efectiva;
- apoyar procesos de auditoría o revisión interna;
- facilitar la investigación de incidentes similares en el futuro.

El valor de una documentación sólida no es solo histórico; también sirve para la mejora en tiempo real. Si la organización no controla la trazabilidad del caso, corre el riesgo de repetir errores, perder evidencia o tomar decisiones basadas en suposiciones.

## 6. Comunicación efectiva

La comunicación es una función crítica dentro de la respuesta. Un incidente bien gestionado puede fracasar si la información no se transmite con precisión y oportunidad. La comunicación interna y externa debe cumplir ciertos criterios de calidad.

### 6.1. Principios de la comunicación

Los principios básicos de la comunicación durante un incidente son:

- claridad: sin ambigüedad ni información incompleta;
- precisión: basada en hechos y evidencia disponible;
- veracidad: evitando suposiciones o afirmaciones no contrastadas;
- oportunidad: comunicando con rapidez sin perder rigor;
- coordinación: alineando los mensajes entre áreas;
- adaptabilidad: ajustando el mensaje al destinatario.

La comunicación eficaz reduce la confusión, mejora la toma de decisiones y aumenta la confianza de los implicados.

### 6.2. Comunicación en crisis

Durante una crisis, la organización debe trabajar con mensajes breves, coordinados y consistentes. Cuando hay presión, la información que llega a la dirección, al personal y a los afectados debe ser coherente y centrada en los aspectos esenciales: qué ha pasado, qué impacto tiene, qué se está haciendo y cómo se va a gestionar la situación.

La comunicación en una crisis puede incluir:

- avisos internos a responsables y áreas afectadas;
- mensajes a usuarios o clientes afectados;
- información a medios o a autoridades, cuando procede;
- coordinación con la dirección para evitar mensajes contradictorios.

Es crucial que la organización controle su narrativa y no responda de forma emotiva o improvisada. La confianza se construye con transparencia y consistencia, no con declaraciones apresuradas.

## 7. Casos prácticos

### Caso 1. Exposición de datos personales

Un sistema de gestión contiene información personal de empleados y clientes. Tras una revisión, se confirma un acceso no autorizado. El procedimiento correcto deberá incluir:

- notificación interna inmediata;
- revisión del alcance del incidente;
- análisis de los datos implicados y de los riesgos asociados;
- notificación a la autoridad competente, si procede;
- comunicación a los afectados con información clara sobre los riesgos y las medidas de protección;
- revisión de acceso, permisos y control de seguridad;
- cierre documental del caso con lecciones aprendidas.

Este caso ilustra la necesidad de articular la respuesta técnica con la respuesta legal, regulatoria y de comunicación. En un escenario de este tipo, la velocidad de reacción puede condicionar la magnitud del impacto, pero la calidad del análisis y la transparencia de la comunicación son factores decisivos para mantener la confianza institucional y cumplir con la normativa aplicable.

### Caso 2. Ataque de phishing masivo

Se detectan varios usuarios que han abierto correos fraudulentos. La respuesta debe incluir:

- notificación interna del posible incidente;
- bloqueo de dominios, enlaces y campañas;
- revisión de credenciales y accesos comprometidos;
- documentación de los afectados directos y de la campaña;
- comunicación a responsables de seguridad y continuidad;
- formación o concienciación frente a nuevas campañas;
- registro del caso y cierre con recomendación de mejora.

Aunque el impacto inicial pueda parecer limitado, un phishing masivo puede derivar en acceso no autorizado, robo de credenciales o campañas más sofisticadas si la organización no actúa con rapidez y con una comunicación eficaz. En este tipo de incidentes, la documentación del patrón observado y la capacidad de notificar de manera coordinada pueden marcar la diferencia entre una respuesta local y una amenaza de mayor alcance.

### Caso 3. Ransomware con datos en riesgo

Una organización detecta que varios sistemas han sido cifrados por un ransomware y que existe sospecha de acceso a archivos sensibles. La fase documental y comunicativa se vuelve esencial, porque el conflicto no es solo técnico, sino también reputacional y potencialmente legal.

En este contexto, la organización debe:

- notificar rápidamente a la dirección y al equipo de respuesta;
- aislar equipos y revisar el alcance de la infección;
- valorar si se han afectado datos personales o datos de terceros;
- activar la cadena de comunicación con proveedores, autoridades o servicios relevantes;
- documentar la cronología, decisiones y dispositivos afectados;
- mantener una comunicación clara con los implicados y con la autoridad competente cuando proceda;
- registrar las medidas de recuperación y las lecciones aprendidas.

La clave de este caso es que la respuesta técnica debe acompañarse de una comunicación basada en la evidencia, un esquema de notificación apropiado y un cierre documental formal.

### Caso 4. Uso indebido de credenciales de un usuario administrativo

Un usuario con privilegios administrativos realiza accesos no habituales desde una ubicación remota y en un horario fuera de lo normal. La detección del fenómeno exige una valoración rápida del riesgo, no solo un cierre de sesión. La respuesta correcta no se limita a bloqueare la cuenta; es necesario:

- validar si hubo acceso real a recursos críticos;
- documentar el comportamiento observado;
- comunicar el caso a seguridad, decisiones y responsables de servicio;
- revisar si existieron cambios en permisos o tareas programadas;
- informar a la dirección si los activos afectados son críticos;
- preparar una nota de evolución del incidente y un cierre con recomendaciones.

Este tipo de caso ilustra que la documentación y la comunicación no son un epílogo del incidente, sino parte activa de la gestión del riesgo.

## 8. Ejercicios de consolidación

### Ejercicio 1. Reacción ante un incidente

¿Qué pasos harías para notificar un incidente de exfiltración de datos desde un servicio interno?

#### Solución orientativa

- validar la evidencia y confirmar si se ha producido un acceso no autorizado;
- comunicar el incidente al responsable relevante y al equipo de seguridad;
- aislar el servicio o restringir el acceso si procede;
- analizar el alcance, los datos afectados y el impacto;
- preparar la notificación interna y externa según corresponda;
- registrar cronología, decisiones y medidas adoptadas;
- documentar el cierre del caso y las lecciones aprendidas.

### Ejercicio 2. Comunicación interna

Redacta un mensaje breve para la dirección explicando qué ha ocurrido, el impacto y las medidas ya tomadas.

#### Solución orientativa

Debe incluir: descripción del incidente, impacto potencial, medidas iniciales adoptadas, responsables, nivel de severidad, evolución prevista y coordinación aplicada. El tono debe ser claro, objetivo y sin alarmismo.

### Ejercicio 3. Notificación a afectados

¿Qué criterios considerarías para comunicar el incidente a personas afectadas?

#### Solución orientativa

- existencia de riesgo real para datos personales o seguridad;
- sensibilidad del dato implicado;
- alcance del incidente y el número de participantes afectados;
- posibilidad de que la persona deba tomar medidas preventivas;
- necesidad legal o regulatoria de comunicarlo.

### Ejercicio 4. Cierre del caso

¿Qué elementos deben aparecer en el cierre del incidente para que la organización aprenda de la situación?

#### Solución orientativa

- resumen del caso y de la respuesta;
- causa raíz y vector;
- impacto real;
- medidas aplicadas;
- lecciones aprendidas;
- recomendación de mejora y seguimiento.

### Ejercicio 5. Evaluación del nivel de riesgo comunicativo

Explica qué criterios utilizarías para decidir si un incidente debe notificarse a la dirección, a autoridad competente, a clientes o a medios.

#### Solución orientativa

- nivel de daño potencial;
- naturaleza del dato comprometido;
- volumen de usuarios o afectados;
- impacto operativo o reputacional;
- obligaciones legales y regulatorias;
- necesidad de coordinación con terceros.

## 9. Actividades recomendadas

- elaborar un protocolo de notificación interna;
- diseñar una plantilla de comunicación a afectados;
- preparar un plan de respuesta ante filtración de datos;
- realizar una prueba de notificación a la dirección;
- comparar distintos modelos de comunicación ante crisis;
- redactar un informe de cierre de caso basado en un ejercicio práctico;
- valorar la necesidad de notificación a autoridades en función del tipo de incidente;
- practicar la redacción de mensajes de crisis para distintas audiencias.

## 10. Resumen

La detección y la documentación son la parte final del ciclo de respuesta, pero no menos importante que la contención o la recuperación. Informar bien y registrar con rigor permite evitar dudas, cumplir requisitos y cerrar con aprendizaje real. Un incidente gestionado sin documentación ni comunicación no aporta lecciones ni justifica decisiones; por eso, la evidencia y la comunicación forman parte de la propia calidad de la respuesta.

Cuando una organización aprende a documentar y comunicar adecuadamente sus incidentes, mejora su madurez en seguridad, refuerza su capacidad de respuesta y reduce el impacto de futuros sucesos. La gestión de incidentes no termina con la resolución técnica; termina con la capacidad de cerrar el caso con rigor, responsabilidad y aprendizaje.


## 11. Autoevaluación

1. ¿Qué debe incluir una notificación interna?
2. ¿Cuándo se activa una notificación a autoridades o afectados?
3. ¿Qué es una buena documentación de incidente?
4. ¿Qué función tiene la comunicación externa?
5. ¿Por qué el cierre del caso es importante para la mejora continua?
6. ¿Qué relación existe entre trazabilidad y responsabilidad organizativa?
7. ¿Por qué es necesario adaptar el mensaje a cada receptor?
8. ¿Qué elementos distinguen una comunicación efectiva de una crisis informativa?
9. ¿Qué diferencias existen entre notificar a la dirección, a afectados y a autoridades?
10. ¿Por qué una organización debería documentar tanto la respuesta técnica como la comunicación?

---

<p align="center">
  <strong>La mejor respuesta no termina con la recuperación técnica: termina con una comunicación correcta, una documentación sólida y una mejora real del sistema de seguridad.</strong>
</p>
