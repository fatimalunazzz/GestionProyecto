# 🔗 Red de Tareas y Camino Crítico

## Diagrama de precedencias

> Las tareas del **Camino Crítico** se muestran en rojo (holgura = 0).

```mermaid
flowchart LR
START(["▶ INICIO"])
T411["4.1.1 Acta de constitución y alcance\\n⏱ 20.0h (2.5d) | σ 8.6h"]
T412["4.1.2 WBS, Cronograma y RACI\\n⏱ 26.0h (3.3d) | σ 8.5h"]
T111["1.1.1 Estandarización de parámetros de audio\\n⏱ 16.8h (2.1d) | σ 6.7h"]
T121["1.2.1 Sistema de alimentación autónomo\\n⏱ 17.6h (2.2d) | σ 7.9h"]
T122["1.2.2 Micrófono, placa, SD, gabinete y soportes\\n⏱ 16.4h (2.1d) | σ 1.7h"]
T131["1.3.1 Integración de micrófono y placa comercial\\n⏱ 19.2h (2.4d) | σ 8.3h"]
T132["1.3.2 Configuración firmware y almacenamiento SD\\n⏱ 31.2h (3.9d) | σ 13.4h"]
T133["1.3.3 Montaje y comprobación de funcionamiento\\n⏱ 16.4h (2.1d) | σ 5.7h"]
T14["1.4 Pruebas de autonomía en campo (48h)\\n⏱ 45.8h (5.7d) | σ 20.2h"]
T211["2.1.1 Diseño esquema de datos y metadatos\\n⏱ 23.6h (3.0d) | σ 7.4h"]
T221["2.2.1 Algoritmo de cálculo NDSI y ACI\\n⏱ 26.8h (3.4d) | σ 7.2h"]
T31["3.1 Estandarización del dataset acústico\\n⏱ 22.8h (2.9d) | σ 8.0h"]
T222["2.2.2 Clasificador binario Aves vs Perturbación\\n⏱ 52.8h (6.6d) | σ 16.8h"]
T231["2.3.1 Mapa interactivo de puntos de muestreo\\n⏱ 32.8h (4.1d) | σ 7.2h"]
T232["2.3.2 Panel de visualización de indicadores\\n⏱ 38.4h (4.8d) | σ 6.5h"]
T32["3.2 Análisis comparativo zona conservada vs urbana\\n⏱ 24.0h (3.0d) | σ 11.7h"]
T331["3.3.1 Elaboración de informe ambiental para Sponsor\\n⏱ 24.0h (3.0d) | σ 11.4h"]
T42["4.2 Seguimiento y Control\\n⏱ 30.8h (3.9d) | σ 10.0h"]
T43["4.3 Cierre del Proyecto\\n⏱ 10.0h (1.3d) | σ 3.5h"]
END(["⏹ FIN"])

START --&gt; T411
T411 --&gt; T412
T411 --&gt; T111
T411 --&gt; T211
T111 --&gt; T121
T111 --&gt; T122
T111 --&gt; T221
T121 --&gt; T131
T122 --&gt; T131
T122 --&gt; T132
T131 --&gt; T133
T132 --&gt; T133
T133 --&gt; T14
T14 --&gt; T31
T14 --&gt; T43
T211 --&gt; T231
T211 --&gt; T232
T221 --&gt; T232
T221 --&gt; T32
T231 --&gt; T232
T31 --&gt; T222
T31 --&gt; T32
T222 --&gt; T32
T32 --&gt; T331
T232 --&gt; T43
T331 --&gt; T43
T412 --&gt; T42
T42 --&gt; T43
T43 --&gt; END

style START fill:#E8F5E9,stroke:#2E7D32
style END fill:#ECEFF1,stroke:#37474F
style T411 fill:#FFCCCC,stroke:#C62828,color:#000000
style T111 fill:#FFCCCC,stroke:#C62828,color:#000000
style T122 fill:#FFCCCC,stroke:#C62828,color:#000000
style T132 fill:#FFCCCC,stroke:#C62828,color:#000000
style T133 fill:#FFCCCC,stroke:#C62828,color:#000000
style T14 fill:#FFCCCC,stroke:#C62828,color:#000000
style T31 fill:#FFCCCC,stroke:#C62828,color:#000000
style T222 fill:#FFCCCC,stroke:#C62828,color:#000000
style T32 fill:#FFCCCC,stroke:#C62828,color:#000000
style T331 fill:#FFCCCC,stroke:#C62828,color:#000000
style T43 fill:#FFCCCC,stroke:#C62828,color:#000000
```

