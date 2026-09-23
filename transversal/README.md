# Módulo Transversal: Gestión de Incidentes Cibernéticos

## 1. Introducción

La gestión de incidentes cibernéticos es el conjunto de procesos, procedimientos y buenas prácticas que permiten detectar, analizar, contener, remediar y aprender de eventos de seguridad que puedan afectar la confidencialidad, integridad o disponibilidad de los activos de una organización.

En un entorno digital, los incidentes no solo implican daños técnicos; también afectan la continuidad del negocio, la reputación, la confianza de clientes y la cumplimiento regulatorio. Por ello, la respuesta a incidentes debe organizarse como una disciplina operativa y estratégica.

Este módulo tiene un enfoque transversal: conecta aspectos técnicos, analíticos, organizativos y de comunicación, con el objetivo de dotar a la organización de una capacidad de respuesta ágil, documentada y reutilizable.

## 2. Objetivos del módulo

- Comprender qué es un incidente de seguridad y cómo se diferencia de un evento o de una vulnerabilidad.
- Conocer el ciclo de vida de la gestión de incidentes.
- Identificar tipos de incidentes y sus implicaciones.
- Establecer roles y responsabilidades para la respuesta.
- Aplicar una metodología práctica para la detección, análisis, contención y recuperación.
- Documentar y comunicar incidentes de forma efectiva.
- Aprender lecciones para mejorar la resiliencia y la seguridad organizativa.

## 3. Fundamentos teóricos

### 3.1. Conceptos básicos

#### Evento de seguridad
Un evento es una actividad observable en un sistema o red, como un inicio de sesión, una conexión TCP, una alerta de firewall, la ejecución de un proceso o un cambio en una configuración. Un evento por sí solo no siempre implica un incidente.

#### Incidente de seguridad
Un incidente es un evento o serie de eventos que comprometen o pueden comprometer la seguridad de un activo, sistema o servicio. Un incidente puede suponer:

- acceso no autorizado,
- pérdida de confidencialidad,
- manipulación de datos,
- indisponibilidad de servicios,
- abuso de privilegios,
- ejecución de malware,
- suplantación de identidad,
- exfiltración de información o daño a la reputación.

#### Vulnerabilidad
Una vulnerabilidad es un fallo, defecto o debilidad en un sistema, proceso o configuración que puede ser explotado por un atacante para violar la seguridad.

#### Amenaza
Una amenaza es una fuente potencial de daño: un actor malicioso, un malware, un error humano, un desastre natural o una causa interna accidental.

#### Riesgo
El riesgo es la combinación de la probabilidad de que ocurra una amenaza y el impacto potencial que tendría sobre los activos y la organización.

### 3.2. Diferencia entre evento, incidente, brecha y crisis

- Evento: señal o hecho técnico observable.
- Incidente: evento que afecta o puede afectar la seguridad.
- Brecha: incidente confirmado y materializado que implica exposición o compromiso de información, sistemas o procesos.
- Crisis: situación de mayor gravedad, con impacto operacional, reputacional o regulatorio, que exige coordinación institucional y decisiones de nivel estratégico.

### 3.3. Tipos de incidentes cibernéticos

Los incidentes pueden clasificarse según su naturaleza:

- Malware y ransomware.
- Phishing y suplantación de identidad.
- Uso indebido de credenciales o acceso no autorizado.
- Denegación de servicio (DoS/DDoS).
- Exfiltración de datos.
- Manipulación de configuración o integridad del sistema.
- Compromiso de dispositivos móviles o endpoints.
- Incidentes de terceros y proveedores.
- Ataques a infraestructura crítica y servicios en la nube.

### 3.4. Importancia de la gestión de incidentes

Una buena gestión de incidentes permite:

- minimizar el impacto de los ataques,
- reducir el tiempo de aislamiento y recuperación,
- asegurar la continuidad del negocio,
- preservar la evidencia para análisis y acciones legales,
- mejorar la postura de seguridad a partir de la experiencia,
- cumplir con obligaciones regulatorias y auditorías.

### 3.5. Ciclo de vida de un incidente

El ciclo de vida más extendido se basa en una secuencia lógica:

