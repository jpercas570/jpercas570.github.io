# UD3. Investigación del incidente

<p align="center">
  <img src="https://images.unsplash.com/photo-1516321318423-f06f85e504b3?auto=format&fit=crop&w=1400&q=80" alt="Investigación forense de incidentes" width="100%" />
</p>

<div align="center">

![Unidad](https://img.shields.io/badge/Unidad-UD3-0A84FF?style=for-the-badge)
![Resultado](https://img.shields.io/badge/Resultado-RA3-34D399?style=for-the-badge)
![Enfoque](https://img.shields.io/badge/Enfoque-Investigación%20forense-8B5CF6?style=for-the-badge)

</div>

> Una vez se confirma la presencia de un incidente, es necesario investigar de forma ordenada, preservando la evidencia, comprendiendo la causa y definiendo la mejor respuesta. La investigación es la base para la contención, la recuperación y la mejora del sistema.

## 1. Introducción

La investigación del incidente implica la recogida, custodia, análisis y contextualización de la evidencia asociada a un ataque o una anomalía de seguridad. No se trata de una simple revisión de registros: requiere rigor metodológico, trazabilidad y control del entorno para no alterar la evidencia.

En esta unidad se trabaja sobre varios ejes:

- recopilación segura de evidencias,
- análisis forense,
- investigación de la causa raíz,
- intercambio de información con proveedores u organismos,
- medidas de contención.

## 2. Resultado de aprendizaje y criterios

### Resultado de aprendizaje 3

Investiga incidentes de ciberseguridad analizando los riesgos implicados y definiendo las posibles medidas a adoptar.

### Criterios de evaluación

1. Recopila y almacena evidencias de forma segura.
2. Analiza evidencias e investiga el incidente.
3. Intercambia información del incidente con proveedores u organismos competentes.
4. Aplica medidas de contención del incidente.

## 3. Principios fundamentales de la investigación

### 3.1. Integridad de la evidencia

La evidencia debe mantenerse inalterada desde que se recoge hasta que se presenta o se utiliza en un proceso formal.

### 3.2. Cadena de custodia

Debe registrarse:

- quién recoge la evidencia,
- cuándo se recoge,
- dónde está guardada,
- quién la ha manipulado,
- por qué se ha movido o analizado.

### 3.3. Orden de volatilidad

Se prioriza la captura de datos más volátiles primero:

- memoria RAM,
- conexiones activas,
- procesos en ejecución,
- archivos temporales,
- registros del sistema,
- disco duro,
- copias de seguridad.

### 3.4. No contaminación

Se debe evitar modificar el estado original del sistema. Por eso, la investigación suele realizarse sobre imágenes forenses, snapshots o entornos aislados.

## 4. Fases de la investigación del incidente

```mermaid
flowchart LR
A[Detección y validación] --> B[Preservación de evidencia]
B --> C[Recopilación]
C --> D[Análisis técnico]
D --> E[Determinación de causa raíz]
E --> F[Contención y recuperación]
F --> G[Documentación y cierre]
```

## 5. Recopilación de evidencias

### 5.1. Evidencias de red

- PCAPs,
- logs de firewall,
- DNS,
- conexiones salientes,
- tráfico sospechoso,
- paquetes relevantes.

### 5.2. Evidencias de sistema

- hashes de archivos,
- logs del sistema operativo,
- servicios activos,
- usuarios creados,
- cronjobs,
- cambios de configuración.

### 5.3. Evidencias de endpoint

- procesos activos,
- tareas programadas,
- archivos ejecutables,
- artefactos de persistencia,
- EDR y antivirus,
- listas de ejecuciones.

### 5.4. Evidencias de aplicaciones

- registros de autenticación,
- cambios en bases de datos,
- trazas de acceso,
- documentos accesados,
- configuración de la aplicación.

### 5.5. Evidencias de seguridad física

- registro de accesos,
- grabaciones de cámaras,
- dispositivos vinculados,
- ubicación de equipos.

## 6. Técnicas y herramientas de análisis

### 6.1. Herramientas de análisis forense

- Wireshark
- Autopsy
- FTK Imager
- Volatility
- Strings
- MD5/SHA256
- OSQuery
- Sysinternals Suite

### 6.2. Hashing y integridad

La verificación de integridad en la evidencia se realiza mediante hashes. Ejemplo:

```bash
sha256sum archivo_sospechoso.bin
```

### 6.3. Análisis de memoria

La RAM puede contener:

- procesos activos,
- credenciales,
- conexiones,
- artefactos de malware,
- comandos ejecutados.

## 7. Métodos de investigación

### 7.1. Análisis de causa raíz

Se busca responder a:

- ¿Qué ocurrió?
- ¿Cómo entró el atacante?
- ¿Qué objetivo tenía?
- ¿Qué herramientas usó?
- ¿Qué impacto tuvo?
- ¿Qué controles fallaron?

### 7.2. Timeline

La línea temporal organiza hechos en orden cronológico para construir la narrativa del incidente.

| Fecha/hora | Evento | Evidencia | Observación |
| --- | --- | --- | --- |
| 08:10 | Acceso anómalo | Log de VPN | IP no reconocida |
| 08:14 | Elevación de privilegios | Seguridad del sistema | Cambio de rol |
| 08:18 | Ejecución de script | Endpoint log | Artefacto sospechoso |
| 08:22 | Cifrado de archivos | EDR | Indicador de ransomware |

## 8. Intercambio de información

### 8.1. ¿Por qué es necesario compartir información?

Cuando el incidente afecta a proveedores, infraestructura de terceros o entidades reguladoras, es necesario compartir información para:

- validar indicadores,
- reducir riesgos,
- coordinar respuesta,
- recibir soporte técnico,
- cumplir obligaciones legales.

### 8.2. Agentes con los que se puede intercambiar información

- proveedores de seguridad,
- servicio de telecomunicaciones,
- proveedores cloud,
- autoridades competentes,
- equipos internos de seguridad,
- fuerza de seguridad de la organización.

### 8.3. Qué se puede compartir

- IOCs: indicadores de compromiso,
- direcciones IP,
- hashes,
- nombres de dominio,
- patrones de correo,
- artefactos,
- informe técnico inicial.

## 9. Contención y mitigación

La investigación no termina con la explicación del incidente: debe conducir a medidas prácticas para detener la amenaza.

### Aislamiento

- desconectar equipos afectados,
- bloquear accesos a red o VPN,
- cortar conexiones sospechosas,
- limitar servicios críticos.

### Erradicación

- eliminar malware,
- limpiar herramientas maliciosas,
- reparar servicios afectados,
- corregir vulnerabilidades.

### Recuperación

- restaurar desde imágenes limpias,
- validar integridad,
- comprobar servicios,
- incorporar controles nuevos.

## 10. Ejemplos prácticos

### 10.1. Análisis básico de un archivo sospechoso

```bash
file archivo_sospechoso.exe
sha256sum archivo_sospechoso.exe
strings -n 8 archivo_sospechoso.exe | head -n 50
```

### 10.2. Verificación de conexiones sospechosas

```bash
ss -tulpn | grep -E ':80|:443|:22|:3389'
netstat -ano | findstr LISTENING
```

### 10.3. Script básico para recoger metadatos

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

## 11. Ejercicios de consolidación

### Ejercicio 1. Cadena de custodia

Imagina que un técnico recoge un equipo sospechoso. Redacta la cadena de custodia con: quién, qué, cuándo, dónde, motivo y acceso posterior.

### Ejercicio 2. Caso forense

Un usuario ha recibido un correo con un archivo ejecutable. ¿Qué evidencias vas a recoger primero?

#### Solución orientativa

- archivo adjunto,
- correo original,
- headers del mensaje,
- logs del correo,
- memoria o proceso si ya se ejecutó,
- sistema y red asociados.

### Ejercicio 3. Respuesta ante malware

La máquina de un usuario muestra comportamiento anómalo. ¿Qué decisión tomas primero: aislar, investigar o recuperar?

#### Solución orientativa

Primero aislar para evitar propagación; después preservar evidencia y analizar.

### Ejercicio 4. Análisis de causa raíz

Describe qué preguntas harías para investigar si un acceso no autorizado se produjo desde una cuenta de administrador.

#### Solución orientativa

- ¿Se produjo por phishing?
- ¿Hubo reutilización de credenciales?
- ¿Existen registros de MFA fallidos?
- ¿Se usó un token o soporte externo?
- ¿Se aplicó un cambio en la política de acceso?

## 12. Actividades prácticas recomendadas

- análisis de un sospechoso en entorno virtual,
- captura y validación de un paquete de red,
- extracción de hash y verificación de integridad,
- análisis de logs de VPN y autenticación,
- preparación de una línea temporal.

## 13. Resumen

La investigación del incidente es la fase que convierte la sospecha en conocimiento. Para actuar de forma efectiva, la organización debe preservar la evidencia, evitar contaminarla, reconstruir la secuencia de eventos y decidir la mejor respuesta técnica y organizativa.

## 14. Recursos recomendados

- TeoríaUD3-04-Intercambio de información.pdf
- TeoríaUD3-05-Respuesta al incidente.pdf

## 15. Autoevaluación

1. ¿Qué es la cadena de custodia y por qué es esencial?
2. ¿Qué tipo de evidencia se prioriza en una investigación?
3. ¿Qué son los IOCs y para qué sirven?
4. ¿Qué diferencias hay entre contención, erradicación y recuperación?
5. ¿Por qué es necesario documentar la investigación?

---

<p align="center">
  <strong>La investigación del incidente no busca solo confirmar lo ocurrido, sino comprender la causa raíz para evitar repetirlo.</strong>
</p>