## Análisis del Camino Crítico
| ID | Tarea | Inicio Temprano | Fin Temprano | Inicio Tardío | Fin Tardío | Holgura | ¿Crítica? |
|----|-------|:-:|:-:|:-:|:-:|:-:|:-:|
| 1.1.1 | Estandarización de parámetros de audio | 3 | 5 | 3 | 5 | 0 | SÍ |
| 1.2.1 | Sistema de alimentación autónomo | 5 | 7 | 5 | 7 | 0 | SÍ |
| 1.2.2 | Micrófono, placa comercial, almacenamiento SD, gabinete y soportes | 7 | 9 | 7 | 9 | 0 | SÍ |
| 1.3.1 | Integración de micrófono y placa comercial | 9 | 12 | 11 | 13 | 2 | NO |
| 1.3.2 | Configuración de firmware y almacenamiento SD | 9 | 13 | 9 | 13 | 0 | SÍ |
| 1.3.3 | Montaje y comprobación de funcionamiento | 13 | 15 | 13 | 15 | 0 | SÍ |
| 1.4 | Pruebas de autonomía y funcionamiento en campo | 15 | 21 | 15 | 21 | 0 | SÍ |
| 2.1.1 | Diseño de esquema de datos y metadatos | 5 | 8 | 25 | 28 | 20 | NO |
| 2.2.1 | Algoritmo de cálculo NDSI y ACI | 5 | 8 | 27 | 30 | 23 | NO |
| 2.2.2 | Clasificador binario Aves vs Perturbación | 24 | 30 | 24 | 30 | 0 | SÍ |
| 2.3.1 | Mapa interactivo de puntos de muestreo | 8 | 12 | 28 | 32 | 20 | NO |
| 2.3.2 | Panel de visualización de indicadores | 12 | 17 | 32 | 36 | 20 | NO |
| 3.1 | Estandarización del dataset acústico | 21 | 24 | 21 | 24 | 0 | SÍ |
| 3.2 | Análisis comparativo zona conservada vs urbana | 30 | 33 | 30 | 33 | 0 | SÍ |
| 3.3.1 | Elaboración de informe ambiental para el Sponsor | 33 | 36 | 33 | 36 | 0 | SÍ |
| 4.1.1 | Acta de constitución y alcance | 0 | 3 | 0 | 3 | 0 | SÍ |
| 4.1.2 | WBS, Cronograma y RACI | 3 | 6 | 29 | 33 | 27 | NO |
| 4.2 | Seguimiento y Control | 6 | 10 | 33 | 36 | 27 | NO |
| 4.3 | Cierre | 36 | 38 | 36 | 38 | 0 | SÍ |

**Relación hs/día:** 8 h/día (20 h = 2.5 d= 3 d)

**Duración total del proyecto:** 62 días (495.4 h)

**Duración total del proyecto con desvío:** 84 días (662.92 h)(3 meses)

**Camino Crítico:** `INICIO → 4.1.1 → 1.1.1 → 1.2.1 → 1.2.2 → 1.3.2 → 1.3.3 → 1.4 → 3.1 → 2.2.2 → 3.2 → 3.3.1 → 4.3 → FIN`

---

*Cátedra Gestión de Proyectos · FIUNER · 2026*
