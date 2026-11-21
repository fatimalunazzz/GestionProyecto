#  Plantilla de Informe Mensual Ejecutivo — Proyecto TRINO

###  Informes para el Sponsor (Fundación CAUCE)

a comunicación ejecutiva con la ONG se concentra en **2 Informes Hito Estratégicos**:

1.  **Informe Hito 1: A Mitad de Proyecto (Semana 4-5 / Fin de Fase 2):**
  * **Enfoque:** Demostración del prototipo físico operativo (gabinete IP65, autonomía y grabado SD), estado de integración del mapa web interactivo preliminar y balance de salud global/presupuesto.
2.  **Informe Hito 2: Previo al Cierre Final (Semana 8-9 / Fin de Fase 3):**
  * **Enfoque:** Entrega del **Informe Ambiental Integrador (Entregable 3.3.1)** con el análisis de los índices bioacústicos (**NDSI** y **ACI**), validación del modelo de IA ante ruidos y transferencia tecnológica a la ONG.

---

## 1. Identificación del Período y Estado General del Proyecto

* **Nombre del Proyecto:** TRINO — Sistema de Monitoreo Bioacústico Autónomo
* **Período Reportado:** `[ Indicar Mes / Año: Ej. Mes 01 — Marzo 2027 / Informe Hito 1 ]`
* **Director de Proyecto (PM):** `[ Nombre y Apellido ]`
* **Sponsor Institucional:** Fundación CAUCE (Cultura Ambiental Causa Ecologista)
* **Fecha de Emisión:** `[ DD/MM/AAAA ]`

### 🚦 Semáforo de Salud del Proyecto
Marcar con una `X` el estado de salud global correspondiente al período reportado, fundamentado en los criterios cuantitativos de la matriz de desvío:

| Estado | Selección | Criterio de Tiempo (Cronograma / SPI) | Criterio de Costo (Presupuesto / CPI) | Condición de Riesgos Críticos |
|:---:|:---:|:---|:---|:---|
| 🟢 **VERDE** <br>*(En Regla)* | `[   ]` | Atraso $\le 2$ días hábiles ($\le 5\%$ del camino crítico). <br>$\text{SPI} \ge 0,95$. | Desvío de costo $\le 5\%$. <br>$\text{CPI} \ge 0,95$. | Riesgos bajo control; sin amenazas críticas materializadas. | 
| 🟡 **AMARILLO** <br>*(Alerta)* | `[   ]` | Atraso de **3 a 5 días hábiles** ($5\% - 12\%$ de desvío). <br>$0,88 \le \text{SPI} < 0,95$. | Sobrecosto de **$5\%$ a $15\%$**. <br>$0,88 \le \text{CPI} < 0,95$. | Riesgo medio/alto activado; uso parcial de holguras. | 
| 🔴 **ROJO** <br>*(Crítico)* | `[   ]` | Atraso **$> 5$ días hábiles** ($> 12\%$ de desvío). <br>$\text{SPI} < 0,88$. | Sobrecosto **$> 15\%$**. <br>$\text{CPI} < 0,88$. | Riesgo alto ($R2, R3, R4$) agota reserva PERT o afecta entrega. | Notificación formal al Sponsor/Comité para redefinir línea base. |

---

## 2. Métricas y KPIs de Gestión del Proyecto

Resumen cuantitativo del progreso físico y cumplimiento de la planificación temporal:

* **Avance Físico Acumulado Real:** `[ % ]` vs. **Planificado:** `[ % ]`
* **Índice de Desempeño del Cronograma (SPI):** `[ Valor: Ej. 1.02 ]` $\left(\text{SPI} = \frac{\text{Avance Real}}{\text{Avance Planificado}}\right)$
* **Índice de Desempeño del Costo (CPI):** `[ Valor: Ej. 0.98 ]` $\left(\text{CPI} = \frac{\text{Valor Ganado}}{\text{Costo Real}}\right)$

### Cumplimiento de Hitos de la Estructura de Desglose del Trabajo (WBS)

