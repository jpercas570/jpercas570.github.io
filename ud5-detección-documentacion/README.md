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

## Índice

- [1. Introducción a la unidad](#1-introducción-a-la-unidad)
- [2. Resultado de aprendizaje y criterios](#2-resultado-de-aprendizaje-y-criterios)
- [3. Proceso de detección y notificación](#3-proceso-de-detección-y-notificación)
  - [3.1. Detección](#31-detección)
  - [3.2. Validación inicial](#32-validación-inicial)
  - [3.3. Notificación interna](#33-notificación-interna)
- [4. Tipos de notificación](#4-tipos-de-notificación)
  - [4.1. Notificación interna](#41-notificación-interna)
  - [4.2. Notificación de incidentes: marco regulatorio, autoridades competentes y comunicación interna](#42-notificación-de-incidentes-marco-regulatorio-autoridades-competentes-y-comunicación-interna)
    - [4.2.1. Notificaciones externas](#421-notificaciones-externas)
    - [4.2.2. Notificación obligatoria asociada](#422-notificación-obligatoria-asociada)
    - [4.2.3. Notificaciones internas](#423-notificaciones-internas)
    - [4.2.4. Información a notificar](#424-información-a-notificar)
    - [4.2.5. Estrategia de comunicación](#425-estrategia-de-comunicación)
    - [4.2.6. Informes de incidentes de seguridad](#426-informes-de-incidentes-de-seguridad)
  - [4.3. Notificación a autoridades competentes](#43-notificación-a-autoridades-competentes)
  - [4.4. Notificación a afectados](#44-notificación-a-afectados)
  - [4.5. Comunicación a medios y a la opinión pública](#45-comunicación-a-medios-y-a-la-opinión-pública)
- [5. Documentación del incidente](#5-documentación-del-incidente)
- [6. Comunicación efectiva](#6-comunicación-efectiva)
- [7. Casos prácticos](#7-casos-prácticos)
- [8. Ejercicios de consolidación](#8-ejercicios-de-consolidación)
- [9. Actividades recomendadas](#9-actividades-recomendadas)
- [10. Resumen](#10-resumen)
- [11. Recursos recomendados](#11-recursos-recomendados)
- [12. Autoevaluación](#12-autoevaluación)

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

### 4.2. Notificación de incidentes: marco regulatorio, autoridades competentes y comunicación interna

En este punto se abordarán tanto las directrices para la notificación de incidentes de una organización a su autoridad competente y CSIRT de referencia, como las directrices para la notificación de incidentes desde un punto de vista interno a la organización.

#### 4.2.1. Notificaciones externas

La Guía Nacional de notificación y gestión de ciberincidentes proporciona las directrices para el cumplimiento de las obligaciones de reporte de incidentes de ciberseguridad acaecidos en el seno de las Administraciones Públicas, las infraestructuras críticas y operadores estratégicos de su competencia, así como el resto de entidades comprendidas en el ámbito de aplicación del Real Decreto-Ley 12/2018.

A continuación, se muestra un esquema acerca de autoridades competentes y CSIRT de referencia:

| Tipo de operador | Subtipo | Características | Autoridad competente | CSIRT de referencia |
|---|---|---|---|---|
| Operador de servicios esenciales | Operador crítico | CNPIC | Sector Público: CCN-CERT; Sector Privado: INCIBE-CERT | - |
| Operador de servicios esenciales | Operador no crítico | Comprendido en el ámbito de aplicación de la Ley 40/2015, de 1 de octubre, de Régimen Jurídico del Sector Público | CCN | Resto Autoridad Sectorial |
| Proveedor de Servicios Digitales | Sector Privado | - | Secretaría de Estado de Digitalización e Inteligencia Artificial | - |
| Proveedor de Servicios Digitales | Sector Público | Comprendido en el ámbito de aplicación de la Ley 40/2015, de 1 de octubre, de Régimen Jurídico del Sector Público | CCN | - |

Para la notificación de los incidentes se usará como criterio de referencia el nivel de peligrosidad que se asigne a un incidente sin perjuicio de que, a lo largo de la gestión del incidente, se categorice con un determinado nivel de impacto que haga aconsejable la comunicación del incidente a la autoridad competente o CSIRT de referencia.

En relación con los ciudadanos y empresas no incluidos en el ámbito de protección de infraestructuras críticas, del sector público, o del Real Decreto-ley 12/2018, la notificación de incidentes de ciberseguridad tendrá, en todo caso, un carácter potestativo y voluntario.

#### 4.2.2. Notificación obligatoria asociada

De acuerdo con la Guía Nacional, los incidentes cuyo nivel de peligrosidad y/o nivel de impacto sea crítico, muy alto o alto para todos aquellos sujetos obligados deberán ser notificados a su autoridad competente o CSIRT de referencia.

Como se indica en la guía, “deberán comunicar, en tiempo y forma, los incidentes que registren en sus redes y sistemas de información y estén obligados a notificar por superar los umbrales de impacto o peligrosidad establecidos en esta guía”.

Siempre que se haya producido un delito es necesario “ponerlo inmediatamente en conocimiento”, es decir, ante un posible delito se debe denunciar ante las fuerzas competentes, además de notificar al CSIRT/CERT de referencia o a la AGPD si hay datos de carácter personal. El artículo 33 del RGPD impone a los responsables de un tratamiento de datos personales la obligación de notificar a la autoridad de control competente las brechas de datos personales cuando sea probable que constituyan un riesgo para los derechos y libertades de las personas.

El responsable de tratamiento debe valorar el nivel de riesgo de una brecha de datos personales y notificarla a la autoridad de control cuando exista tal riesgo; además, cuando el riesgo sea alto, el responsable también deberá comunicar la brecha a las personas afectadas conforme al artículo 34 del RGPD.

El plazo para notificar a la autoridad de control es de 72 horas desde que la organización tiene constancia de la brecha.

En el ámbito privado, los responsables del tratamiento afectados por una brecha de datos personales deberán notificar a la AEPD:

- cuando su único establecimiento esté localizado en España;
- si tienen varios establecimientos en la Unión Europea, únicamente cuando el establecimiento principal esté localizado en España;
- si no tienen establecimiento principal en la Unión Europea, sólo en el caso de que hayan designado un representante en España;
- si no tienen establecimiento ni representante en la Unión Europea, en el caso de que la brecha de datos personales cuente con afectados en España.

#### 4.2.3. Notificaciones internas

Aunque la organización disponga de un sistema de monitorización para la detección de incidentes de seguridad, es necesario implantar canales de comunicación que permitan al personal de la organización, o a personas vinculadas a la misma de manera directa, como proveedores o colaboradores, la notificación de posibles incidentes de seguridad. Esos canales de comunicación, como correo electrónico, teléfonos de contacto, formularios web o herramientas de ticketing, deben ser ágiles, estar disponibles a través de distintos medios, estar debidamente publicitados y ser probados periódicamente para corroborar su correcto funcionamiento.

El personal deberá estar concienciado para identificar y notificar lo antes posible cualquier situación sospechosa de ser un incidente de seguridad. La velocidad con la que se reconozca, analice y responda a ese incidente limitará el daño y reducirá el coste de recuperación. Por ello, es necesario emprender acciones formativas y de concienciación dirigidas a los empleados.

#### 4.2.4. Información a notificar

Tanto en el caso de que la entidad afectada por el incidente notifique a la autoridad competente o CSIRT de referencia, como en el caso de que se realice una notificación interna en la organización, existen una serie de datos mínimos que deben aportarse de la forma más precisa posible para una correcta gestión del incidente registrado. En este punto debe tenerse presente que se prima la agilidad por encima de la completitud de la información.

Los campos esenciales suelen ser los siguientes:

- asunto: breve descripción genérica del incidente;
- descripción detallada de lo sucedido;
- fecha y hora del incidente y de su detección; indicar con la mayor precisión posible cuándo se produjo y cuándo se detectó el primer indicio;
- recursos tecnológicos afectados; aportar la mayor información técnica posible, como direcciones IP, sistemas operativos, aplicaciones, usuarios y puntos de acceso implicados;
- causa del incidente si se conoce; por ejemplo, apertura de un correo malicioso, conexión de un USB infectado, descarga de un fichero sospechoso;
- estimación del nivel de impacto; a priori es posible que sea difícil concretar el impacto ocasionado, pero es importante hacer una aproximación inicial.

Habitualmente, durante el registro de un incidente, el equipo responsable de su gestión (CERT/CSIRT/ERI) asignará a cada caso un identificador único que estará presente durante todas las comunicaciones relacionadas con el incidente. En aquellos casos en los que la comunicación se realice por correo electrónico, este identificador aparecerá en el campo “Asunto”. Este valor no debe modificarse ni eliminarse, ya que esto ralentizaría la gestión de las comunicaciones y la resolución final del ciberincidente.

Un ejemplo de comunicación, con respecto a un potencial incidente, entre un usuario de la compañía y el equipo de gestión de incidentes podría ser el siguiente:

Asunto: Correo sospechoso
De: usuario@compañia.com
Para: cert@compañia.com

Estimados compañeros. Les notifico que he recibido un correo que parecía venir del departamento de finanzas en el que se me indicaba que debía completar un formulario con una serie de información sobre mi banco e información personal. Tras completar el formulario y darle a enviar, llamé al departamento de finanzas y me indicaron que ellos no habían enviado ningún correo, lo que me hizo sospechar que pudiese ser un fraude.

Espero que me ayuden a solucionar la situación.
Saludos,

Asunto: [CERT #1234] Re: Correo sospechoso
De: cert@compañia.com
Para: usuario@compañia.com

Buenos días. Le indicamos que el equipo del CERT ha abierto un caso de investigación con identificador [CERT #1234]. En unos minutos le llamaremos para recopilar toda la información que necesitemos para completar la investigación. Mientras, por favor reenvíenos el correo recibido para iniciar las primeras acciones.
Saludos,

A partir de este punto, los analistas del CERT comenzarán a analizar la situación: revisarán el correo fraudulento recibido, si el envío de datos ha sido exitoso, qué recomendaciones debe seguir el usuario para mitigar el impacto del robo de datos, qué medidas tomar para evitar que vuelva a entrar este tipo de correos, qué acciones llevar a cabo para concienciar a este usuario para que desconfíe de este tipo de solicitudes de información, estudiar si ha habido más víctimas y valorar la necesidad de ampliar la investigación.

Otro ejemplo de un reporte de un posible incidente de seguridad puede observarse en un extracto anonimizado de un evento de seguridad que se visualiza en la consola de administración del SIEM. Como puede verse, la notificación incluye información detallada del evento, como el asunto, la fecha en la que se detectó la alerta, la criticidad asociada, las IP involucradas, el usuario implicado, el analista responsable de la investigación y el tipo del potencial incidente. Los campos sensibles han sido anonimizados por confidencialidad.

En un escenario de phishing, la notificación puede indicar el asunto “New products” en un buzón de un usuario de la compañía, y la solución antispam no ha neutralizado el mensaje. Entonces, la investigación debe centrarse en saber si el usuario ha interactuado con ese correo, qué tipo de phishing es, si lleva anexos, si incluye URL incrustadas, cuántos usuarios han podido recibir ese correo y cuánta atención precisa requiere la campaña.

#### 4.2.5. Estrategia de comunicación

Como hemos mencionado en los primeros capítulos, es necesario abordar la gestión de cada incidente de seguridad desde una perspectiva operativa y técnica, pero también desde una perspectiva organizativa y estratégica. Esto incluye evaluar cuál es la mejor estrategia de comunicación con los diferentes grupos de interés, como otras organizaciones, clientes, proveedores, empleados, sedes de la compañía, prensa o autoridades, dependiendo de la organización y del tipo de incidente.

En los incidentes más críticos es fundamental establecer una estrategia de comunicación en función del tiempo y la prioridad, y del grupo de interés al que va dirigida la comunicación: ¿qué tipo de información se va a ofrecer?, ¿cuáles son los mensajes clave?, ¿qué formato se utilizará para la difusión de la comunicación (nota de prensa, correo electrónico, vídeo, informe, etc.)?, ¿qué canales o medios se usarán (reuniones periódicas, videoconferencias, llamadas telefónicas, correos electrónicos, listas de distribución, mensajería instantánea, etc.)?

Cabe mencionar que es posible que el incidente haya provocado una denegación de servicios que se puedan plantear para comunicarse o se consideren comprometidos y no se pueda hacer uso de ellos (correo electrónico, sistema de videoconferencia, etc.). Por tanto, es necesario disponer de una alternativa segura.

Es importante que la organización sea proactiva y ágil a la hora de comunicar la situación, ya que debe tener en cuenta posibles filtraciones de información, voluntarias o no, por parte de empleados, proveedores o clientes, que puedan dar a conocer de manera incompleta o errónea lo que está sucediendo. Esto puede maximizar el impacto del propio incidente en la organización.

Los mensajes a comunicar deberían tener las siguientes características:

- ofrecer un discurso unificado y, si es posible, procedente de una única fuente oficial de información;
- transparencia, empatía y asunción de responsabilidades; nunca se debe mentir ni ofrecer información no contrastada;
- transmitir confianza, actuar con serenidad, firmeza y profesionalidad;
- demostrar atención y respeto hacia todos los involucrados;
- poner en valor las acciones adoptadas; cualquier situación de crisis representa una oportunidad para demostrar la capacidad de la organización para solventar una situación compleja.

Tal y como aconseja el CCN, se evitará mencionar, al menos inicialmente y hasta que se conozca el alcance de la situación y se valore, las causas del incidente, su responsable si lo hubiera, los datos de la investigación interna o posibles consecuencias del incidente para la organización o para otros grupos de interés.

Un ejemplo público de una buena estrategia de comunicación fue la que llevó a cabo Kaspersky cuando sus redes fueron vulneradas en 2015. Lejos de centrarse solo en el compromiso y en su parte negativa, se focalizaron en cómo habían sido capaces de detectar y estudiar en detalle una amenaza tan avanzada, proporcionando información valiosa para la comunidad de ciberseguridad y transmitiendo confianza al asegurar que sus servicios no habrían sido comprometidos. El ejemplo demuestra que la comunicación de crisis debe ser clara, meditada y orientada a reforzar la confianza institucional.

#### 4.2.6. Informes de incidentes de seguridad

Escribir un informe sobre un incidente de seguridad no es una tarea trivial, porque puede requerirse para diferentes audiencias. En general, habrá una audiencia técnica que querrá más detalles de tipo técnico, y otra de carácter directivo que necesitará un lenguaje más claro, centrado en costes, plazos e impacto en el negocio. También puede existir una audiencia legal, interesada en normativas, evidencias y cumplimiento. Por ello, la organización deberá valorar si el informe se presenta en un único documento con diferentes partes diferenciadas (resumen ejecutivo, análisis técnico y consideraciones legales), o bien en varios informes específicos dirigidos a cada audiencia.

En cualquier caso, tanto el resumen ejecutivo como las conclusiones deberán ser lo más concisos y claros posible, redactados en un lenguaje accesible y sin una excesiva carga técnica.

Una estructura básica para redactar este tipo de informes podría ser la siguiente:

1. Objeto y alcance del documento.
2. Antecedentes y consideraciones preliminares.
3. Resumen ejecutivo.
4. Análisis.
5. Conclusiones.
6. Lecciones aprendidas.
7. Anexos.
8. Referencias.

En el análisis se describirá detalladamente el trabajo realizado, incorporando información que aporte valor, como capturas de pantalla de evidencias, extractos de logs, cronología de los hechos, correos intercambiados, pruebas de concepto realizadas y cualquier otra evidencia útil. Es fundamental exponer los hechos con objetividad y demostrar que las decisiones técnicas propuestas por el equipo de respuesta tienen solvencia. Cuando se redacta el informe, conviene reforzar todas las afirmaciones con evidencia sólida y dejar claro si alguna conclusión es una hipótesis, no un hecho probado.

Este apartado puede estructurarse, por ejemplo, en subapartados como timeline del incidente, detección del incidente, medidas de contención y erradicación adoptadas, recomendaciones de seguridad y análisis forense o de malware si se han realizado.

En el punto de conclusiones se expondrán las principales deducciones del análisis. Deben ser claras, contundentes y oportunas, de manera que cualquier lector pueda comprender rápidamente qué ocurrió, cómo se gestionó y qué impacto tuvo.

En las lecciones aprendidas, la organización evaluará qué se hizo bien y qué se hizo mal durante la gestión del incidente, proponiendo acciones que permitan mejorar estos fallos. Las preguntas clave podrían ser:

- ¿Qué se gestionó adecuadamente?
- ¿Qué etapas fueron exitosas?
- ¿Qué actividades o metodologías ayudaron a lograr ese éxito?
- ¿Qué se gestionó de forma inadecuada?
- ¿Qué causas originaron el incidente y qué medidas se podrían haber implementado para evitarlo?
- ¿El ERI disponía de los medios adecuados para llevar a cabo las tareas de respuesta?
- ¿Los pasos indicados en los procedimientos de respuesta eran los correctos?
- ¿El tiempo de respuesta fue el adecuado?

Como resultado de esta etapa saldrán iniciativas que mejoren la seguridad de la compañía.

Por último, en los anexos se incluirá toda la información adicional que sustente lo redactado en los puntos anteriores, como IOCs identificados, evidencias, listados de equipos comprometidos, logs y documentación complementaria. La referencia a las fuentes internas y externas también es esencial para asegurar la trazabilidad y la solvencia del análisis.

En síntesis, la notificación y la comunicación no son actividades accesorias en la gestión del incidente; son parte integral de la respuesta, porque permiten coordinar la actuación, cumplir con obligaciones regulatorias, mantener la confianza y documentar la evolución del caso con rigor. Una organización que comunica bien y documenta con precisión es una organización que gestiona mejor su riesgo y mejora su capacidad de resiliencia.

### 4.3. Notificación a autoridades competentes

En algunos incidentes, la organización debe notificar a autoridades competentes. Esta obligación surge cuando se afectan datos personales, servicios críticos, infraestructuras relevantes o se incumplen requisitos normativos. La notificación puede ser obligatoria por ley o por regulación sectorial, y su ausencia puede tener consecuencias legales, sancionadoras o reputacionales.

Los casos en los que suele producirse esta notificación son los siguientes:

- exposición accidental de datos personales;
- acceso no autorizado a sistemas con información sensible;
- incidentes que afectan a servicios esenciales o infraestructuras críticas;
- brechas que implican obligaciones legales de comunicación;
- incidentes con un impacto significativo en la integridad o disponibilidad de sistemas.

El contenido de la notificación a autoridades puede variar en función del marco regulador, pero normalmente incluye el tipo de incidente, el alcance, el impacto, las medidas tomadas y la identificación de los responsables.

### 4.4. Notificación a afectados

La notificación a personas o entidades afectadas es una práctica esencial cuando el incidente supone riesgo para derechos, privacidad o seguridad. Se comunica a quienes han podido ver comprometida su información, su cuenta, su acceso o sus datos personales.

La notificación a afectados debe ser clara, serena y útil. Debe explicar, en lenguaje inteligible, qué ha ocurrido, qué riesgo existe, qué medidas se están tomando y qué puede hacer la persona afectada para protegerse. La notificación debe evitar alarmas innecesarias, pero tampoco ocultar riesgos relevantes.

Se suele activar cuando:

- se han visto comprometidos datos personales;
- se ha producido una brecha de privacidad;
- un usuario o cliente puede necesitar tomar medidas inmediatas;
- existe riesgo para la confidencialidad o seguridad de la información.

### 4.5. Comunicación a medios y a la opinión pública

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

## 11. Recursos recomendados

- Documentación del módulo y materiales adjuntos.
- Procedimientos internos de notificación y comunicación.
- Guías de notificación de incidentes y seguridad de la información.
- Marcos de gestión de riesgo y cumplimiento normativo en seguridad.
- Plantillas de informes de ciberincidentes y de comunicación ante crisis.
- Materiales sobre gestión de crisis y responsable corporativa.

## 12. Autoevaluación

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
