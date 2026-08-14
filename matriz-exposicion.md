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
    R1 — [Nombre corto]: [0.7, 0.8]
    R2 — [Nombre corto]: [0.5, 0.6]
    R3 — [Nombre corto]: [0.3, 0.7]
    R4 — [Nombre corto]: [0.6, 0.3]
    R5 — [Nombre corto]: [0.2, 0.4]
    R6 — [Nombre corto]: [0.4, 0.2]
```

> **Cómo leer el gráfico:** cada punto representa un riesgo. El eje X es la probabilidad normalizada (valor/10) y el eje Y es el impacto normalizado (valor/10).

## Interpretación

| Cuadrante | Zona | Riesgos | Acción |
|-----------|------|---------|--------|
| Superior derecho | 🔴 Atención Inmediata | R1, R3 | Mitigar o evitar activamente |
| Superior izquierdo | 🟠 Monitorear | R2 | Planificar contingencia |
| Inferior derecho | 🟡 Contingencia | R4 | Transferir o aceptar con plan |
| Inferior izquierdo | 🟢 Aceptar | R5, R6 | Registrar y monitorear |

---

*Cátedra Gestión de Proyectos · FIUNER · 2026*
