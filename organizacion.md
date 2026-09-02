# 🏢 Organización del Proyecto

## Usuarios e interesados (Stakeholders)

| Nombre / Rol | Área | Interés en el proyecto | Influencia |
|--------------|------|------------------------|-----------|
|Organismo Estatal de Conservación | Secretaría de Ambiente de Entre Ríos / Dirección de Áreas Naturales| Disponer de una herramienta autónoma y de bajo costo para justificar la toma de decis[...]
|Municipios de Oro Verde y Paraná |Gestión Ambiental Urbana / Planificación Territorial| Utilizar la información del Índice de Calidad Acústico-Ecológica y los reportes de perturbación acú[...]
| Directiva de la ONG / Parque Natural | Gestión territorial / Conservación | Disponer de una herramienta autónoma y de bajo costo para justificar la toma de decisiones y reportar el estado de c[...]
| Administrador del espacio natural/Guardaparques (usuario final)  | Conservación /Operaciones de campo  | Conocer la actividad de fauna y detectar zonas con intrusiones o perturbaciones sonoras [...]
| Comité Científico / Equipo Biológico | Investigación y Monitoreo Ecológico | Validar la calibración científica de los índices bioacústicos elegidos (NDSI, ACI) sobre el terreno y utiliz[...]
| Comunidad Local y Donantes / Financiadores | Desarrollo Institucional / Difusión | Visualizar los resultados mediante mapas interactivos para verificar el impacto de los proyectos de conservaci[...]
## Áreas involucradas

- Gestión ambiental: define las necesidades de monitoreo, los sitios de interés y el uso de los indicadores generados.
- Bioingeniería / Electrónica: diseña e implementa dispositivos autónomos de bajo costo, resistentes a la intemperie, con autonomía energética suficiente para campañas en zonas alejadas.
- Procesamiento de señales e Inteligencia Artificial: desarrolla los algoritmos para procesar y clasificar los registros acústicos.
- Biodiversidad / Ciencias ambientales: alida la correlación entre las métricas del software y la biodiversidad real, ajustando parámetros según la fauna del lugar.  
## Equipo del proyecto

| Integrante | Rol en el proyecto | Responsabilidad principal |
|------------|--------------------|--------------------------|
| [COMPLETAR] | Director / Líder de Proyecto (PM) | Coordinar el proyecto, gestionar recursos, plazos y entregables y mantener la comunicación con los interesados |
| [COMPLETAR] | Responsable de Hardware e Infraestructura de Campo | Diseñar e implementar el sistema de adquisición de audio, alimentación y almacenamiento |
| [COMPLETAR] | Responsable de Software e IA | Desarrollar el procesamiento de señales, clasificación de eventos acústicos y generación de indicadores |
| [COMPLETAR] | Especialista en Bioacústica y Conservación/Especialista en Biodiversidad / Asesor ambiental | Configurar las métricas de biodiversidad (NDSI, ACI) y validar científicamente las[...]
| [COMPLETAR] | Responsable de Datos y Visualización | Organizar la base de datos, generar indicadores y desarrollar la visualización de los resultados |


## Estructura del equipo

```mermaid
graph TD
    Sponsor["🏛️ Sponsor Estatal / Patrocinador\n(Organismo Estatal de Conservación - Secretaría de Ambiente)"]
    PM["👤 Director de Proyecto (PM)\nCoordinador General"]
    M1["👤 Responsable de Hardware y Campo\nDiseño Físico & Despliegue"]
    M2["👤 Responsable de Software e IA\nClasificación & Algoritmia"]
    M3["👤 Especialista en Bioacústica/Asesor Ambiental\nEstandarización & Calibración Científica"]
    M4["👤 Responsable de Datos y Visualización\nBase de Datos & Plataforma Web"]

    Sponsor --> PM
    PM --> M1
    PM --> M2
    PM --> M3
    PM --> M4
```

---

*Cátedra Gestión de Proyectos · FIUNER · 2026*