1. Preparación
2. Detección y análisis
3. Contención
4. Erradicación
5. Recuperación
6. Lecciones aprendidas

#### 1) Preparación
La preparación incluye políticas, procedimientos, herramientas, formación, plan de respuesta, backups, comunicaciones y roles definidos. Es la fase que reduce el tiempo de reacción y facilita la coordinación.

#### 2) Detección y análisis
La detección se produce mediante logs, SIEM, EDR, antivirus, monitorización, alertas de red, reportes de usuarios, etc. El análisis permite validar si el evento es real, entender su alcance, detectar el vector de ataque y decidir la severidad.

#### 3) Contención
Consiste en aislar sistemas, bloquear conexiones, restringir accesos, desactivar cuentas o desconectar equipos comprometidos para evitar la propagación del incidente.

#### 4) Erradicación
Se eliminan malware, artefactos, vulnerabilidades explotadas, cuentas comprometidas y cambios maliciosos. También puede implicar la reinstalación o restauración de sistemas limpios.

#### 5) Recuperación
Se reintroducen servicios, se validan sistemas y se comprueba que la infraestructura vuelve a operar de forma segura. Es vital verificar integridad antes de restablecer servicios críticos.

#### 6) Lecciones aprendidas
Se documentan causas raíz, tiempos de respuesta, puntos débiles y mejoras organizativas. Esta fase es esencial para cerrar el ciclo y evitar repetición.

### 3.6. Modelos de referencia

Aunque existen diversas metodologías, algunas de las más ampliamente utilizadas son:

- NIST SP 800-61: Computer Security Incident Handling Guide.
- SANS Institute: incident response lifecycle.
- ISO/IEC 27035: Information security incident management.

Estas metodologías comparten una lógica común: preparación, detección, análisis, contención, erradicación, recuperación y mejora continua.

### 3.7. Roles y responsabilidades

Una respuesta eficaz requiere una estructura clara:

- Responsable de seguridad o CISO: coordinación estratégica.
- Equipo de respuesta a incidentes (CSIRT/SOC): análisis y ejecución técnica.
- Administradores de sistemas: soporte operativo y recuperación.
- Red y firewall: control de tráfico y aislamiento.
- Desarrollo y aplicaciones: corrección de vulnerabilidades y revisión de logs.
- Legal/compliance: revisión de obligaciones legales y comunicación.
- Comunicaciones y dirección: coordinación con clientes, medios y junta directiva.
- Usuarios: reportar anomalías y seguir procedimientos.

### 3.8. Evidencia digital

Durante un incidente se debe preservar la evidencia para análisis técnico, posible investigación penal o auditoría. Esto incluye:

- logs de aplicación, firewall, antivirus, SIEM, DNS, proxies, Active Directory, servidores y endpoints;
- hashes de archivos;
- capturas de pantalla,
- imágenes forenses,
- copias de memoria,
- trazas de red,
- registros de cambios en la configuración.

La cadena de custodia es clave: quién ha tocado la evidencia, cuándo y por qué.

### 3.9. Clasificación y priorización

Los incidentes deben clasificarse por:

- impacto potencial,
- criticidad del activo,
- sensibilidad de la información afectada,
- alcance del problema,
- duración estimada del impacto,
- afectación a clientes, regulaciones o continuidad del negocio.

Esto permite priorizar la atención según la gravedad.

## 4. Metodología práctica de gestión de incidentes

### 4.1. Fase 1: preparación

Antes de que ocurra un incidente, la organización debe estar lista para responder. Esto incluye:

- políticas y procedimientos de seguridad,
- mapeo de activos críticos,
- plan de continuidad,
- copias de seguridad regulares y verificadas,
- segmentos de red y control de acceso,
- alertas y monitorización,
- formación a usuarios,
- canales de comunicación definidos,
- listados de contacto del equipo de respuesta.

#### Ejemplo práctico
Una empresa con correo corporativo, servidor web y un CRM debe tener:

- alertas de acceso anómalo,
- autenticación multifactor,
- backups diarios de CRM y web,
- registro centralizado de logs,
- contacto del responsable de seguridad y del servicio de TI.

