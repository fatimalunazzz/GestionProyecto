# 📅 Cronograma del Proyecto

## Diagrama de Gantt

```mermaid
gantt
    title Cronograma 
    dateFormat  YYYY-MM-DD
    excludes    weekends

    section Fase 1 - Dispositivo Autónomo (Hardware & Campo)
    Estandarización de parámetros de audio (1.1.1)     :crit, t111, after t411, 3d
    Sistema de alimentación autónomo (1.2.1)           :t121, after t111, 3d
    Micrófono, placa, SD, gabinete y soportes (1.2.2)  :crit, t122, after t111, 3d
    Integración de micrófono y placa comercial (1.3.1) :t131, after t121 t122, 3d
    Configuración de firmware y almacenamiento SD (1.3.2) :crit, t132, after t122, 4d
    Montaje y comprobación de funcionamiento (1.3.3)   :crit, t133, after t131 t132, 3d
    Pruebas de autonomía y funcionamiento en campo (1.4):crit, t14, after t133, 6d
    🏁 Fin Fase 1 - Dispositivo y Campo                :milestone, m1, after t14, 0d

    section Fase 2 - Plataforma de Visualización (Software & IA)
    Diseño de esquema de datos y metadatos (2.1.1)     :t211, after t411, 3d
    Algoritmo de cálculo NDSI y ACI (2.2.1)            :t221, after t111, 4d
    Mapa interactivo de puntos de muestreo (2.3.1)     :t231, after t211, 5d
    Panel de visualización de indicadores (2.3.2)      :t232, after t211 t221 t231, 5d
    Clasificador binario Aves vs. Perturbación (2.2.2) :crit, t222, after t31, 7d
    🏁 Fin Fase 2 - Plataforma de Visualización e IA   :milestone, m2, after t222 t232, 0d

    section Fase 3 - Informe de Diagnóstico Bioacústico
    Estandarización del dataset acústico (3.1)         :crit, t31, after t14, 3d
    Análisis comparativo zona conservada vs. urbana (3.2):crit, t32, after t31 t222, 3d
    Elaboración de informe ambiental para Sponsor (3.3.1):crit, t331, after t32, 3d
    🏁 Fin Fase 3 - Informe de Diagnóstico Final       :milestone, m3, after t331, 0d

    section Gestión del Proyecto (Gobernanza & Control)
    Acta de constitución y alcance (4.1.1)             :crit, t411, 2026-04-01, 3d
    WBS, Cronograma y RACI (4.1.2)                     :t412, after t411, 4d
    Seguimiento y Control (4.2)                        :t42, after t412, 4d
    Cierre del Proyecto (4.3)                          :crit, t43, after m1 m2 m3 t42, 2d
    🏁 Cierre Definitivo del Proyecto SiMABPA          :milestone, m4, after t43, 0d
```

## Tabla de tareas

