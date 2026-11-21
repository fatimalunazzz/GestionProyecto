
# Plan de Comunicaciones y Registro de Interesados


## 1. Necesidades de Información por Interesado

| Interesado / Rol | Información Requerida | Propósito de la Información | Nivel de Detalle | Frecuencia Requerida |
|:---|:---|:---|:---:|:---:|
| **Director / PM** | Avance físico y financiero, métricas de desempeño (SPI/CPI), riesgos activos, desvíos y solicitudes de cambio. | Coordinar la ejecución global, tomar decisiones correctivas y asegurar el cumplimiento de la línea base. | **Alto** | Continua / Semanal |
| **Sponsor (Secretaría de Ambiente / CAUCE)** | Cumplimiento de hitos principales, ejecución presupuestaria, informes de diagnóstico bioacústico y fechas de entrega. | Validar la inversión, justificar fondos públicos y asegurar los resultados de conservación ambiental. | **Bajo (Sintético)** | Quincenal / Por Hito |
| **Responsable de Hardware (HW)** | Especificaciones de componentes COTS, diseño de gabinete IP65, dependencias de la WBS, asignación de horas y pruebas de campo. | Ensamble, configuración del firmware, calibración del micrófono y pruebas de autonomía de 48h. | **Alto** | Semanal / Diaria |
| **Responsable de Software e IA (SW)** | Requisitos de señales de audio, estandarización de formato, dataset de entrenamiento y métricas del clasificador (aves vs. perturbación). | Desarrollar algoritmos de índices NDSI/ACI y entrenar el modelo de aprendizaje automático. | **Alto** | Semanal / Diaria |
| **Especialista en Bioacústica (BIO)** | Protocolos de grabación (duración, ventanas y horarios), bandas espectrales para índices y calidad del audio de campo. | Estandarizar la metodología científica, validar los datasets y redactar el informe ambiental para el Sponsor. | **Alto** | Por Hito / Semanal |
| **Responsable de Datos (DAT)** | Esquemas de datos y metadatos, estructura de la base de datos local, endpoints de visualización y coordenadas de muestreo. | Diseñar la base de datos local, implementar el mapa interactivo georreferenciado y el dashboard de indicadores. | **Alto** | Semanal |
| **Gestión de Calidad / Cátedra FIUNER** | Cumplimiento de metodologías PMBOK, consistencia entre WBS, RACI y Gantt, y calidad formal de documentos del proyecto. | Auditar el progreso del proyecto integrador, evaluar entregables y autorizar hitos de gobernanza. | **Alto** | Previa a cada Entrega |
| **Usuario Final (Municipios / Guardaparques)** | Usabilidad de la interfaz web, localización de estaciones en campo, alertas de perturbación y guía de consulta de datos. | Operar la plataforma web, interpretar mapas acústicos y utilizar los resultados en ordenamiento territorial. | **Medio** | Demostraciones / Al finalizar prototipo |

---


## 2. Tabla de Comunicaciones

| Información | Contenido | Formato | Nivel de Detalle | Responsable | Grupo Receptor | Canal | Metodología / Herramienta | Frecuencia |
|:---|:---|:---:|:---:|:---|:---|:---|:---|:---:|
| **Reunión de Avance Semanal** | Estado de tareas en desarrollo, resolución de bloqueos técnicos, avance en la WBS y asignación de actividades. | Minuta / Markdown | **Alto** | Director de Proyecto (PM) | Equipo Técnico (HW, SW, DAT, BIO) | Google Meet / Presencial | GitHub Projects / Standup | **Semanal** |
| **Reporte Ejecutivo de Hitos** | Síntesis de cumplimiento de hitos, estado financiero, riesgos consolidados y avances clave. | Presentación / PDF | **Bajo** | Director de Proyecto (PM) | Sponsor Estatal (Secretaría de Ambiente) | Reunión Virtual / Email | Google Meet / Minuta Ejecutiva | **Quincenal / Por Hito** |
| **Informe de Avance Mensual** | Avance general, tareas completadas vs. planificadas, desvíos observados, acciones correctivas y KPIs (SPI/CPI). | Documento Word / PDF | **Medio** | Director de Proyecto (PM) | Equipo Operativo, Cátedra y Sponsor | Correo Electrónico / Repositorio | Plantilla Oficial de Avance | **Mensual** |
| **Sincronización Técnica y Commits** | Revisión de código, esquemas de base de datos, scripts matemáticos y documentación técnica. | Código / Markdown | **Alto** | Responsables de HW, SW, DAT, BIO | Equipo de Desarrollo Técnico | Repositorio GitHub | GitHub Issues / Pull Requests | **Diaria / Continua** |
| **Validación Metodológica Bioacústica** | Definición de parámetros de audio, bandas para NDSI/ACI y precisión del modelo de IA (aves vs. ruido). | Ficha Técnica / Word | **Alto** | Especialista en Bioacústica | Equipo SW, DAT y PM | Reunión Técnica / Drive | Google Meet / Docs Colaborativo | **Por Hito / Según necesidad** |
| **Auditoría de Calidad y Entregables** | Verificación de concordancia entre WBS, RACI, Gantt y matriz de riesgos según estándar PMBOK. | Documento / Checklist | **Alto** | Gestión de Calidad / PM | Cátedra FIUNER / Equipo | Repositorio GitHub | Checklist de Auditoría Metodológica | **Previa a cada Entrega** |
| **Demostración Práctica (Showcase)** | Demostración interactiva de la plataforma web, mapa de muestreo y prototipo físico de grabación. | Demostración Oral | **Medio** | Director de Proyecto (PM) / Equipo | Usuarios Finales (Municipios / Guardaparques) | Taller Presencial / Demo Virtual | Google Meet / Taller en Campo | **Puntual / Al finalizar prototipo** |
| **Control de Cambios y Solicitudes** | Justificación del cambio, análisis de impacto en alcance/tiempo/costo y resolución del comité. | Formulario de Cambio | **Alto** | Solicitante / PM | Comité de Control de Cambios | Repositorio GitHub / Email | Formulario Estándar de Cambio | **Eventual / Cuando ocurra** |