### 4.2. Fase 2: detección y validación

Se recogen señales de alerta, se validan y se decide si requieren una investigación formal.

#### Técnicas de detección
- SIEM: correlación de eventos.
- EDR: detección y aislamiento de endpoints.
- IDS/IPS: detección de tráfico sospechoso.
- Logs de aplicaciones y servicios.
- Alertas de cuentas con privilegios.
- Reportes del personal.

#### Preguntas clave
- ¿Qué ocurre exactamente?
- ¿Es un evento falso positivo o un incidente real?
- ¿Qué activos están afectados?
- ¿Cuándo comenzó?
- ¿Qué ha cambiado?
- ¿Qué información está expuesta?

### 4.3. Fase 3: análisis del incidente

Durante el análisis se intenta responder a la pregunta: ¿qué está ocurriendo y cuál es el alcance?

El análisis incluye:

- identificación del vector de ataque,
- revisión de privilegios explotados,
- identificación de archivos o procesos sospechosos,
- determinar si se produjo movimiento lateral,
- comprobar qué cuentas, hosts y servicios están implicados,
- evaluar si la amenaza sigue activa.

#### Herramientas de apoyo
- Wireshark para análisis de red.
- Sysinternals para análisis de procesos y memoria.
- SIEM para correlación temporal.
- Logs de firewall, DNS y proxy.
- Hashing para comprobar integridad.

### 4.4. Fase 4: contención

La contención es inmediata y prioritaria. Su objetivo es desconectar o limitar los puntos de propagación.

#### Acciones típicas
- aislar un equipo comprometido,
- bloquear IPs o dominios maliciosos,
- deshabilitar cuentas sospechosas,
- restringir acceso a archivos sensibles,
- bloquear conexiones de salida para prevenir exfiltración,
- cerrar servicios afectados,
- activar políticas de control de acceso de emergencia.

La contención debe ser proporcional a la amenaza. No siempre se puede desconectar todo; en algunos casos se requiere limitar el impacto sin interrumpir servicios críticos.

### 4.5. Fase 5: erradicación

Una vez contenido el impacto, se elimina la causa raíz.

#### Elementos clave
- eliminar malware o backdoors,
- cerrar vulnerabilidades explotadas,
- revocar sesiones y tokens,
- cambiar contraseñas y secretos,
- reconstruir equipos o servidores comprometidos,
- aplicar parches,
- corregir misconfiguraciones.

La erradicación debe ser verificable: se deben revisar artefactos, procesos, servicios y cambios no autorizados.

### 4.6. Fase 6: recuperación

La recuperación no trata solo de iniciar servicios, sino de devolver la operación sin introducir riesgo.

#### Buenas prácticas
- restaurar desde backups verificados y limpios,
- validar integridad y autenticidad de los datos,
- comprobar que no quedan artefactos del atacante,
- rehidratar servicios paso a paso,
- mantener la monitorización durante varios días,
- confirmar con usuarios y equipos que los servicios funcionan correctamente.

### 4.7. Fase 7: cierre y aprendizaje

Tras la recuperación, la organización debe documentar:

- qué ocurrió,
- cómo se detectó,
- qué impacto tuvo,
- qué decisiones se tomaron,
- cuánto tardó cada fase,
- qué se podría mejorar.

Estas lecciones se convierten en acciones concretas: mayor monitorización, más formación, cambios de política, mejora de backups, hardening de endpoints y priorización de parches.

## 5. Práctica recomendada: flujo de respuesta a incidentes

### 5.1. Checklist operativo

- Confirmar la alerta o el reporte.
- Clasificar el incidente por severidad.
- Asignar roles.
- Iniciar la documentación.
- Recolectar evidencia sin alterar el entorno.
- Validar la amenaza y el alcance.
- Contener el riesgo.
- Eliminar el punto de entrada.
- Recuperar servicios de forma segura.
- Revisar la evolución y comunicar.
- Cerrar con aprendizaje.

### 5.2. Plantilla de registro de incidente