| ID | Tarea | Predecesoras | Responsable | Duración (días) | Inicio | Fin | Hito |
|----|-------|-------------|------------|----------------|--------|-----|------|
| 4.1.1 | Acta de constitución y alcance | — | Director de Proyecto (PM) | 3 | 2026-04-01 | 2026-04-03 | No |
| 4.1.2 | WBS, Cronograma y RACI | 4.1.1 | Director de Proyecto (PM) | 4 | 2026-04-06 | 2026-04-09 | No |
| 1.1.1 | Estandarización de parámetros de audio | 4.1.1 | Especialista en Bioacústica | 3 | 2026-04-06 | 2026-04-08 | No |
| 1.2.1 | Sistema de alimentación autónomo | 1.1.1 | Responsable de Hardware | 3 | 2026-04-09 | 2026-04-13 | No |
| 1.2.2 | Micrófono, placa, SD, gabinete y soportes | 1.1.1 | Responsable de Hardware | 3 | 2026-04-09 | 2026-04-13 | No |
| 1.3.1 | Integración de micrófono y placa comercial | 1.2.1, 1.2.2 | Responsable de Hardware | 3 | 2026-04-14 | 2026-04-16 | No |
| 1.3.2 | Configuración de firmware y almacenamiento SD | 1.2.2 | Responsable de Hardware | 4 | 2026-04-14 | 2026-04-17 | No |
| 1.3.3 | Montaje y comprobación de funcionamiento | 1.3.1, 1.3.2 | Resp. Hardware e Infraestructura | 3 | 2026-04-20 | 2026-04-22 | No |
| 1.4 | Pruebas de autonomía y funcionamiento en campo | 1.3.3 | Resp. Hardware e Infraestructura | 6 | 2026-04-23 | 2026-04-30 | No |
| M1 | 🏁 Fin Fase 1 - Hardware y Campo | 1.4 | — | 0 | 2026-04-30 | 2026-04-30 | **Sí** |
| 2.1.1 | Diseño de esquema de datos y metadatos | 4.1.1 | Resp. Datos y Visualización | 3 | 2026-04-06 | 2026-04-08 | No |
| 2.2.1 | Algoritmo de cálculo NDSI y ACI | 1.1.1 | Responsable de Software e IA | 4 | 2026-04-09 | 2026-04-14 | No |
| 2.3.1 | Mapa interactivo de puntos de muestreo | 2.1.1 | Resp. Datos y Visualización | 5 | 2026-04-09 | 2026-04-15 | No |
| 2.3.2 | Panel de visualización de indicadores | 2.1.1, 2.2.1, 2.3.1 | Resp. Datos y Visualización | 5 | 2026-04-16 | 2026-04-22 | No |
| 2.2.2 | Clasificador binario Aves vs. Perturbación | 3.1 | Responsable de Software e IA | 7 | 2026-05-06 | 2026-05-14 | No |
| M2 | 🏁 Fin Fase 2 - Plataforma de Visualización e IA | 2.2.2, 2.3.2 | — | 0 | 2026-05-14 | 2026-05-14 | **Sí** |
| 3.1 | Estandarización del dataset acústico | 1.4 | Especialista en Bioacústica | 3 | 2026-05-01 | 2026-05-05 | No |
| 3.2 | Análisis comparativo zona conservada vs. urbana | 3.1, 2.2.1, 2.2.2 | Especialista en Bioacústica | 3 | 2026-05-15 | 2026-05-19 | No |
| 3.3.1 | Elaboración de informe ambiental para Sponsor | 3.2 | Especialista en Bioacústica / PM | 3 | 2026-05-20 | 2026-05-22 | No |
| M3 | 🏁 Fin Fase 3 - Informe de Diagnóstico Bioacústico | 3.3.1 | — | 0 | 2026-05-22 | 2026-05-22 | **Sí** |
| 4.2 | Seguimiento y Control | 4.1.2 | Director de Proyecto (PM) | 4 | 2026-04-10 | 2026-04-15 | No |
| 4.3 | Cierre del Proyecto | 1.4, 2.3.2, 3.3.1, 4.2 | Director de Proyecto (PM) | 2 | 2026-05-25 | 2026-05-26 | No |
| M4 | 🏁 Cierre Definitivo del Proyecto | 4.3 | — | 0 | 2026-05-26 | 2026-05-26 | **Sí** |

---
### Duración Total del Proyecto

* **En horas netas continuas (CPM exacto):** La suma exacta de la ruta crítica es de **297.8 horas** (\~**37.23 días hábiles**).
* **En días redondeados de trabajo directo:** La suma de los días enteros sobre el camino crítico asciende a **40 días hábiles**.
* **En el Cronograma Gantt (Cobertura Temporal):** La **duración total figura en 43 días**. Esta diferencia incluye la ventana de días no laborables (como feriados o días de descanso) dentro del calendario del proyecto
---
*Cátedra Gestión de Proyectos · FIUNER · 2026*
