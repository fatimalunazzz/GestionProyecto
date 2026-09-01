# 🔄 Ciclo de Vida del Proyecto

## Enfoque seleccionado

> **Híbrido**

## Justificación de la elección

> [COMPLETAR: explicar por qué este enfoque es el más adecuado para el proyecto, considerando características como: complejidad, claridad de requisitos, tamaño del equipo, tolerancia al cambio, experiencia del equipo, etc.]
> Si bien conocemos, a priori, los distintos pasos para llevar a cabo el proyecto, también tenemos en cuenta limitaciones tecnológicas y burocraticas, por esto consideramos un enfoque hibrido.
> La complejidad del proyecto es moderada en cuanto a su implementación, el equipo tiene experiencia relativa en cuanto al procesamiento digital de señales e implementación de hardware para adquisición de señales. Al analizar el proyecto en fases, la relacionada a la construcción del clasificador de las señales de audio, el equipo no posee experiencia en generar en algoritmos de clasificación y/o clasificadores en general.
> El equipo es flexible en la adaptación al cambio, por lo que un enfoque que se aproxime a ágil no es algo desconocido para el desarrollo de un proyecto. 

## Árbol de decisión

```mermaid
flowchart TD
    A{{"¿Los requisitos\nson estables?"}}
    B{{"¿El equipo tiene\nexperiencia en ágil?"}}
    C{{"¿El entorno admite\nentregas incrementales?"}}

    A -- Sí --> P["✅ Predictivo\n(Cascada)"]
    A -- No --> B
    B -- Sí --> D["✅ Adaptativo\n(Scrum / Kanban)"]
    B -- No --> C
    C -- Sí --> H["✅ Híbrido"]
    C -- No --> P

    style P fill:#BDD7EE,stroke:#2E75B6
    style D fill:#C8E6C9,stroke:#2E7D32
    style H fill:#FFF9C4,stroke:#F9A825
```

> **Decisión del grupo:** [COMPLETAR: indicar cuál rama del árbol aplica a su caso y por qué]

## Fases del proyecto

```mermaid
flowchart LR
    F1["📌 Fase 1\n[COMPLETAR]"]
    F2["📌 Fase 2\n[COMPLETAR]"]
    F3["📌 Fase 3\n[COMPLETAR]"]
    F4["📌 Fase 4\n[COMPLETAR]"]

    F1 --> F2 --> F3 --> F4
```

| Fase | Nombre | Objetivo | Criterio de salida |
|------|--------|----------|-------------------|
| 1 | [Inicio] | [COMPLETAR] | [COMPLETAR] |
| 2 | [Planificación] | [COMPLETAR] | [COMPLETAR] |
| 3 | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] |
| 4 | [COMPLETAR] | [COMPLETAR] | [COMPLETAR] |

---

*Cátedra Gestión de Proyectos · FIUNER · 2026*
