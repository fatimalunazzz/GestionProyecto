# 📅 Cronograma del Proyecto

## Diagrama de Gantt

```mermaid
gantt
    title Cronograma - Nombre del Proyecto
    dateFormat  YYYY-MM-DD
    excludes    weekends

    section Fase 1 - Nombre
    Tarea 1.1               :t11, 2026-04-01, 5d
    Tarea 1.2               :t12, after t11, 7d
    Tarea 1.3               :t13, after t12, 3d
    Hito - Fin Fase 1       :milestone, m1, after t13, 0d

    section Fase 2 - Nombre
    Tarea 2.1               :t21, after m1, 10d
    Tarea 2.2               :t22, after t21, 5d
    Tarea 2.3               :t23, after t21, 8d
    Hito - Fin Fase 2       :milestone, m2, after t22, 0d

    section Fase 3 - Nombre
    Tarea 3.1               :t31, after m2, 6d
    Tarea 3.2               :t32, after t31, 4d
    Hito - Cierre           :milestone, m3, after t32, 0d

    section Gestion
    Planificacion           :g1, 2026-04-01, 5d
    Seguimiento y Control   :g2, after g1, 45d
    Cierre                  :g3, after t32, 3d
```

## Tabla de tareas

| ID | Tarea | Predecesoras | Responsable | Duración (días) | Inicio | Fin | Hito |
|----|-------|-------------|------------|----------------|--------|-----|------|
| 1.1 | [COMPLETAR] | — | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | No |
| 1.2 | [COMPLETAR] | 1.1 | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | No |
| 1.3 | [COMPLETAR] | 1.2 | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | No |
| M1 | 🏁 Fin Fase 1 | 1.3 | — | 0 | [COMPLETAR] | [COMPLETAR] | **Sí** |
| 2.1 | [COMPLETAR] | M1 | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | No |
| 2.2 | [COMPLETAR] | 2.1 | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | No |
| 2.3 | [COMPLETAR] | 2.1 | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] | No |
| M2 | 🏁 Fin Fase 2 | 2.2, 2.3 | — | 0 | [COMPLETAR] | [COMPLETAR] | **Sí** |

---

*Cátedra Gestión de Proyectos · FIUNER · 2026*
