# UD3. Investigación del incidente

<p align="center">
  <img src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?auto=format&fit=crop&w=1400&q=80" alt="Investigación forense de incidentes" width="100%" />
</p>

<div align="center">

![Unidad](https://img.shields.io/badge/Unidad-UD3-0A84FF?style=for-the-badge)
![Resultado](https://img.shields.io/badge/Resultado-RA3-34D399?style=for-the-badge)
![Enfoque](https://img.shields.io/badge/Enfoque-Investigación%20forense-8B5CF6?style=for-the-badge)

</div>

> La investigación del incidente constituye la fase analítica y técnica del tratamiento de un evento de seguridad. Una vez se ha detectado y validado una anomalía o un ataque, la organización debe determinar qué ocurrió, por qué ocurrió, qué impacto tuvo, qué activos se vieron afectados y qué medidas deben adoptarse para evitar recurrencia. En este sentido, la investigación no es un acto meramente documental ni descriptivo; es un proceso de análisis metodológico, orientado a la construcción de una narrativa técnica y legalmente defendible de los hechos.

## Índice

- [1. Introducción a la unidad](#1-introducción-a-la-unidad)
- [2. Resultado de aprendizaje y criterios](#2-resultado-de-aprendizaje-y-criterios)
- [3. Principios fundamentales de la investigación](#3-principios-fundamentales-de-la-investigación)
- [4. Fases de la investigación del incidente](#4-fases-de-la-investigación-del-incidente)
- [5. Recopilación de evidencias](#5-recopilación-de-evidencias)
- [6. Técnicas y herramientas de análisis](#6-técnicas-y-herramientas-de-análisis)
- [7. Métodos de investigación](#7-métodos-de-investigación)
- [8. Investigación forense aplicada a distintos tipos de evidencia](#8-investigación-forense-aplicada-a-distintos-tipos-de-evidencia)
- [9. Intercambio de información](#9-intercambio-de-información)
- [10. Contención, erradicación y recuperación](#10-contención-erradicación-y-recuperación)
- [11. Ejemplos prácticos](#11-ejemplos-prácticos)
- [12. Ejercicios de consolidación](#12-ejercicios-de-consolidación)
- [13. Actividades prácticas recomendadas](#13-actividades-prácticas-recomendadas)
- [14. Resumen](#14-resumen)
- [15. Recursos recomendados](#15-recursos-recomendados)
- [16. Autoevaluación](#16-autoevaluación)

## 1. Introducción a la unidad

La investigación del incidente constituye una de las funciones esenciales dentro de la gestión de la seguridad de la información. Su finalidad no es únicamente confirmar la existencia de una anomalía o de una amenaza, sino reconstruir el conjunto de hechos, determinar la causa raíz, medir el impacto operativo y técnico, y servir de base para la adopción de medidas eficaces de contención, erradicación, recuperación y mejora continua. Desde una perspectiva metodológica, se trata de un proceso analítico, documental y forense que convierte una alarma en conocimiento accionable para la organización.

La investigación del incidente se sitúa en la intersección entre la seguridad operativa, la ciencia forense digital, la gestión de riesgos y la continuidad del negocio. En términos prácticos, implica distinguir entre señales de alarma, ruido operacional y evidencia válida; entre un problema funcional y un incidente de seguridad; entre una anomalía aislada y una campaña maliciosa con impacto real. Esta diferencia exige un enfoque riguroso, basado en la correlación de fuentes, la validación de hypotheses y la preservación de la evidencia.

La disciplina se apoya en una serie de principios metodológicos que la convierten en una actividad técnica y académicamente sólida: preservación de la evidencia, trazabilidad, confidencialidad, integridad, orden de volatilidad, necesidad y proporcionalidad, y documentación formal del proceso. La evidencia debe mantenerse inalterada desde su recogida hasta su análisis; cualquier acción indebida puede comprometer la validez del caso, la reconstrucción cronológica y la defensa de la decisión organizativa. Por ello, la investigación forense digital se fundamenta en procedimientos que priorizan la captura segura de datos, la documentación de la cadena de custodia y la minimización del riesgo de contaminación del escenario.

En la práctica profesional, la investigación del incidente se desarrollará alrededor de varios ejes fundamentales:

- recopilación segura de evidencias;
- análisis forense de sistemas, redes, endpoints y servicios;
- reconstrucción cronológica y correlación de eventos;
- identificación de la causa raíz y del vector de ataque;
- intercambio de información con terceros, proveedores y organismos competentes;
- definición de medidas de contención, erradicación y recuperación;
- elaboración de informes técnicos y de lecciones aprendidas.

Desde un enfoque universitario y profesional, la investigación del incidente no puede entenderse como una respuesta improvisada ni como un conjunto de acciones aisladas. Se trata de un proceso estructurado, basado en evidencias, compatible con el marco regulatorio y orientado a la mejora del nivel de madurez de seguridad. En organizaciones complejas, esta capacidad es un componente esencial del control interno, la continuidad del negocio, la gestión del riesgo y la preparación frente a incidentes de alta severidad.

## 2. Resultado de aprendizaje y criterios

### Resultado de aprendizaje 3

Investiga incidentes de ciberseguridad analizando los riesgos implicados y definiendo las posibles medidas a adoptar.

### Criterios de evaluación

1. Recopila y almacena evidencias de forma segura.
2. Analiza evidencias e investiga el incidente.
3. Intercambia información del incidente con proveedores u organismos competentes.
4. Aplica medidas de contención del incidente.

## 3. Principios fundamentales de la investigación

### 3.1. Concepto de investigación del incidente

La investigación del incidente es el conjunto de actividades técnicas, analíticas, documentales y decisionales orientadas a responder preguntas esenciales sobre un suceso de seguridad. En la práctica, permite responder a interrogantes como: ¿qué ocurrió?, ¿cuándo ocurrió?, ¿cómo se produjo?, ¿qué activos o personas se vieron implicadas?, ¿qué fallo o vulnerabilidad permitió la acción?, ¿qué impacto tuvo?, ¿qué medidas deben adoptarse y con qué prioridad? La respuesta a estas cuestiones no solo permite mitigar el daño inmediato, sino también aprender de la experiencia y reducir la probabilidad de recurrencia.

El propósito de la investigación no es únicamente describir la secuencia de los hechos, sino explicar la relación causal entre la acción del atacante, la vulnerabilidad explotada y el impacto operativo o reputacional. En este sentido, no basta con formular una hipótesis intuitiva basada en una alerta; el analista debe contrastarla con evidencia, reconstruir la cronología y validar las conclusiones antes de presentar una explicación definitiva. Una investigación correcta debe generar conocimiento accionable, no únicamente un informe descriptivo o un conjunto de observaciones aisladas.

Además, la investigación tiene un carácter eminentemente profesional. Debe respetar las normas de integridad, confidencialidad y trazabilidad, y debe estar alineada con las capacidades reales de la organización. En muchos casos, la investigación no solo responde a una necesidad técnica, sino a una necesidad de gestión del riesgo, continuidad del negocio y responsabilidad institucional.

### 3.2. Integridad de la evidencia

La evidencia es el elemento central de una investigación. Sin evidencia sólida, las conclusiones pueden ser especulativas, contradictorias o no admisibles en un contexto formal. La integridad de la evidencia hace referencia a la necesidad de mantenerla inalterada desde su recogida hasta su análisis final, salvo las manipulaciones técnicas necesarias para extraer datos sin modificar el contenido original.

Esto implica evitar cambios accidentales en archivos, logs, memoria o configuración del sistema. Un solo cambio puede destruir la posibilidad de reconstruir el origen del incidente. En el análisis forense, se aplican técnicas de cálculo de hashes, copias bit a bit, montajes de lectura únicamente y aislamiento del entorno para asegurar que la evidencia mantiene su exactitud.

Un ejemplo claro es la investigación de un equipo comprometido: si se revisa directamente el disco del sistema infectado sin realizar una imagen forense, puede producirse una alteración del contenido de los archivos, marcadores temporales o metadatos que dificulta la reconstrucción del caso. Por ello, la práctica correcta exige preservar la evidencia, documentar cada acción realizada y controlar quién accede a ella.

### 3.3. Cadena de custodia

La cadena de custodia es el registro documental y secuencial de la posesión, manipulación, traslado y análisis de la evidencia. Este registro debe incluir información esencial sobre la identidad de la persona que la ha recogido, la fecha y hora de la recogida, el lugar en el que se encontró, la razón de su obtención, el tipo de medio, el identificador de la evidencia, las personas que la han manejado y las razones por las que se ha movido o extraído información.

La cadena de custodia es crucial porque permite demostrar que el material analizado es el mismo que fue recogido inicialmente y que no se ha contaminado ni manipulado de forma arbitraria. En contextos internos, esta práctica permite defender las decisiones tomadas por la organización y sustentar los informes. En contextos externos, técnicos o legales, puede ser un requisito esencial para que la evidencia sea admisible o útil en una acción jurídica o disciplinaria.

La cadena de custodia no es un formalismo vacío: es una prueba de rigor. Si no existe control sobre quién ha tenido acceso a la evidencia, no puede asegurarse la fiabilidad del análisis ni la validez de las conclusiones. En la práctica, se suele usar un registro físico o digital con un identificador único para cada elemento, acompañado de firma, fecha, lista de acceso y propósito del análisis.

### 3.4. Orden de volatilidad

La evidencia digital no tiene el mismo grado de persistencia ni valor analítico. Algunas fuentes de información desaparecen o cambian de forma casi inmediata si no se capturan oportunamente. Por este motivo, se aplica el principio del orden de volatilidad, que prioriza la recolección de datos más volátiles antes que los de mayor persistencia.

El orden de volatilidad habitual es el siguiente:

1. memoria RAM;
2. conexiones activas y procesos en ejecución;
3. cachés de sistema y archivos temporales;
4. registros de sistema y logs en memoria;
5. almacenamiento de disco;
6. copias de seguridad;
7. evidencia física secundaria o de larga duración.

La memoria RAM puede almacenar credenciales, cadenas de ejecución, archivos en uso, comandos ejecutados, tráfico activo y artefactos de malware que desaparecen muy pronto. Si se analiza primero el disco duro, se corre el riesgo de perder información crítica que ya no estará en memoria. Por este motivo, las herramientas forenses suelen comenzar con la captura del estado vivo del sistema o del entorno, antes de desconectar o congelar el equipo.

### 3.5. No contaminación y aislamiento

Durante una investigación, se debe evitar toda acción que altere el escenario original. Esto es especialmente importante cuando el equipo está comprometido o cuando los datos pueden ser modificados por el atacante. La no contaminación implica no cerrar procesos sin documentar la acción, no ejecutar comandos de diagnóstico sobre un sistema sospechoso si esto puede destruir evidencia, no borrar archivos sin tener una justificación técnica y no conectar equipos infectados a redes sin aislamiento.

El aislamiento del entorno es una medida esencial. Si un equipo infectado conserva conectividad a la red, el atacante puede continuar sus acciones, borrar artefactos o propagar la amenaza. El aislamiento debe hacerse de forma controlada, con registro y con atención a la preservación de la evidencia. Aun así, la desconexión de una máquina puede alterar parte de la evidencia de red o volátil, por lo que siempre debe decidirse según el tipo de caso y la estrategia analítica.

### 3.6. Relación entre investigación y respuesta al incidente

La investigación del incidente no es un proceso completamente independiente de la respuesta. De hecho, ambas actividades se solapan y se retroalimentan. Durante la contención puede ser necesario realizar ciertos análisis rápidos para detectar el alcance del problema. Durante la investigación, se puede descubrir que la amenaza aún está activa y requiere nuevos cierres de acceso o desconexiones. En este sentido, no existe una frontera clara entre la fase de identificación y la de resolución: el analista trabaja bajo una lógica de evidencia, prioridad y riesgo.

La investigación ayuda a decidir qué tipo de contención es necesaria: aislamiento de host, bloqueo de cuentas, deshabilitación de servicios, restricción de tráfico, validación de permisos, eliminación de persistencia, restauración de sistemas o preparación de a prueba de concepto para la recuperación. La forma de responder depende en gran medida de la causa raíz y del impacto real o potencial; por eso, la naturaleza técnica de la investigación es un eje determinante del éxito global del manejo del incidente.

## 4. Fases de la investigación del incidente

La investigación de un incidente suele desarrollarse en una secuencia lógica que permite reconstruir la secuencia de los hechos y tomar decisiones de forma consistente. Aunque el detalle varía según el tipo de incidente, la mayoría de los casos siguen una estructura común.

```mermaid
flowchart LR
A[Detección y validación] --> B[Preservación de evidencia]
B --> C[Recopilación]
C --> D[Análisis técnico]
D --> E[Determinación de causa raíz]
E --> F[Contención y recuperación]
F --> G[Documentación y cierre]
```

### 4.1. Detección y validación

La fase inicial consiste en confirmar que se ha producido una anomalía relevante. Esto no siempre significa que exista un ataque confirmado; a veces se trata de una actividad sospechosa que aún necesita validación. El analista debe determinar si la señal es realmente un incidente, si resulta de una prueba de seguridad, de una mala configuración, de un fallo del sistema o de un comportamiento legítimo de usuario.

La validación implica contrastar la información procedente de distintas fuentes: EDR, SIEM, firewall, antivirus, logs de autenticación, tráfico de red o alertas del sistema. Si la alerta se confirma, se inicia la investigación formal.

### 4.2. Preservación de evidencia

Una vez validado el incidente, se debe proteger la prueba antes de intervenir. Esto incluye congelar entornos, crear imágenes forenses, guardar logs, exportar metadatos y documentar cualquier acción. La preservación debe ser inmediata y cuidadosa, con una prioridad clara según el orden de volatilidad.

### 4.3. Recogida de evidencias

Esta fase consiste en obtener la mayor cantidad posible de datos útiles sin alterar el origen. La evidencia se captura desde distintas dimensiones: endpoints, red, identidad, autenticación, aplicaciones y entorno físico. La calidad de la recolección determina la capacidad de establecer la cronología de los hechos y la relación de causa y efecto.

### 4.4. Análisis técnico

Cuando ya se dispone de la evidencia, se estudian los artefactos: archivos, procesos, conexiones, hashes, logs, tokens, cronjobs, permisos, ficheros temporales, tráfico, mensajes de correo, etc. Aquí es donde se examina la conducta del atacante, se correlacionan los eventos y se construye una narrativa razonada del incidente.

### 4.5. Determinación de causa raíz

La causa raíz no es simplemente “qué fue lo que se vio”, sino qué combinación de factores permitieron que el incidente ocurriera. Puede incluir una contraseña débil, una vulnerabilidad no parcheada, un software con fallos, una configuración insegura, un usuario con permisos excesivos, un phishing exitoso o un proceso de autenticación débil. La causa raíz permite corregir la vulnerabilidad real, no solo el síntoma.

### 4.6. Contención y recuperación

Una vez comprendido el problema, se toman medidas para limitar el daño y recuperar la normalidad operativa. La contención puede consistir en aislar máquinas, cerrar cuentas, bloquear tráfico, deshabilitar servicios o cambiar políticas de acceso. La recuperación implica restaurar sistemas, validar la integridad, comprobar servicios y confirmar que ya no queda actividad maliciosa.

### 4.7. Documentación y cierre

La investigación concluye con un informe técnico que documenta los hechos, los análisis, las decisiones adoptadas y las lecciones aprendidas. Este documento es fundamental para la mejora del plan de continuidad, la revisión de controles y la preparación ante futuros incidentes.

## 5. Recopilación de evidencias

La recogida de evidencias constituye la base del trabajo analítico. No basta con observar una alerta; es necesario obtener los datos que permitan reconstruir el incidente y evaluarlo de manera objetiva. Dependiendo del tipo de amenaza, la evidencia puede provenir de múltiples fuentes, cada una con un valor distinto.

### 5.1. Evidencias de red

La evidencia de red permite visualizar la actividad de comunicación entre hosts y servicios. En muchos incidentes, esta capa ofrece pruebas importantes sobre el origen del ataque, la ubicación geográfica, los patrones de tráfico, las conexiones a dominios sospechosos y los intentos de exfiltración.

Entre las fuentes más habituales se incluyen:

- flujos de red y paquetes capturados (PCAP);
- logs de firewall y proxies;
- registros de DNS y resolución de nombres;
- registros de VPN o acceso remoto;
- trazas de tráfico saliente e interno;
- conexiones a puertos y servicios no habituales;
- patrones de transferencia de datos sospechosos.

Un PCAP, por ejemplo, puede revelar que un equipo comprometido estableció una conexión a una IP externa en una hora concreta, realizó transferencia de datos o descargó un comando malicioso. Las evidencias de red ayudan a identificar la infraestructura de ataque y a detectar actividades de exfiltración, beaconing o exfiltración a servicios de nube.

### 5.2. Evidencias de sistema

Los sistemas operativos generan una gran cantidad de información útil para la investigación: eventos de inicio de sesión, cambios de configuración, creación de usuarios, instalación de software, ejecución de procesos y errores del sistema. Estas evidencias permiten relacionar la actividad maliciosa con cambios o estados específicos del entorno.

Entre los indicadores más relevantes destacan:

- hashes de archivos;
- registros del sistema operativo;
- servicios activos e iniciados;
- cuentas creadas o modificadas;
- cambios en permisos y grupos;
- tareas programadas o cronjobs;
- eventos de arranque y apagado;
- registros de seguridad y de auditoría.

Los análisis de integridad y de cambios de configuración permiten detectar si un atacante ha añadido una cuenta administrativa, modificado un servicio crítico o ejecutado un script en el arranque del sistema. Esto es especialmente importante en ataques de persistencia.

### 5.3. Evidencias de endpoint

Los endpoints son objetivos habituales de malware, acceso no autorizado y manipulación. El análisis del endpoint ofrece información sobre la actividad del usuario, los procesos ejecutados, la red involucrada y las herramientas usadas. Un equipo comprometido puede contener artefactos técnicos de gran valor para la investigación, como archivos ejecutables, scripts, DLLs, accesos a recursos compartidos o rutinas de persistencia.

Las evidencias más habituales son:

- procesos activos;
- artefactos de ejecución y persistencia;
- tareas programadas;
- conexiones de red abiertas;
- archivos ejecutables y librerías cargadas;
- cambios en el registro del sistema;
- antivirus o EDR con alertas;
- listas de procesos, servicios y autoruns.

La investigación de un endpoint puede revelar que un usuario introdujo un archivo descargado desde un correo sospechoso o que una herramienta de administración fue ejecutada de forma no autorizada con privilegios elevados. Esto permite reconstruir la secuencia del ataque y valorar el impacto real.

### 5.4. Evidencias de aplicaciones y servicios

Los servicios y aplicaciones también generan representaciones de la actividad que pueden aportar claves sobre el incidente. Esto incluye registros de autenticación, logs de acceso a aplicaciones, trazas de errores, cambios en bases de datos, actividad de API, carga de archivos y operaciones sobre documentos sensibles.

En una investigación relacionada con una fuga de información, puede ser crucial revisar:

- accesos a documentos sensibles;
- cambios en la base de datos;
- limpiezas de evidencia o logs;
- trazas de autenticación y tokens;
- movimientos de usuarios y permisos;
- actividad de servicios y cronjobs;
- cambios en configuración de la aplicación.

Estas evidencias permiten relacionar un incidente con un servicio concreto, un usuario o una integración específica. El análisis de aplicaciones es especialmente relevante cuando el impacto no se limita a la infraestructura, sino que recae sobre activos de negocio o registros empresariales.

### 5.5. Evidencias de seguridad física

Aunque la investigación del incidente suele centrarse en la dimensión digital, la seguridad física también puede ser relevante. Un incidente digital puede iniciarse o aprovecharse a partir de accesos físicos no autorizados, vehículos, dispositivos robados o accesos a salas técnicas. En algunos casos, la evidencia física permite determinar la causa del incidente o confirmar su origen.

Entre los elementos físicos de interés destacan:

- registro de accesos a instalaciones;
- grabaciones de cámaras;
- equipos reportados como perdidos o robados;
- presencia de periféricos no autorizados;
- uso de USB o almacenamiento externo;
- presencia de dispositivos a la vista de pantallas o documentos sensibles.

Esto es especialmente importante en casos de espionaje industrial, exfiltración de información por medios físicos o manipulación de equipos en entornos no supervisados.

## 6. Técnicas y herramientas de análisis

El análisis forense de incidentes combina estrategia, procedimientos y herramientas especializadas. El objetivo es convertir la evidencia bruta en información interpretable, útil para reconstruir la secuencia de hechos y evaluar las consecuencias.

### 6.1. Herramientas de análisis forense

La práctica profesional utiliza un conjunto amplio de herramientas, que pueden dividirse en varias categorías:

- capturas y análisis de red: Wireshark, tcpdump, Zeek;
- análisis forense de disco: Autopsy, EnCase, FTK Imager, Sleuth Kit;
- análisis de memoria: Volatility, Rekall;
- extracción de artefactos: Strings, binwalk, exiftool;
- validación de integridad: MD5, SHA256, hashdeep;
- análisis de procesos y rendimiento: Sysinternals Suite, OSQuery;
- análisis de malware: YARA, sandboxes, análisis estático y dinámico;
- monitorización y correlación: Elastic SIEM, Splunk, QRadar.

Estas herramientas no sustituyen el criterio del analista; sirven como apoyo para extraer, validar y correlacionar evidencias. El valor real del análisis depende de la comprensión del contexto del sistema, la comprensión del comportamiento del atacante y la capacidad de reconocer patrones relevantes.

### 6.2. Hashing e integridad de la evidencia

El hashing es un procedimiento fundamental dentro del análisis forense. Consiste en generar un valor criptográfico de un archivo o un conjunto de datos, de modo que cada cambio introducido en ese contenido modifique el hash. Por ejemplo, si se genera el hash SHA-256 de un archivo sospechoso al comienzo de la investigación, se puede comprobar después si el archivo sigue siendo el mismo.

Ejemplo:

```bash
sha256sum archivo_sospechoso.bin
```

Este cálculo se usa para verificar la integridad de archivos, capturas de imagen, paquetes, documentos y archivos de evidencia. También permite confirmar si un artefacto ha sido alterado durante la investigación o la transferencia entre equipos.

### 6.3. Análisis de memoria

La memoria RAM es una de las fuentes de evidencia más valiosas en un incidente activo. Puede contener procesos en ejecución, credenciales cargadas, DLLs, conexiones activas, comandos usados por usuarios o atacantes, listas de archivos abiertos y artefactos de malware. En muchos ataques avanzados, la memoria es la única fuente que revela la actividad reciente que no ha quedado persistida en disco.

El análisis de memoria permite identificar:

- procesos ejecutados recientemente;
- credenciales y tokens activos;
- conexiones de red abiertas;
- scripts, payloads o cargas maliciosas en ejecución;
- artefactos ocultos no visibles en disco;
- indicadores de persistencia o ejecución de comandos.

Sin embargo, la memoria es volátil y puede cambiar con rapidez. Por eso, debe capturarse lo antes posible y se debe realizar una vez asegurada la preservación del sistema.

### 6.4. Análisis del disco y artefactos forenses

El análisis de disco permite detectar archivos, metadatos, entradas en registros, cambios de sistema, temporales, archivos eliminados y patrones de persistencia. Un atacante rara vez se queda solo con una carga ejecutable visible; suele dejar trazas como:

- registro de ejecución;
- cambios en la configuración de arranque;
- entidades relacionadas con servicios o tareas programadas;
- archivos en directorios temporales;
- scripts o payloads ocultos en la carpeta de usuario;
- archivos comprimidos, autocopias o herramientas de post-explotación.

La investigación del entorno de archivos es imprescindible para distinguir entre un incidente puntual y un ejercicio de persistencia prolongada. Un atacante puede haber entrado en una máquina y dejado herramientas para mantenerse activo durante semanas; por eso, la evidencia del disco debe analizarse cuidadosamente.

## 7. Métodos de investigación

La investigación del incidente se apoya en métodos analíticos que permiten reconstruir la cronología, determinar causalidad y distinguir lo relevante de lo incidental. Estos métodos son la base para elaborar informes sólidos y tomar decisiones basadas en evidencia.

### 7.1. Análisis de causa raíz

La causa raíz responde a la pregunta de por qué ocurrió el incidente. No basta con afirmar que hubo malware o un acceso no autorizado; se debe explicar qué vulnerabilidad o fallo hizo posible el ataque. En ese sentido, la causa raíz puede ser técnica, organizativa, humana o procedimental.

Se busca responder a cuestiones como:

- ¿Qué ocurrió exactamente?
- ¿Cómo entró el atacante?
- ¿Qué objetivo tenía?
- ¿Qué herramientas usó?
- ¿Qué impacto tuvo?
- ¿Qué controles fallaron?
- ¿Qué medidas de mitigación resultan insuficientes o inexistentes?

El análisis de causa raíz exige ir más allá del síntoma. Si un ransomware afecta a una empresa, la causa raíz puede no ser solo la ejecución del ransomware, sino la falta de segmentación de red, una política débil de copias de seguridad, un acceso remoto no reforzado o un fallo de parcheo. Solo identificando la causa se puede actuar con eficacia a largo plazo.

### 7.2. Línea temporal o timeline

La línea temporal organiza los eventos en orden cronológico para reconstruir el desarrollo del incidente. Esta práctica es esencial porque permite relacionar acciones realizadas por el atacante, cambios técnicos, alertas del sistema y respuestas internas.

Un ejemplo básico sería:

| Fecha/hora | Evento | Evidencia | Observación |
| --- | --- | --- | --- |
| 08:10 | Acceso anómalo | Log de VPN | IP no reconocida |
| 08:14 | Elevación de privilegios | Seguridad del sistema | Cambio de rol |
| 08:18 | Ejecución de script | Endpoint log | Artefacto sospechoso |
| 08:22 | Cifrado de archivos | EDR | Indicador de ransomware |

La construcción de la timeline permite ver si la actividad maliciosa se produjo antes o después de una alarma, si hubo registros de exfiltración o si la contención se realizó a tiempo. Además, la cronología facilita la comparación con otras fuentes de evidencia y ayuda a detectar lagunas en la vigilancia.

### 7.3. Correlación de eventos

La correlación es un proceso clave en la investigación. Un solo evento puede ser irrelevante; sin embargo, al conectarlo con otros datos se vuelve significativo. Por ejemplo, un acceso fallido a una cuenta aislado puede ser un ruido, pero si coincide con un aumento de actividad de autenticación, una IP externa no habitual, una ventana de tiempo rara y un cambio de permisos, la conclusión cambia por completo.

Esto exige combinar fuentes de información para obtener un panorama contextual. La seguridad operativa no se basa en la lectura de un único log, sino en la capacidad de correlacionar eventos y entender la lógica del comportamiento del sistema. El analista debe ser capaz de distinguir entre causalidad real y coincidencia temporal.

### 7.4. Análisis de persistencia y lateralización

En incidentes avanzados, el atacante no suele limitarse a una máquina. Puede intentar mantener acceso, ampliar su presencia en la red, obtener credenciales para otros sistemas y mover lateralmente. Por ello, la investigación debe contemplar:

- persistencia en inicio de sesión o tareas programadas;
- uso de herramientas administrativas o scripts ocultos;
- cambios en cuentas de servicio;
- creación de cuentas de usuario o privilegios;
- acceso a máquinas adyacentes;
- uso de tokens o credenciales en otros servicios.

La detección de persistencia es crítica, porque un ataque puede haber sido contenido en apariencia, pero la amenaza podría seguir activa si no se elimina la puerta de acceso o el mecanismo de ejecución automática.

### 7.5. Análisis de indicadores de compromiso (IOCs)

Los IOCs son artefactos o señales que permiten identificar la actividad de un atacante. Pueden ser direcciones IP, dominios, hashes, nombres de archivo, técnicas de malware, cadenas de referencia, patrones de correo y firmas de comportamiento. La utilidad de los IOCs radica en que permiten buscar confirmación en diferentes partes del entorno y detectar si la amenaza se ha propagado o si ya había existido montaje previo.

Los IOCs no son solo una herramienta de detección: también son evidencia de investigación. Permiten establecer si un incidente está relacionado con un grupo o campaña concreta, si se ha reutilizado infraestructura maliciosa o si ya se había producido actividad previa no detectada.

## 8. Investigación forense aplicada a distintos tipos de evidencia

Los tipos de evidencia más habituales son diversos, y cada uno exige un enfoque distinto. La investigación no puede plantearse de forma uniforme: cada entorno genera artefactos particulares y requiere herramientas y criterios específicos.

### 8.1. Red y tráfico

El análisis de tráfico permite detectar conexiones sospechosas, intentos de exfiltración, uso de protocolos no habituales o comunicación con infraestructura externa. Se pueden inspeccionar PCAPs, logs de proxy, DNS, conexiones de red y patrones de envío de datos. Es especialmente útil para detectar C2 (command and control), beaconing y actividades con exfiltración de datos.

### 8.2. Sistema operativo

El sistema operativo ofrece evidencia clave sobre procesos, autenticación, permisos, archivos abiertos, arranque, servicios, cronjobs y cambios de seguridad. En un análisis de ransomware, por ejemplo, puede detectar cambios en la configuración de servicios, creación de tareas para ejecución persistente y alteración de permisos.

### 8.3. Endpoint

Los investigadores trabajan con endpoints para determinar si se ejecutó una herramienta, si se abrió un archivo malicioso, si el usuario interactuó con contenido sospechoso o si el sistema presenta artefactos de mantenimiento. El endpoint suele ser la mejor fuente para establecer una relación entre las acciones del usuario y la actividad del atacante.

### 8.4. Aplicaciones y bases de datos

El impacto del incidente puede afectar a las aplicaciones y a los datos de negocio. En esos casos es necesario combinar evidencias procedentes del sistema, del servicio y de la base de datos. La investigación puede revelar cambios no autorizados, alteración de registros o extracción de información sensible.

### 8.5. Evidencia física

Cuando el incidente tiene origen o consecuencias físicas, la investigación debe incluir registros de acceso, grabaciones, dispositivos y presencia de personas. Incluso cuando se trata de un incidente digital, la evidencia física puede explicar la manera en que se produjo un acceso o una alteración del entorno.

## 9. Intercambio de información

### 9.1. Importancia del intercambio de información

Cuando un incidente afecta a una organización, su impacto rara vez se limita al entorno inmediato. En un ecosistema interconectado, la amenaza puede propagarse a proveedores, socios, clientes, prestadores de servicios, y entidades reguladoras o de coordinación. Por ello, el intercambio de información es una práctica esencial dentro de la gestión del incidente: permite validar indicadores, reducir la latencia en la respuesta, coordinar acciones y acelerar la mitigación en un contexto de riesgo compartido.

La información compartida puede incluir datos técnicos y operativos sobre actores, fraudes identificados, URLs y dominios asociados, IOCs, patrones de uso, comportamiento observado, artefactos detectados y hallazgos de investigación. Este flujo tiene un valor estratégico porque permite a otras organizaciones protegerse antes de que el ataque alcance nuevas víctimas, se repita en otros entornos o se convierta en una campaña más amplia. El intercambio de información, por tanto, no es un acto administrativo secundario, sino una dimensión de la defensa colectiva.

Desde un punto de vista empresarial y académico, el intercambio debe entenderse como un mecanismo de aprendizaje organizativo y colectivo. Las organizaciones no solo responden a un incidente aislado: también integran el conocimiento generado en su capacidad de detección, prevención y mejora continua. La organización que comparte información útil y la convierte en inteligencia operativa aumenta su resiliencia y fortalece su posición frente a amenazas persistentes y emergentes.

### 9.2. Agentes con los que se puede intercambiar información

El intercambio de información puede producirse con distintos actores:

- proveedores de seguridad;
- proveedores cloud y de infraestructura;
- operadores de red y telecomunicaciones;
- auditores o consultores de ciberseguridad;
- servicio de atención o coordinación nacional y sectorial;
- equipos internos de seguridad y respuesta;
- autoridades competentes en materia de seguridad y protección de datos.

No siempre la información debe compartirse de la misma forma. Algunas organizaciones gestionan la divulgación según su nivel de sensibilidad, su marco regulatorio, la necesidad de protección del negocio y la relevancia del indicador para terceros. El intercambio debe equilibrar la necesidad de acelerar la respuesta con la obligación de proteger información sensible, secretos empresariales o datos de terceros.

### 9.3. Qué se puede compartir

Se suele intercambiar información de naturaleza técnica y operativa, como:

- IOCs: direcciones IP, dominios, hashes, nombres de archivos, patrones de correo;
- indicadores de comportamiento o técnicas observadas;
- datos de conexión y acceso no autorizados;
- artefactos asociados a la campaña;
- evidencia resumida de la investigación;
- informes iniciales y análisis preliminares;
- recomendaciones de mitigación o bloqueo.

El objetivo no es exponer íntegramente la investigación, sino compartir la información que permita reducir el riesgo para otras organizaciones y mejorar la capacidad colectiva de defensa.

### 9.4. Intercambio de información en ciberdefensa y gestión de incidentes

Con independencia de la obligatoriedad que en algunos casos conlleva la comunicación de incidentes a terceros (autoridades competentes, CSIRT de referencia, afectados, etc.), el intercambio de información con entidades relevantes en el ámbito de la seguridad puede aportar a las organizaciones un valor añadido muy importante de cara tanto a la detección como a la gestión de incidentes de seguridad.

La colaboración e intercambio de información en ciberdefensa puede mejorar los tiempos de respuesta frente a incidentes. Si se comparte información, las organizaciones tienen la posibilidad de contar con un panorama de información mayor, ya que cuando únicamente se utilizan datos propios, la perspectiva está sesgada. Este hecho permite tomar conciencia del estado global de la seguridad y obtener una comprensión más avanzada frente a las amenazas nuevas y ya existentes.

Por ello, es recomendable que las organizaciones establezcan relaciones de confianza con terceros de interés y formalicen mecanismos de intercambio que enriquezcan el conocimiento sobre nuevas amenazas, nuevas técnicas de ataque, vulnerabilidades y, en definitiva, la inteligencia que posibilita una respuesta temprana ante la materialización de un incidente.

Entre los ejemplos de información que puede compartirse destacan:

- avisos de seguridad y campañas de ataque;
- vulnerabilidades nuevas o críticas;
- informes sectoriales y análisis de tendencias;
- buenas prácticas y recomendaciones de mitigación;
- indicadores de compromiso (IP, hashes, dominios, certificados, firmas, patrones de comportamiento);
- alertas tempranas y avisos de actividad sospechosa;
- procedimientos de respuesta y guías de actuación;
- hallazgos derivados de análisis forenses o investigaciones internas.

La organización debe, por tanto, evaluar la conveniencia de establecer y formalizar mecanismos de intercambio con los principales proveedores de productos y sistemas de información, Fuerzas y Cuerpos de Seguridad del Estado, proveedores de telecomunicaciones y CSIRT u otros grupos de respuesta o gestión de incidentes, principalmente de su sector.

Sin embargo, el proceso no siempre resulta sencillo, porque:

- es difícil registrar, resaltar y comunicar los modus operandi de los atacantes;
- existe exceso de fuentes de información, lo que dificulta hacer un seguimiento de la información de calidad;
- el formato de la información suele ser inconexo, ya que cada fuente elige una forma diferente de caracterizar las amenazas.

Para lograr que el intercambio de información sea efectivo, debe tenerse en cuenta la relación entre confianza, estandarización, accesibilidad, calidad de los datos y tratamiento del dato. En este sentido, conviene:

- acordar con los terceros el tipo de información a diseminar para garantizar el equilibrio de intereses y expectativas;
- medir la calidad de la información intercambiada;
- asegurar que la información compartida sea necesaria para el propósito que se persigue;
- compartir solo con quienes realmente lo necesiten, aplicando niveles de difusión y clasificación adecuados;
- aplicar estándares y acuerdos para uso y protección de la información;
- garantizar que la información sea precisa, actualizada y compartida con agilidad;
- llevar un registro seguro de la información compartida y de a quién se facilita;
- utilizar canales seguros, apropiados y efectivos para incentivar la confianza y la colaboración.

### 9.5. Indicadores de compromiso (IOC)

Los indicadores de compromiso describen las características técnicas de una amenaza a partir de las evidencias que deja en un entorno una vez se ha producido la intrusión o la ejecución maliciosa. En la práctica, los IOC pueden consistir en direcciones IP, dominios, hashes, nombres de archivos, rutas de persistencia, firmas, tokens, cambios en registros, patrones de comunicación o comportamientos observados en sistemas afectados. Su función principal es ayudar a detectar, confirmar y rastrear la actividad maliciosa a través del entorno organizativo.

Tal como describe Antonio Villalón en Security Art Work, un indicador de compromiso puede definirse como una pieza de información útil para identificar el posible compromiso de un entorno: desde una dirección IP hasta un conjunto de Tácticas, Técnicas y Procedimientos (TTP) empleados por un atacante. La calidad del IOC depende de su capacidad para ser específico, verificable y accionable. Una mala definición de un indicador puede originar falsos positivos, ruido operacional y pérdida de confianza en el proceso de detección.

Los IOC pueden clasificarse en tres tipos principales:

- Atómicos: no pueden descomponerse en partes más pequeñas sin perder utilidad. Ejemplos: una IP, un dominio, una URL, un valor hash.
- Calculados: se derivan de artefactos o datos implicados en un incidente, como el hash de un fichero, una firma de malware o un valor de identificación asociado a una muestra.
- Conductuales: representan el comportamiento del atacante y su modus operandi, más que la firma de un artefacto concreto. Por ejemplo, la modificación de políticas del dominio como mecanismo de escalada de privilegios o la ejecución de scripts ocultos tras la autenticación del usuario.

Los IOC atómicos y calculados suelen asociarse a la inteligencia táctica y tienen un tiempo de vida corto; un atacante puede cambiar fácilmente la dirección IP del servidor de mando y control o el hash del payload. Los indicadores conductuales, en cambio, están más ligados a la inteligencia operativa y a la interpretación de patrones, por lo que suelen ser más persistentes y más útiles para detectar intrusiones continuadas o campañas repetidas.

La pirámide del dolor, propuesta por David J. Bianco, ilustra muy bien la relación entre la disponibilidad de indicadores y la dificultad de evadirlos. A medida que se avanza desde indicadores simples e identificadores aislados hacia patrones de comportamiento y técnicas, los IOC se vuelven más valiosos desde el punto de vista analítico y más difíciles de eludir para el atacante. Sin embargo, también requieren una mayor capacidad de análisis, contexto y correlación.

### 9.6. Estándares para el intercambio de información

En la gestión de la ciberseguridad y, sobre todo, en la gestión de incidentes, la información es un recurso estratégico. En ocasiones es necesario procesar una cantidad ingente de datos en el mínimo tiempo posible; para ello resulta imprescindible un lenguaje común que permita comunicar y compartir información de forma sencilla y no ambigua. Este lenguaje debe basarse en estándares que definan con claridad las características de una amenaza, los observables asociados, la cronología del incidente, los activos afectados y el contexto del compromiso.

La guía CCN-STIC-424, “Intercambio de información de ciberamenazas. STIX-TAXII. Empleo en REYES”, es una referencia fundamental en este ámbito. Su objetivo es permitir que la información sobre amenazas se describa de manera uniforme, se analice y se comparta sin pérdida de contexto ni ambigüedad. De lo contrario, el intercambio de información se convierte en un ejercicio de acumulación de datos sin utilidad operativa.

La inteligencia de amenazas es el conjunto de datos que, tras ser refinados, analizados, contextualizados y procesados, se convierten en información útil para la organización. Para que un dato sea inteligencia, debe cumplir tres condiciones: ser relevante, procesable y valioso. Debe aportar contexto para apoyar la toma de decisiones, ser suficientemente preciso como para generar una respuesta o acción, y contribuir a la consecución de objetivos del negocio o del entorno institucional.

En este sentido, la inteligencia de amenazas es mucho más que un repositorio de indicadores. Es un mecanismo de conocimiento orientado a la prevención, la detección y la respuesta. Una organización que comparte solo listas de IPs o hashes sin contextualizar su relación con el riesgo, el vector, la técnica o la oportunidad de explotación, no está produciendo inteligencia real; está generando ruido.

En esta lógica, la organización necesita plataformas de Threat Intelligence que faciliten y agilicen el intercambio y la explotación de esa información. Cuando no existen mecanismos de normalización ni análisis, la información puede generar incertidumbre, duplicidad, falsas alarmas y baja confianza en los canales de colaboración. Entre las iniciativas y marcos más relevantes se encuentran ATT&CK, desarrollado por MITRE, y los estándares STIX, TAXII, CyBOX, OpenIOC y MAEC.

La diferencia entre dato, información e inteligencia es esencial:

- dato: elemento bruto, aislado y sin contexto contextual;
- información: conjunto de datos organizados y relacionados;
- inteligencia: información valorada, interpretada y útil para la toma de decisiones.

En ciberseguridad, esta distinción es crítica, porque los indicadores más simples pueden ser rápidamente inútiles si no se relacionan con contexto actor, técnica, impacto y propósito.

### 9.7. STIX, TAXII, OpenIOC y otros estándares

#### STIX

STIX (Structured Threat Information eXpression) es un lenguaje estandarizado en formato XML que permite caracterizar la información sobre ciberamenazas para que pueda ser compartida, almacenada y analizada de forma consistente. MITRE mantiene la especificación oficial, y la documentación puede consultarse en su sitio web y en repositorios públicos.

El lenguaje STIX está diseñado para apoyar múltiples casos de uso relacionados con la gestión y el análisis de ciberamenazas, la respuesta ante incidentes, la caracterización de patrones específicos o el intercambio de información sobre amenazas. Un analista puede documentar observables de interés e indicadores de compromiso obtenidos del análisis del correo fraudulento, como direcciones de envío y entrega, URLs involucradas, adjuntos y tipos de archivo, así como las Tácticas, Técnicas y Procedimientos detectados.

En STIX, los incidentes se representan como instancias discretas de indicadores que incluyen información como cronología de hechos, partes involucradas, activos afectados, evaluación de impacto, TTP, actores atribuidos, naturaleza del compromiso y registro de acciones tomadas.

Desde un punto de vista metodológico, STIX permite transformar una investigación forense en un artefacto estructurado, reutilizable y comparables con otras fuentes de inteligencia. Esto resulta especialmente útil para la automatización de detección, el análisis comparativo entre incidentes y la gestión de información a escala organizativa o sectorial.

#### TAXII

TAXII (Trusted Automated eXchange of Indicator Information) define un conjunto de servicios y formatos que permiten el intercambio de información sobre ciberamenazas entre organizaciones y sistemas de información de forma automática y en tiempo real. Al igual que STIX, está mantenido por MITRE.

La función de TAXII es dar una base técnica para el transporte de la información, mientras que STIX define su contenido semántico. En otras palabras, STIX describe la amenaza; TAXII expone la forma de distribuirla de manera segura y automatizada entre organizaciones o sistemas. La combinación de ambos es clave para diseñar canales de colaboración fiables, rápidos y escalables.

#### OpenIOC

La empresa Mandiant desarrolló OpenIOC, un framework open source para describir de forma semántica el comportamiento de malware o APTs mediante ficheros XML, o bien para buscar signos de infección en una máquina sin necesidad de realizar un análisis exhaustivo para identificar el tipo de amenaza.

OpenIOC define un formato de fichero con extensión .ioc que contiene un esquema XML para describir las características técnicas de una amenaza, una metodología de ataque o cualquier otro tipo de indicador de compromiso. Aunque STIX es más amplio en alcance, OpenIOC es especialmente útil para representar condiciones de detección concretas y reutilizables en herramientas de seguridad.

#### TLP

El TLP (Traffic Light Protocol) es un estándar de facto utilizado por la comunidad internacional de equipos de respuesta a incidentes para clasificar qué información puede compartirse y con quién. Basado en cuatro niveles de color, el esquema permite indicar el alcance de la difusión de la información y evita que la información sensible desborde el círculo de destinatarios apropiados. TLP no es aplicable a información clasificada.

Su utilidad es clara: establece límites claros para la distribución de la información sin imponer una estructura legal rígida. De este modo, se facilita que los equipos compartan hallazgos esenciales sin comprometer la confidencialidad ni la necesidad de protección del negocio.

### 9.8. Plataformas de inteligencia de amenazas

Los indicadores de compromiso pueden almacenarse y distribuirse a través de las llamadas Threat Intelligence Sharing Platforms (TISP), plataformas de inteligencia contra amenazas que centralizan gran cantidad de datos provenientes de distintas fuentes y formatos. Estas plataformas están diseñadas para:

- combinar fuentes de información en un solo punto centralizado;
- recibir y configurar alertas en tiempo real;
- normalizar los datos que obtienen;
- integrar sus datos con otros sistemas, como cortafuegos o SIEM;
- generar informes y cuadros de mando.

Algunas de sus funciones más relevantes son la correlación de amenazas, la validación de indicadores, la automatización de reglas y la consolidación de la información operativa en un único punto. Esto permite convertir fuentes dispares en un flujo gestionado y accionable.

Algunos ejemplos de plataformas ampliamente conocidas son MISP, MineMeld y MANTIS.

#### MISP

MISP (Malware Information Sharing Platform) es una tecnología usada por organizaciones para implementar una plataforma de intercambio de ciberinteligencia centrada principalmente en malware y sus indicadores de compromiso. Ofrece una base de datos centralizada de eventos de ciberseguridad en un formato estructurado compatible con iniciativas como OpenIOC o STIX.

Sus principales objetivos son:

- facilitar el almacenamiento de información sobre ataques y malware detectado;
- crear relaciones automáticas entre el malware y sus atributos;
- almacenar la información en un formato estructurado;
- generar reglas para sistemas de detección de intrusos;
- compartir las características de muestras de malware y de amenazas con grupos de confianza.

MISP combina un repositorio indexado con un mecanismo de compartición multidireccional. Además, en determinadas circunstancias, permite automatización de importación y exportación y la interconexión con otros sistemas. Su utilidad es especialmente clara para redes de colaboración y centros de respuesta, donde la reutilización de inteligencia puede mejorar la detección y la respuesta en tiempo real.

#### MineMeld

MineMeld es un framework open source de Palo Alto Networks que permite recopilar indicadores de compromiso, asignarles una fiabilidad y tratarlos para generar parámetros y objetos que luego puedan incorporarse a distintos elementos de la arquitectura de seguridad. A través de MineMeld, las organizaciones pueden integrar fuentes públicas, privadas o comerciales de inteligencia y traducir los indicadores a controles procesables para los dispositivos de seguridad.

Su valor reside en que convierte la inteligencia en políticas accionables: listas de bloqueo, reglas de firewall, restricciones de acceso, búsquedas en SIEM y cuellos de botella de detección. Es un ejemplo claro de cómo la inteligencia debe incorporarse al control operacional, no quedarse solo como información documental.

#### MANTIS

MANTIS (Model-based Analysis of Threat Intelligence Sources) es una plataforma que ayuda a la gestión de la ciberinteligencia expresada en estándares como STIX, CyBOX, OpenIOC, etc. Uno de sus principales objetivos es proporcionar una base sobre la cual se puedan llevar a cabo investigaciones y desarrollos impulsados por la comunidad en la gestión de inteligencia de amenazas, facilitando la navegación, el filtrado y la búsqueda de la información recopilada.

MANTIS enfatiza la necesidad de un entorno común para la investigación de amenazas, la comparación de indicadores, la integración de fuentes distintas y la trazabilidad del conocimiento colectado. Al hacerlo, refuerza la visión de que la inteligencia es un proceso de construcción, validación y reutilización, no un mero archivo de observables.

### 9.9. Relación entre intercambio de información, ciberinteligencia y respuesta

La ciberinteligencia no es solo un conjunto de indicadores aislados, sino una capa de conocimiento que conecta amenazas, técnicas, actores, contextos y acciones realizadas. El intercambio de información tiene sentido solo si se convierte en inteligencia útil, si se normaliza y si se incorpora a las decisiones de seguridad operativa.

En este sentido, se puede afirmar que la inteligencia sirve a la organización para:

- anticiparse a nuevas amenazas;
- reforzar la detección y la correlación;
- mejorar la respuesta ante incidentes;
- reducir el tiempo entre detección y contención;
- apoyar la toma de decisiones de riesgo y continuidad del negocio;
- mejorar la coordinación con terceros, autoridades y proveedores.

La relación entre estos elementos es estrecha: la información compartida se analiza, se valida y se transforma en inteligencia; la inteligencia permite identificar patrones de amenaza; y esos patrones se convierten en medidas de detección, contención y mejora organizativa. En términos académicos, se trata de un ciclo de aprendizaje organizativo en materia de ciberseguridad, donde la experiencia de cada incidente se integra en el sistema de conocimiento colectivo.

Este enfoque convierte el intercambio de información en una pieza clave del ciclo de defensa: desde la detección inicial hasta la contención, la recuperación y la mejora continua del sistema.

### 9.10. Calidad, utilidad y validez de la información compartida

La inteligencia no es útil por el simple hecho de existir; lo relevante es su calidad, su grado de fiabilidad y su capacidad para sostener una decisión operativa. Una pieza de información puede parecer útil por su apariencia técnica o por la autoridad de la fuente, pero si no está contextualizada, validada y actualizada, puede inducir a una respuesta inadecuada. Por ello, cualquier flujo de intercambio de información debe evaluarse con criterios de relevancia, valor, veracidad y oportunidad.

En términos prácticos, la calidad de la información de amenazas se mide atendiendo a varios factores:

- exactitud: la observación describe fielmente lo ocurrido;
- relevancia: la información es útil para el entorno, la infraestructura o la amenaza concreta;
- actualidad: la información está viva, no obsoleta;
- contexto: el dato se interpreta en relación con actor, vector, impacto y tiempo;
- trazabilidad: puede atribuirse a una fuente o proceso de validación;
- confiabilidad: la fuente tiene una historia de calidad y no produce ruido excesivo;
- accionabilidad: la información permite actuar de manera concreta y medible.

Un indicador de compromiso sin contexto puede convertirse en ruido, mientras que la misma información integrada en una línea temporal, una técnica de ataque y un impacto de negocio puede transformar el dato en inteligencia ejecutable. Por esta razón, la organización debe establecer procesos de validación y saneamiento de la información antes de incorporarla a los sistemas de detección o a los informes de gestión.

La evaluación de la calidad tampoco puede limitarse a la dimensión técnica, porque la inteligencia sobre amenazas tiene una dimensión organizativa y estratégica. El valor de la información no depende solo de su grado de detalle, sino también de la capacidad que tenga la empresa para procesarla, interpretarla y aplicarla a su contexto operativo. Esto exige una mezcla de ciberinteligencia, analítica, conocimiento del control interno y comprensión del negocio.

### 9.11. Ciclo de la inteligencia de amenazas

La ciberinteligencia no se reduce a la obtención de indicadores aislados, sino que se articula como un ciclo continuo. De forma general, este proceso comprende varias etapas:

1. recopilación: obtención de datos desde redes, endpoints, logs, feeds externos y fuentes públicas o privadas;
2. normalización: transformación de los datos a un formato común para evitar incompatibilidades;
3. análisis: correlación, contextualización, validación y comparación con incidentes previos;
4. interpretación: construcción de conocimiento sobre actor, técnica, impacto y propósito;
5. difusión: distribución de la información relevante a quienes deben tomar decisiones;
6. uso operativo: incorporación a reglas de detección, respuesta y gestión de riesgo;
7. retroalimentación: evaluación de la eficacia de la información y mejora del proceso.

Este ciclo refleja que la inteligencia no es un producto final estático, sino un sistema dinámico de aprendizaje. La organización que integra esta lógica mejora su capacidad para identificar amenazas emergentes, ajustar sus controles y decidir con más rapidez ante un incidente. Sin retroalimentación, cualquier inteligencia acabará siendo un archivo de indicadores sin valor real para la defensa.

Un ejemplo claro es el caso de una campaña de phishing dirigida a un sector concreto. El primer dato puede ser un dominio sospechoso o una URL maliciosa. Al analizarlo con contexto, se comprueba que se utiliza una técnica de suplantación de identidad y que el dominio comparte infraestructura con anteriores ataques. A partir de ahí, la información se convierte en inteligencia operativa que puede activar filtros, revisión de nuevos mensajes, análisis de correo, y alertas en usuarios críticos. Este proceso demuestra que la utilidad de la inteligencia reside en su capacidad de convertirse en acción.

### 9.12. Relación entre inteligencia, riesgo y decisión organizativa

La inteligencia de amenazas solo tiene sentido si se vincula con los objetivos de la organización. En otras palabras, no se comparte o consume información por el mero interés técnico, sino porque permite reducir el riesgo y proteger activos estratégicos. El riesgo no solo depende de la existencia de una amenaza, sino también de la vulnerabilidad del sistema, la criticidad del activo, la capacidad de detección y la resistencia operativa de la organización.

Por ello, el analista o responsable de seguridad debe responder a una pregunta esencial: ¿qué amenaza concreta afecta a nuestro negocio y cuál es la probabilidad de que se materialice? La inteligencia ayuda a responder esta cuestión, pero no sustituye la gestión del riesgo. La toma de decisiones debe combinar la ciberinteligencia, la evaluación de riesgos, la continuidad del negocio y la estratificación de los activos.

Esto es especialmente importante en organizaciones con entornos híbridos, proveedores de servicios críticos, infraestructuras en la nube o sistemas de información con alta dependencia tecnológica. En estos entornos, la amenaza no se percibe solo como un conflicto técnico, sino como un riesgo organizativo cuya materialización puede afectar a la reputación, la operación, la privacidad y la continuidad del servicio.

### 9.13. Dimensión jurídica, ética y regulatoria del intercambio

La investigación del incidente y el intercambio de información no son solo cuestiones técnicas; también tienen implicaciones jurídicas y éticas. Las organizaciones deben respetar normas de protección de datos, confidencialidad, privacidad, propiedad intelectual y regulación sectorial, así como las restricciones legales de cada país o ámbito institucional.

La información de un incidente puede incluir datos personales, detalles de usuarios, metadatos, contenido de comunicaciones o indicadores que, si se comparten sin control, pueden afectar a terceros. Por eso, cualquier mecanismo de intercambio ha de estar alineado con políticas internas, marco legal aplicable y procedimientos de tratamiento de la información. La apertura de canales de colaboración no debe convertirse en una vía para la divulgación indiscriminada de evidencias o de datos sensibles.

Desde un punto de vista ético, la ciberinteligencia debe usarse para proteger y reducir el riesgo, no para vigilar de manera arbitraria ni para convertir la amenaza en una herramienta de presión o manipulación. El cumplimiento de protocolos de clasificación, la trazabilidad del flujo de información y la justificación del intercambio son requisitos esenciales para mantener la confianza entre organizaciones, proveedores y autoridades.

La buena práctica exige distinguir entre información relevante para la defensa colectiva y datos que podrían ser excesivamente sensibles o no necesarios para el objetivo de la operación. En este sentido, la utilización del TLP, la clasificación del impacto, las políticas internas de acceso y la documentación del intercambio son instrumentos esenciales para mantener un equilibrio entre colaboración y prudencia.

### 9.14. Intercambio de información como factor de resiliencia

En un entorno cada vez más interconectado, la ciberresiliencia depende no solo de la capacidad de reaccionar al ataque, sino también de la capacidad de aprender y adaptarse. El intercambio de información contribuye directamente a esa capacidad. Cuando distintas organizaciones comparten indicadores, patrones y hallazgos relevantes, el conjunto del ecosistema se vuelve más resistente frente a la repetición de amenazas.

La resiliencia no se define solo por la capacidad de restaurar servicios tras un incidente, sino por la capacidad de anticipar, detectar, aprender y mejorar. En ese marco, la información compartida gana valor si se convierte en práctica recurrente: reglas de detección, actualizaciones de políticas, formación específica, revisión de controles, rediseño de procesos y mejora de la continuidad del negocio.

En resumen, la investigación forense del incidente y la inteligencia compartida no son actividades separadas; forman parte de una misma lógica de conocimiento, defensa y mejora. La organización que logra convertir información dispersa en inteligencia útil, y esa inteligencia en decisiones operativas, consigue reforzar su capacidad de respuesta y aumentar la madurez de su seguridad.

## 10. Contención, erradicación y recuperación

La investigación no termina con la identificación de la causa. La información obtenida debe traducirse en acciones concretas para controlar la amenaza, minimizar el impacto y restaurar la operación normal.

### 10.1. Contención

La contención consiste en limitar la propagación del incidente y reducir sus efectos. Se puede llevar a cabo mediante una amplia variedad de medidas, como:

- desconexión de equipos comprometidos;
- bloqueo de cuentas o ingressos de red;
- aislamiento de segmentos de red;
- desactivación de servicios específicos;
- restricciones de acceso a recursos críticos;
- cierre de sesiones sospechosas o tokens comprometidos.

La contención debe priorizar los activos más críticos y la continuidad del negocio, sin perder de vista la necesidad de preservar la evidencia.

### 10.2. Erradicación

La erradicación consiste en eliminar el vector o la causa del incidente. Puede incluir:

- eliminación de malware o scripts;
- corrección de vulnerabilidades detectadas;
- limpieza de cuentas o permisos maliciosos;
- desmontaje de persistencia;
- revisión de infraestructura de confianza;
- cribado de otros hosts o activos afectados.

A menudo la erradicación requiere más que borrar un archivo; puede implicar revisar toda la red, validar si existe persistencia, comprobar cuentas de servicio, eliminar tareas programadas y revisar servicios de administración.

### 10.3. Recuperación

La recuperación se refiere a la restauración del sistema y la vuelta a la normalidad. Esto puede implicar:

- restauración desde imágenes limpias;
- reimplantación de equipos;
- verificación de la integridad de servicios;
- comprobación de backups y de copias de seguridad;
- validación de permisos y autenticación;
- monitorización intensificada durante un periodo posterior.

La recuperación debe verificarse con evidencia objetiva: no basta con “volver a poner en marcha” un servicio; hay que comprobar que los sistemas funcionan correctamente y que no quedan rastros del incidente.

### 10.4. Lecciones aprendidas

Una vez finalizado el caso, la organización debe documentar las lecciones aprendidas. Este paso es esencial para la mejora del nivel de seguridad. Se analizan los controles que fallaron, las debilidades procedimentales, los errores de detección, la adecuación del plan de respuesta y la necesidad de reforzar formación, segmentación o monitorización.

El objetivo no es solo cerrar el caso, sino reducir la probabilidad de repetición. La lecciones aprendidas convierten la experiencia en un activo organizativo para la mejora continua del sistema de gestión de riesgos.

## 11. Ejemplos prácticos

### 11.1. Análisis básico de un archivo sospechoso

```bash
file archivo_sospechoso.exe
sha256sum archivo_sospechoso.exe
strings -n 8 archivo_sospechoso.exe | head -n 50
```

Este flujo permite identificar el tipo de archivo, su integridad y algunos datos de texto que puedan revelar nombres de servidor, URLs, cadenas internas o comentarios. En un caso real, la ejecución de estas comprobaciones puede ayudar a decidir si el archivo requiere aislamiento o análisis adicional.

### 11.2. Verificación de conexiones sospechosas

```bash
ss -tulpn | grep -E ':80|:443|:22|:3389'
netstat -ano | findstr LISTENING
```

Estas órdenes permiten detectar puertos abiertos, conexiones activas y servicios accesibles. En un caso de intrusión, la presencia de un puerto no habitual o una conexión a una IP externa rara puede servir como punto de partida para la investigación.

### 11.3. Script básico para recoger metadatos

```python
import hashlib
import os

for root, _, files in os.walk('.'):
    for f in files:
        path = os.path.join(root, f)
        h = hashlib.sha256()
        with open(path, 'rb') as fh:
            for chunk in iter(lambda: fh.read(65536), b''):
                h.update(chunk)
        print(f'{path}: {h.hexdigest()}')
```

Este ejemplo demuestra cómo obtener un valor hash para cada archivo del entorno. Esto resulta útil para identificar diferencias entre una imagen original y una copia modificada, así como para documentar evidencia y compararla con artefactos sospechosos.

### 11.4. Investigación de un caso realista

Imaginemos un caso en el que un usuario recibe un correo con un archivo ZIP aparentemente legítimo. El usuario lo abre y el sistema presenta un comportamiento extraño: el navegador se abre, se ejecutan procesos nuevos y el equipo empieza a generar tráfico hacia una dirección externa. El analista debe seguir este proceso:

1. confirmar la anomalía;
2. aislar el equipo;
3. capturar memoria y crear imagen del disco;
4. revisar logs de correo, acceso, navegador y autenticación;
5. analizar procesos, tareas programadas y ejecución de scripts;
6. localizar tráfico de red asociado;
7. comprobar si la máquina tiene persistencia;
8. identificar la causa raíz y decidir contención;
9. documentar el caso para la organización y la mejora del sistema.

Este tipo de caso ilustra la relevancia de la investigación ordenada frente a la reacción impulsiva. Cuanto antes se preserve la evidencia, mejor será la calidad del análisis y más efectiva la respuesta.

## 12. Ejercicios de consolidación

### Ejercicio 1. Cadena de custodia

Imagina que un técnico recoge un equipo sospechoso. Redacta la cadena de custodia con: quién, qué, cuándo, dónde, motivo y acceso posterior.

#### Solución orientativa

- identificar al responsable de la recogida;
- registrar la fecha, hora y ubicación exacta;
- describir el equipo y el estado en que se encontró;
- documentar el motivo de la intervención;
- registrar cada vez que alguien accede al equipo o al soporte físico;
- asegurar la conservación del material y la trazabilidad documental.

### Ejercicio 2. Caso forense

Un usuario ha recibido un correo con un archivo ejecutable. ¿Qué evidencias vas a recoger primero?

#### Solución orientativa

- archivo adjunto y evidencia del correo original;
- headers del mensaje y metadatos del correo;
- logs de correo y gateway;
- memoria del equipo si ya se ejecutó el archivo;
- registros de sistema de ejecución y procesos;
- información de red y conexión de salida asociada.

### Ejercicio 3. Respuesta ante malware

La máquina de un usuario muestra comportamiento anómalo. ¿Qué decisión tomas primero: aislar, investigar o recuperar?

#### Solución orientativa

Lo primero debe ser aislar el equipo para evitar propagación o actividad maliciosa adicional. A continuación, se debe preservar la evidencia, analizar el sistema y documentar la secuencia de eventos antes de decidir la recuperación definitiva.

### Ejercicio 4. Análisis de causa raíz

Describe qué preguntas harías para investigar si un acceso no autorizado se produjo desde una cuenta de administrador.

#### Solución orientativa

- ¿Se produjo por phishing o sesión comprometida?
- ¿Hubo reutilización de credenciales?
- ¿Existieron registros de MFA fallidos o bypass de autenticación?
- ¿Se usó un token, un servicio de administración o un proceso automático?
- ¿Se produjo un cambio de política o de permisos previo?
- ¿La cuenta estaba protegida con buenas prácticas de gestión de identidades?
- ¿Se detectó comportamiento anómalo en la red o en el endpoint?

### Ejercicio 5. Alcance del incidente

Explica qué aspectos deben analizarse para decidir si un incidente puede considerarse de baja, media, alta o crítica severidad.

#### Solución orientativa

- impacto en confidencialidad, integridad y disponibilidad;
- número de activos afectados;
- sensibilidad de los datos involucrados;
- persistencia y lateralización detectada;
- dependencia funcional de los sistemas comprometidos;
- afectación a clientes, proveedores o cumplimiento normativo;
- capacidad de contención y recuperación.

## 13. Actividades prácticas recomendadas

- análisis forense de un archivo sospechoso en entorno virtual;
- captura y validación de un paquete de red sospechoso;
- extracción de hash y verificación de integridad de evidencias digitales;
- análisis de logs de VPN, autenticación y acceso a recursos;
- preparación de una línea temporal de incidentes;
- simulación de un caso de phishing con posterior investigación forense;
- análisis de persistencia en sistemas Windows y Linux;
- revisión de la correcta aplicación de la cadena de custodia.

## 14. Resumen

La investigación del incidente es la fase que convierte la sospecha en conocimiento y la alarma en acción. Para actuar de forma efectiva, la organización debe preservar la evidencia, evitar contaminarla, reconstruir la secuencia de hechos, identificar la causa raíz y traducir el análisis en medidas de contención, erradicación y recuperación. En este sentido, la calidad de la investigación determina en gran medida la calidad de la respuesta, la fiabilidad de la decisión y la capacidad de aprendizaje organizativo.

Una investigación bien ejecutada no solo confirma lo ocurrido, sino que permite comprender la lógica del ataque, evaluar el impacto real, proteger los activos críticos y construir un conocimiento útil para la mejora permanente de la seguridad. Este enfoque convierte la investigación de incidentes en una disciplina esencial dentro de la gestión de riesgos, la continuidad operativa y la madurez de la organización frente a amenazas crecientes y cada vez más sofisticadas.

## 15. Recursos recomendados

- TeoríaUD3-04-Intercambio de información.pdf
- TeoríaUD3-05-Respuesta al incidente.pdf
- Documentación de herramientas forenses y de análisis de malware
- Guías de buenas prácticas en cadena de custodia y análisis de evidencia digital

## 16. Autoevaluación

1. ¿Qué es la cadena de custodia y por qué es esencial?
2. ¿Qué tipo de evidencia se prioriza en una investigación y por qué?
3. ¿Qué son los IOCs y para qué sirven?
4. ¿Qué diferencias existen entre contención, erradicación y recuperación?
5. ¿Por qué es necesario documentar la investigación y qué elementos debe incluir un informe técnico?
6. ¿Cómo influye la línea temporal en la reconstrucción del incidente?
7. ¿Qué medidas se deben adoptar ante evidencia de persistencia o lateralización?
8. ¿Qué relación existe entre causa raíz e inversión en control de seguridad?

---

<p align="center">
  <strong>La investigación del incidente no busca solo confirmar lo ocurrido, sino comprender la causa raíz para prevenirlo y reducir su impacto en el futuro.</strong>
</p>