| Código WBS | Hito / Entregable Clave | Fecha Planificada | Fecha Real / Estimada | Estado (`Cumplido` / `En Proceso` / `Demorado`) | Observaciones del Hito |
|:---:|:---|:---:|:---:|:---:|:---|
| `[ WBS X.X ]` | `[ Nombre del Hito 1 ]` | `[ DD/MM/AAAA ]` | `[ DD/MM/AAAA ]` | `[ Cumplido ]` | `[ Acta de aprobación / Documento entregado ]` |
| `[ WBS X.X ]` | `[ Nombre del Hito 2 ]` | `[ DD/MM/AAAA ]` | `[ DD/MM/AAAA ]` | `[ En Proceso ]` | `[ Porcentaje de avance y estado ]` |
| `[ WBS X.X ]` | `[ Nombre del Hito 3 ]` | `[ DD/MM/AAAA ]` | `[ DD/MM/AAAA ]` | `[ En Proceso ]` | `[ Porcentaje de avance y estado ]` |

---

## 3. Desempeño Presupuestario 

Balance del uso de fondos asignados y consumo de contingencias:

* **Presupuesto Total Asignado:** `[ $ Monto Total ]`
* **Gasto Acumulado Ejecutado:** `[ $ Monto Ejecutado ]` `[ % del Total ]`
* **Variación Presupuestaria:** `[ $ Sobrecosto o Ahorro ]`

---

## 4. Gestión de Riesgos Críticos y Desvíos

Monitoreo de los principales factores de riesgo del proyecto ($R1$ a $R8$) con mayor nivel de exposición ($P \times I$):

| ID | Factor de Riesgo | Exposición ($P \times I$) | Prioridad | Estado del Riesgo | Medida de Mitigación / Contingencia Aplicada |
|:---:|:---|:---:|:---:|:---:|:---|
| **R2** | Fluctuaciones económicas / cambiarias | **56** | 🔴 **Alta** | `[ Inactivo / Activo ]` | `[ Compra anticipada / Reserva cambiaria ]` |
| **R3** | Falsos positivos / Precisión IA | **56** | 🔴 **Alta** | `[ Inactivo / Activo ]` | `[ Curaduría de dataset / Filtrado espectral ]` |
| **R4** | Corrupción SD / Falla de energía | **54** | 🔴 **Alta** | `[ Inactivo / Activo ]` | `[ MicroSD industrial / Guardado seguro firmware ]` |
| **R1** | Precipitaciones / Clima adverso | **48** | 🟡 **Media** | `[ Inactivo / Activo ]` | `[ Gabinete IP65 / Reprogramación de ventana ]` |
| **R5** | Indisponibilidad de integrante | **40** | 🟡 **Media** | `[ Inactivo / Activo ]` | `[ Reasignación de tareas según Matriz RACI ]` |

---

## 5. Avance Técnico y Entregables para el Sponsor

Resumen del progreso en los cuatro ejes de desarrollo del sistema TRINO:

1. **Hardware y Autonomía (Fase 1):** `[ Estado de ensamblado del nodo, estanqueidad IP65, panel solar y pruebas en terreno ]`
2. **Software, IA e Indicadores Bioacústicos (Fase 2):** `[ Estado de algoritmo NDSI/ACI, clasificación binaria de aves y dashboard web ]`
3. **Datos y Diagnóstico Ambiental (Fase 3):** `[ Avance en la elaboración del Informe Ambiental Integrador 3.3.1 para la ONG ]`
4. **Gobernanza y Calidad (Fase 4):** `[ Estado de auditorías internas de calidad y actualización de documentación ]`

---

## 6. Solicitudes de Decisión y Aprobación al Sponsor (Fundación CAUCE)

Espacio reservado para las solicitudes formales que requieren validación por parte del Sponsor:

1. **Validación de Sitios de Muestreo:** `[ Solicitud de confirmación de puntos de escucha en áreas protegidas ]`
2. **Revisión de Entregables Hito:** `[ Solicitud de conformidad para el hito presentado ]`
3. **Cambios de Alcance o Solicitudes Especiales:** `[ Descripción de cualquier propuesta de ajuste formal ]`

---

## 7. Validaciones y Gobernanza

* **Elaborado por (Director de Proyecto / PM):** `[ Firma / Nombre ]` — Fecha: `[ DD/MM/AAAA ]`
* **Auditado por (Gestión de Calidad):** `[ Firma / Nombre ]` — Fecha: `[ DD/MM/AAAA ]`
* **Conformidad del Sponsor (Fundación CAUCE):** `[ Firma / Nombre ]` — Fecha: `[ DD/MM/AAAA ]`
