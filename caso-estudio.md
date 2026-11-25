# 📖 Caso de Estudio

## Nombre del proyecto

>  Proyecto TRINO: Monitoreo Bioacústico Autónomo para la Evaluación de la Biodiversidad y la Perturbación Antropogénica en el Corredor Periurbano Paraná - Oro Verde 

## Origen del caso

- [ ] Caso provisto por la cátedra
- [x] Caso propio basado en experiencia laboral/profesional
- [ ] Proyecto ya realizado, utilizado como contexto

## Descripción general

> [El **Proyecto TRINO** consiste en el diseño, desarrollo e implementación de un **Sistema de Monitoreo Bioacústico Autónomo** orientado al diagnóstico de biodiversidad y calidad acústico-ecológica en áreas naturales y periurbanas]

## Organización involucrada

| Campo | Detalle |
|-------|---------|
| Nombre de la organización | **Fundación CAUCE** (*Cultura Ambiental Causa Ecologista*) |
| Sector / Industria | Organización No Gubernamental (ONG) / Tercer Sector (Conservación Ambiental, Ecología y Protección de Ecosistemas) |
| Tamaño aproximado | Organización de la Sociedad Civil (OSC) pequeña / mediana (aprox. **10 a 25 colaboradores**, entre equipo técnico, consultores ambientales y voluntarios) |
| Área solicitante | Área de Conservación Ambiental, Monitoreo de Biodiversidad e Investigación Ecológica |

## Problema u oportunidad

> * **Problema:** Los monitoreos tradicionales de biodiversidad dependen de campañas de campo presenciales realizadas por especialistas biólogos. Estas metodologías son discontinuas en el tiempo, presentan altos costos logísticos y tienen una cobertura geográfica acotada, lo que dificulta detectar oportunamente el impacto del crecimiento urbano sobre la fauna autóctona.
* **Oportunidad:** Desarrollar una solución tecnológica autónoma de bajo costo basada en bioacústica que registre datos sonoros en forma continua las 24 horas del día. Esto permite automatizar la generación de indicadores ambientales (NDSI/ACI) e informar la toma de decisiones ecológicas con datos cuantitativos en tiempo casi real.

## Objetivo del proyecto

> * **Objetivo General:** Diseñar, construir y validar un sistema de monitoreo bioacústico autónomo desplegado durante 9 semanas de trabajo (41 días hábiles netos / 62 días calendario), entregando a la Fundación CAUCE una plataforma web interactiva y el Informe Diagnóstico Ambiental.
* **Objetivos Específicos:**
1. Integrar e instalar los nodo físico de captura con protección estanca IP65 y autonomía fotovoltaica continua.
2. Implementar los algoritmos de cálculo espectral (NDSI/ACI) y entrenar el clasificador de IA con una precisión mínima (*F1-score*) del 80%.
3. Desplegar el mapa interactivo web para la visualización georreferenciada de la calidad acústica.
4. Elaborar el informe ambiental comparativo entre la zona conservada (Jardín Botánico) y la zona intervenida (Ruta 11 / Paraná)

## Restricciones conocidas

| Tipo | Descripción |
|------|-------------|
| Tiempo | Período de ejecución estricto de **9 semanas** (41 días hábiles de trabajo neto y 4,7 días de Reserva por Incertidumbre PERT 95%), acotado al calendario de la cátedra de Gestión de Proyectos. |
| Presupuesto | Límite financiero máximo de **$14.370.00 ARS** (\~USD 9.125), que consolida insumos de hardware, servicios cloud (3 meses), 370 horas de honorarios profesionales y los fondos de contingencia (15% en HW por riesgo cambiario R2 y 10% de reserva general).|
| Tecnológica / Hardware | Obligación de utilizar componentes comerciales en stock nacional (*Off-The-Shelf* / COTS) para asegurar disponibilidad inmediata en 24–72 horas sin arriesgar el camino crítico por tiempos de importación aduanera. |
| Legal y Permisos | El despliegue del dispositivo de escucha en terreno está supeditado a la aprobación formal de los permisos de acceso e instalación por parte de los Municipios de Oro Verde (Jardín Botánico) y Paraná. |
| Alcance | El despliegue de los nodos de escucha en terreno está supeditado a la aprobación formal de los permisos de acceso e instalación por parte de los Municipios de Oro Verde (Jardín Botánico) y Paraná. |
| Ambiental / Operativa | Operación continua a la intemperie sujeta a variaciones climáticas (humedad, lluvia, dosel vegetal denso), lo que exige protección estanca IP65 y recarga solar mínima para garantizar 72 horas de autonomía continua. |
| Recursos | Disponibilidad horaria limitada a **370 horas hombre totales** repartidas entre los 6 roles RACI, con un tope de dedicación de 25 hs/semana por integrante para evitar sobreasignaciones. |

## Supuestos 
* **Disponibilidad del equipo técnico:** Se asume la disponibilidad efectiva y continua de las **370 horas hombre** acordadas para los 6 roles RACI, manteniendo un tope máximo de dedicación de 25 hs/semana por integrante para evitar sobreasignaciones.
* **Integridad del almacenamiento en campo:** Se presupone que el uso de tarjetas MicroSD de grado industrial (*High Endurance*) y la rutina de grabado en bloques independientes de 5 minutos evitan la corrupción de encabezados `.wav` ante imprevistos de energía (Mitigación del Riesgo R4).
* **Autonomía fotovoltaica:** Se asume un nivel promedio de radiación solar suficiente en la región para recargar las baterías LiFePO4 mediante el panel solar de 5W, garantizando **72 horas de operación continua** en campo bajo dosel vegetal.
* **Permisos institucionales y de acceso:** Se presupone el otorgamiento oportuno de las autorizaciones de instalación física y acceso en el Jardín Botánico de Oro Verde y el corredor periurbano por parte de las autoridades municipales durante las Semanas 4-5\.
* **Estabilidad económica de insumos:** Se asume que las variaciones de precios o fluctuaciones cambiarias en componentes de hardware se mantendrán dentro del margen cubierto por la **Reserva de Contingencia Financiera ($65.745 ARS / 15% del HW)** (Mitigación del Riesgo R2).
* **Desempeño del clasificador de IA:** Se presupone que la curaduría e identificación de 300 muestras sonoras locales en el Jardín Botánico proporcionará un dataset suficiente para alcanzar una precisión ($F1\text{-score} \ge 80\%$) al discriminar cantos de aves de ruidos de tránsito (Mitigación del Riesgo R3).

---

*Cátedra Gestión de Proyectos · FIUNER · 2026*