---

## 3. Repositorio de Comunicaciones

El repositorio central del proyecto está alojado en **GitHub** bajo la estructura del proyecto `fatimalunazzz/GestionProyecto`. Define las reglas de almacenamiento, versión y acceso de la información:

1. **Almacenamiento de Artefactos de Gestión:**
   * Todos los documentos de gestión (`organizacion.md`, `ciclo-de-vida.md`, `wbs.md`, `red-de-tareas-v4.md`, `matriz-raci-v2.md`, `asignacion-recursos.md`, `plan-comunicaciones.md`) se almacenan en la raíz del repositorio en formato Markdown UTF-8.
2. **Control de Versiones:**
   * Las actualizaciones de los artefactos principales se controlan mediante commits explícitos y sufijos de versión (`_v2`, `_v3`, `_v4`) para mantener trazabilidad histórica de los cambios.
3. **Modelos y Hojas de Cálculo:**
   * Los libros de cálculo de estimación Delphi, Cronograma Gantt y Gestión de Riesgos (`estimacion_delphi_wbs.xlsx`, `cronograma_gantt_v3.xlsx`, `plan_respuesta_riesgos_simabpa.xlsx`, `evolucion_riesgos_simabpa.xlsx`) se guardan en el repositorio en formato binario interoperable.
4. **Comunicaciones y Minutas:**
   * Las minutas de reuniones semanales y los registros de decisiones se publican en las Secciones de Issues/Projects de GitHub y en documentos Markdown dentro del repositorio.
5. **Políticas de Acceso y Resguardo:**
   * **Acceso de Escritura:** Exclusivo para los integrantes del equipo del proyecto.
   * **Acceso de Lectura:** Público para auditoría de la Cátedra de Gestión de Proyectos (FIUNER) y consulta de interesados.
   * **Respaldos:** Sincronización continua en la nube a través de la infraestructura distribuida de GitHub.

---

## PARTE A — Registro e Identificación de Interesados

*Escala — Influencia e Interés: A = Alta · M = Media · B = Baja*

| Interesado | Rol en el proyecto | Influencia (A / M / B) | Interés (A / M / B) | ¿Qué necesita saber? | Observaciones / Estrategia |
|:---|:---|:---:|:---:|:---|:---|
| **Director / PM** | Coordinación General y Líder de Proyecto | **A** | **A** | Avances y estado del proyecto, desvíos de presupuesto y riesgos. | **Gestión atenta:** Monitoreo continuo mediante tableros de control y minutas de seguimiento. |
| **Sponsor (CAUCE)** | Patrocinador Financiero e Institucional | **A** | **A** | Finalización de cada etapa (cumplimiento de hitos), destino del presupuesto, informe bioacústico y fechas de cierre. | **Mantener satisfecho:** Reportes sintéticos quincenales (no técnicos) y reuniones de avance formal. |
| **Resp Hardware** | Desarrolladores y Ejecutores Técnicos | **M** | **A** | Parámetros técnicos a tener en cuenta. Requisitos detallados, dependencias de tareas en el WBS, asignación de horas y calibración. | **Mantener involucrados:** Coordinación técnica directa y sincronización continua en el repositorio de GitHub. |
| **Resp Software** | Desarrolladores y Ejecutores Técnicos | **M** | **A** | Parámetros técnicos a tener en cuenta. Requisitos detallados, dependencias de tareas en el WBS, asignación de horas y calibración. | **Mantener involucrados:** Coordinación técnica directa y sincronización continua en el repositorio de GitHub. |
| **Especialista en Bioacústica** | Experto de Dominio Científico | **B** | **A** | Planificación y lugar. Parámetros de audio, calidad de los datos acústicos grabados y metodología de índices (NDSI/ACI). | **Consultar activamente:** Validaciones metodológicas de los dataset y supervisión del informe ambiental. |
| **Resp de Datos** | Desarrolladores y Ejecutores Técnicos | **M** | **A** | Requisitos detallados, dependencias de tareas en el WBS, asignación de horas y calibración. | **Mantener involucrados:** Coordinación técnica directa y sincronización continua en el repositorio de GitHub. |
| **Gestión de Calidad** | Auditor Metodológico Interno | **M** | **A** | Estadío y entregables. Cumplimiento de estándares de entregables, pruebas de sistema y validación de requisitos. | **Asegurar cumplimiento:** Revisiones y aprobaciones formales previa entrega de cada hito de gobernanza. |
| **Usuario (Municipio / Guardaparques)** | Beneficiario Operativo en Reserva | **A** | **A** | Implementación Práctica. Usabilidad del mapa interactivo, ubicación física de los nodos de campo y alertas de perturbación. | **Mantener informado:** Demostraciones prácticas (*showcases*), capacitaciones sencillas y feedback de interfaz. |

