# 🔗 Red de Tareas y Camino Crítico

## Diagrama de precedencias

> Las tareas del **Camino Crítico** se muestran en rojo (holgura = 0).

```mermaid
flowchart LR
    START(["▶ INICIO"])
    T11["1.1 [Tarea]\n⏱ Xd"]
    T12["1.2 [Tarea]\n⏱ Xd"]
    T13["1.3 [Tarea]\n⏱ Xd"]
    T21["2.1 [Tarea]\n⏱ Xd"]
    T22["2.2 [Tarea]\n⏱ Xd"]
    T23["2.3 [Tarea]\n⏱ Xd"]
    T31["3.1 [Tarea]\n⏱ Xd"]
    T32["3.2 [Tarea]\n⏱ Xd"]
    END(["⏹ FIN"])

    START --> T11
    T11 --> T12
    T11 --> T13
    T12 --> T21
    T13 --> T21
    T21 --> T22
    T21 --> T23
    T22 --> T31
    T23 --> T31
    T31 --> T32
    T32 --> END

    style T11 fill:#FFCCCC,stroke:#C62828
    style T12 fill:#FFCCCC,stroke:#C62828
    style T21 fill:#FFCCCC,stroke:#C62828
    style T22 fill:#FFCCCC,stroke:#C62828
    style T31 fill:#FFCCCC,stroke:#C62828
    style T32 fill:#FFCCCC,stroke:#C62828
```

## Análisis del Camino Crítico

| ID | Tarea | Inicio Temprano | Fin Temprano | Inicio Tardío | Fin Tardío | Holgura | ¿Crítica? |
|----|-------|:-:|:-:|:-:|:-:|:-:|:-:|
| 1.1 | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | 0 | ✅ |
| 1.2 | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | 0 | ✅ |
| 1.3 | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [X] | ❌ |
| 2.1 | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | 0 | ✅ |
| 2.2 | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | 0 | ✅ |
| 2.3 | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [X] | ❌ |

**Duración total del proyecto:** [COMPLETAR] días

**Camino Crítico:** `INICIO → 1.1 → 1.2 → 2.1 → 2.2 → 3.1 → 3.2 → FIN`

---

*Cátedra Gestión de Proyectos · FIUNER · 2026*
