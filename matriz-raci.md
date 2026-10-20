# 👥 Matriz RACI

> **R** = Responsable (ejecuta) · **A** = Aprobador (único por tarea) · **C** = Consultado · **I** = Informado

## Roles del proyecto

| Rol | Persona asignada |
|-----|-----------------|
| Director / Líder de Proyecto (PM)| [COMPLETAR] |
| Responsable de Hardware e Infraestructura de Campo | [COMPLETAR] |
| Responsable de Software e IA | [COMPLETAR] |
| Especialista en Bioacústica y Conservación/Especialista en Biodiversidad / Asesor ambiental | [COMPLETAR] |
| Responsable de Datos y Visualización | [COMPLETAR] |

## Matriz

| ID | Tarea | Director | Responsable de Hardware | Responsable de Software | Especialista en Bioacústica | Responsable de Datos |
|----|-------|:-------:|:-------:|:-------:|:-------:|:-------:|
| 1.1 | Estandarización de parámetros de audio | I | C | R/A | R | C | 
| 1.2.1 | Sistema de alimentación autónomo | I | R/A | C | I  | I |
| 1.2.2 | Micrófono, placa, SD, gabinete y soportes | I | R/A | C | C | I |
| 1.3.1 | Integración de micrófono y placa comercial | I | R/A | R | I | I |
| 1.3.2 | Configuración de firmware y almacenamiento SD | I | R/A | R | C | C |
| 1.3.3 | Montaje y comprobación de funcionamiento | I | R/A | C | C | C |
| 1.4 | Pruebas de autonomía y funcionamiento en campo | I | R/A | I | R | C |
| 2.1.1 | Diseño de esquema de datos y metadatos | I | I | C | C | R/A |
| 2.2.1 | Algoritmo de cálculo NDSI y ACI | I | I | R/A | C | C |
| 2.2.2 | Clasificador binario Aves vs Perturbación | I | I | R/A | C | I |
| 2.3.1 | Mapa interactivo de puntos de muestreo| I | I | C | C | R/A |
| 2.3.2 | Panel de visualización de indicadores | I | I | I | C | R/A |
| 3.1 | Estandarización del dataset acústico | I | I | C | R/A | C |
| 3.2 | Análisis comparativo zona conservada vs urbana | I | I | C | R/A | R |
| 3.3.1 | Elaboración de informe ambiental para el Sponsor | A | I | I | R | C |
| 4.1.1 | Acta de constitución y alcance | R/A | C | C | C | C |
| 4.1.2 | WBS, cronograma y RACI | R/A | C | C | C | C |
| 4.2 | Seguimiento y control | R/A | C | C | C | C |
| 4.3 | Cierre | R/A | I | I | I | I |

> ⚠️ **Verificación obligatoria:** cada fila debe tener exactamente **1 A** y al menos **1 R**.

## Análisis de carga de responsabilidades

```mermaid
xychart-beta
    title "Cantidad de tareas por rol (R + A)"
    x-axis ["Director", "Resp. Hardware", "Resp. Software e IA", "Esp. Bioacustica", "Resp. Datos/visualizacion"]
    y-axis "Nº de tareas" 0 --> 12
    bar [9, 12, 8, 7, 7]
```

La matriz logra un equilibrio funcional dinámico: no existe solapamiento excesivo de ejecución primaria ($R$) en un mismo hito temporal para ningún perfil. La co-responsabilidad en tareas complejas (como la integración firmware/hardware en 1.3 o la elaboración del informe final en 3.3) previene cuellos de botella y promueve el trabajo interdisciplinario.

---

*Cátedra Gestión de Proyectos · FIUNER · 2026*