---

## PARTE B — Plan de Gestión de las Comunicaciones

| Información | Contenido | Formato | Nivel de Detalle | Responsable | Grupo Receptor | Canal | Metodología / Herramienta | Frecuencia |
|:---|:---|:---:|:---:|:---|:---|:---|:---|:---|
| **Informe de avance mensual** | Estado general del proyecto, tareas completadas vs. planificadas, problemas/desvíos, acciones correctivas y KPIs. | Documento en formato word/PDF | **Medio** | Director del proyecto (PM) | Equipo operativo y Sponsor | Correo electrónico | Planilla oficial de avance | **Mensual** |
| **Informe avance semanal** | Información sobre avances técnicos, decisiones requeridas, incidentes resueltos, incidentes no resueltos. | Documento / Plantilla | **Alto** | Software / Hardware / Bioacústica / Datos | Director del proyecto y gestión de calidad | Correo electrónico | Plantilla | **Semanal** |
| **Reporte ejecutivo de Hitos** | Resumen de alto nivel sobre cumplimiento de hitos, estado financiero, riesgos críticos y decisiones requeridas. | Presentación / PDF | **Bajo** | Director del proyecto | Sponsor estatal (Secretaría de Ambiente) | Reunión virtual / Correo electrónico | Google Meet / Zoom / Minuta ejecutiva | **Quincenal / Por hito** |
| **Sincronización técnica semanal** | Revisión de tareas en desarrollo, resolución y avance sobre bloqueos, asignación de dependencias del WBS. | Documento de texto / Markdown | **Alto** | Responsables de hardware, software, datos y especialista de biodiversidad | Equipos de desarrollo técnico | Repositorio | GitHub projects o issues / Asana | **Semanal** |
| **Validación metodológica y calibración** | Estandarización de audio, parámetros para NDSI/ACI y precisión del modelo de IA. | Ficha técnica / Word | **Alto** | Especialista en Bioacústica | Equipo de software (resp. de software y en datos) | Reunión técnica / Drive | Meet / Documento colaborativo | **Por hito / Según necesidad** |
| **Integración de Base de Datos y Plataforma** | Definición de esquemas de datos, puntos del mapa interactivo y dashboard de indicadores. | Ficha técnica / Web | **Alto** | Responsable de Datos y Visualización | Equipo de software (resp. de software y en datos) | Repositorio | GitHub | **Semanal** |
| **Auditoría de Calidad y Entregables** | Verificación de concordancia entre WBS, RACI, Gantt y cumplimiento de criterios de aceptación PMBOK. | Documento / Checklist | **Alto** | Gestión de Calidad / PM | Equipo / Sponsor | Repositorio | Checklist de Auditoría Metodológica | **Previa a cada entrega** |
| **Demostración Práctica** | Presentación interactiva de la plataforma web, mapa de muestreo y prototipo de grabación autónoma. | Demostración Oral / Presentación | **Medio** | Director de Proyecto (PM) / Equipo | Usuarios Finales (Municipios / Guardaparques) | Taller Presencial / Demo Virtual | Google Meet / Taller en Campo | **Al finalizar prototipo** |
| **Solicitud y Control de Cambios** | Justificación del cambio, impacto en alcance / tiempo / costo y resolución del comité de control. | Formulario de Cambio / Word | **Alto** | Integrante que lo solicite / PM | Comité de Control de Cambios / Equipo | Repositorio GitHub / Correo electrónico | Formulario de cambio | **Eventual / Cuando ocurra** |

---
*Cátedra Gestión de Proyectos · FIUNER · 2026*