Nombre del incidente:
Fecha y hora de detección:
Sistema / activo afectado:
Tipo de incidente:
Severidad:
Estado:
Persona responsable:
Descripción del evento:
Impacto inicial:
Acciones de contención:
Evidencia recogida:
Causas raíces:
Medidas correctivas:
Seguimiento y cierre:

### 5.3. Ejemplo de caso práctico

#### Caso: phishing con acceso de credenciales

Un usuario recibe un correo aparentemente legítimo que solicita validar la contraseña del sistema de gestión. El usuario hace clic y introduce credenciales. Horas más tarde, la seguridad observa una serie de accesos anómalos desde una IP externa y un intento de acceso a carpetas compartidas.

##### Proceso

1. Se recibe la alerta de inicio de sesión anómalo.
2. Se valida que la cuenta comprometida pertenece a un responsable de ventas.
3. Se determina que ha habido acceso a una carpeta compartida con información sensible.
4. Se aíslan los equipos afectados y se bloquea la cuenta.
5. Se fuerza el cambio de contraseña y revocación de sesiones.
6. Se revisan los logs de correo, proxy y DNS para identificar la fuente del phishing.
7. Se detectan más usuarios que recibieron el mismo mensaje.
8. Se alerta a la organización para que informe sobre posibles clics.
9. Se actualiza la política de seguridad para reforzar la educación del usuario.
10. Se documenta el incidente y se incorporan mejoras en la configuración del correo y el filtrado.

##### Aprendizaje
- La detección temprana es crucial.
- La formación a usuarios reduce la probabilidad de éxito del phishing.
- Las herramientas de correo y la MFA ayudan a limitar el daño.
- Es necesario hacer seguimiento para detectar movimiento lateral.

## 6. Buenas prácticas para la respuesta

- Defender con principio de menor privilegio.
- Separar responsabilidades entre detección, análisis y respuesta.
- Documentar cada paso.
- No borrar evidencia antes de analizarla.
- Reforzar la monitorización y la automatización.
- Mantener copias de seguridad verificadas y recuperables.
- Revisar y actualizar políticas de seguridad regularmente.
- Hacer ejercicios de simulación y tabletop.

## 7. Medidas de mejora continua

La gestión de incidentes no termina cuando el servicio vuelve a funcionar. Debe mejorar continuamente:

- revisión de indicadores y alertas,
- análisis de causas raíz,
- ejecución de ejercicios de simulación,
- auditoría de procesos,
- actualización de playbooks,
- mejora de la segmentación de red,
- formación y concienciación de usuarios,
- revisión de la continuidad del negocio y la recuperación ante desastres.

## 8. Conclusión

La gestión de incidentes cibernéticos es una capacidad crítica para cualquier organización. No se trata solo de reaccionar ante un ataque, sino de prepararse, detectar con rapidez, responder con criterio y aprender de cada evento.

En una empresa moderna, la diferencia entre un incidente gestionado correctamente y uno descontrolado suele residir en la disciplina, la coordinación, la calidad de los procesos y la capacidad de aprender del error.

Una respuesta eficaz combina:

- preparación técnica,
- análisis forense,
- contención precisa,
- recuperación segura,
- comunicación clara,
- mejora continua y organización.

Solo así la organización puede convertir un incidente en una oportunidad de fortalecer su resiliencia y su postura de seguridad.

## 9. Bibliografía y referencias recomendadas

- NIST SP 800-61 Rev. 2: Computer Security Incident Handling Guide.
- ISO/IEC 27035: Information security incident management.
- SANS Institute: Practical Guidance for Incident Response.
- ENISA: Good practices for incident response and cyber crisis management.
- Frameworks de gestión de continuidad y recuperación ante desastres (BCP/DRP).

## 10. Sugerencia de aplicación práctica

Para reforzar el aprendizaje, se recomienda:

- realizar un análisis de caso real o simulado,
- construir un playbook de respuesta,
- preparar una matriz de severidad,
- ejecutar un ejercicio de mesa (tabletop exercise),
- simular un incidente de phishing, ransomware o acceso no autorizado,
- documentar la lección aprendida y las mejoras propuestas.

Este tipo de práctica permite convertir la teoría en una capacidad operativa útil y repetible.
