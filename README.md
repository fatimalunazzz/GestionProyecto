# 📋 Template — Plan de Proyecto Integrador

> **Gestión de Proyectos · FIUNER · 2026**
> Basado en las buenas prácticas del **PMBOK v7**

---

## ¿Qué es este repositorio?

Este repositorio es una **plantilla de trabajo** para desarrollar el Plan de Proyecto Integrador de la materia Gestión de Proyectos. Cada grupo debe clonarlo, instanciarlo con su caso de estudio y completar los artefactos de forma incremental a lo largo del cuatrimestre.

La documentación está organizada en carpetas que se corresponden con las **5 entregas** del TP más la **Exposición Final (PechaKucha)**. Cada archivo incluye instrucciones, tablas y diagramas en formato [Mermaid](https://mermaid.js.org/) listos para completar.

---

## 🚀 ¿Cómo usar este template?

1. Crear un repositorio propio a partir de este template (botón **Use this template** en GitHub).
2. Habilitar la **Wiki** del repositorio (Settings → Features → Wiki).
3. Agregar el secret `WIKI_TOKEN` con un Personal Access Token (PAT) con permisos `repo` y `wiki` (Settings → Secrets → Actions).
4. Completar los datos del grupo en [`docs/00-caso-y-equipo/equipo.md`](docs/00-caso-y-equipo/equipo.md).
5. Trabajar sobre cada carpeta según el cronograma del TP.
6. Al hacer `push` a `main`, la wiki se actualiza automáticamente.

---

## 📂 Estructura del repositorio

```
plan-proyecto-template/
├── README.md                          ← Este archivo
├── plan-proyecto.md                   ← Plan maestro consolidado
│
├── docs/
│   ├── 00-caso-y-equipo/              ← Contexto y datos del grupo
│   ├── 01-plan-inicial/               ← Entrega 1
│   ├── 02-wbs-estimaciones/           ← Entrega 2
│   ├── 03-recursos-raci/              ← Entrega 3
│   ├── 04-riesgos/                    ← Entrega 4
│   ├── 05-comunicaciones-cambios/     ← Entrega 5
│   └── 06-pechakucha/                 ← Exposición Final
│
├── plantillas/
│   ├── formulario-cambio.md           ← Formulario de solicitud de cambio
│   └── acta-reunion.md                ← Acta de reunión
│
└── .github/
    └── workflows/
        └── sync-wiki.yml              ← Sincronización automática con la Wiki
```

---

## 📅 Cronograma de entregas

| # | Entrega | Carpeta | 1er Cuatrimestre | 2do Cuatrimestre |
|---|---------|---------|-------------------|-------------------|
| 1 | Plan de Proyecto Inicial | `01-plan-inicial/` | 10 de abril | 4 de septiembre |
| 2 | WBS y Estimaciones | `02-wbs-estimaciones/` | 24 de abril | 25 de septiembre |
| 3 | Asignación de Recursos y RACI | `03-recursos-raci/` | 15 de mayo | 9 de octubre |
| 4 | Administración de Riesgos | `04-riesgos/` | 29 de mayo | 23 de octubre |
| 5 | Comunicaciones y Cambios | `05-comunicaciones-cambios/` | 12 de junio | 6 de noviembre |
| F | Exposición Final — PechaKucha | `06-pechakucha/` | 26 de junio | 17 de noviembre |

---

## 🧭 Convenciones del template

- Los bloques `[COMPLETAR: ...]` indican dónde el grupo debe ingresar información.
- Los diagramas Mermaid están pre-armados con la **estructura** correcta; solo hace falta reemplazar los datos de ejemplo.
- Los archivos `README.md` dentro de cada carpeta explican el objetivo de la entrega.

---

*Cátedra Gestión de Proyectos · FIUNER · 2026*
