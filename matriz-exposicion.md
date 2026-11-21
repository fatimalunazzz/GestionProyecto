# 📊 Matriz de Exposición al Riesgo

## Visualización

```mermaid
quadrantChart
    title Matriz de Exposición al Riesgo
    x-axis Baja Probabilidad --> Alta Probabilidad
    y-axis Bajo Impacto --> Alto Impacto
    quadrant-1 "🔴 Atención Inmediata"
    quadrant-2 "🟠 Monitorear"
    quadrant-3 "🟢 Aceptar"
    quadrant-4 "🟡 Plan de Contingencia"
    R1 —  Tormentas intensas: [0.6, 0.6]
    R2 — Fluctuaciones económicas: [0.8, 0.55]
    R3 — Falla clasificador: [0.75, 0.85]
    R4 — SD corrupta: [0.6, 0.9]
    R5 — Descarga electrostatica: [0.3, 0.8]
    R6 — Demoras importacion: [0.5, 0.4]
```

> **Cómo leer el gráfico:** cada punto representa un riesgo. El eje X es la probabilidad normalizada (valor/10) y el eje Y es el impacto normalizado (valor/10).

## Interpretación

| Cuadrante | Zona | Riesgos | Acción |
|-----------|------|---------|--------|
| Superior derecho | 🔴 Atención Inmediata | R1, R2, R3 y R4 | Mitigar o evitar activamente |
| Superior izquierdo | 🟠 Monitorear | R5 | Planificar contingencia |
| Inferior derecho | 🟡 Contingencia |  | Transferir o aceptar con plan |
| Inferior izquierdo | 🟢 Aceptar | R6 | Registrar y monitorear |

---

*Cátedra Gestión de Proyectos · FIUNER · 2026*
