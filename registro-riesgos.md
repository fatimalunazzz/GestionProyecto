# ⚠️ Registro de Riesgos
&gt; **Escala de prioridades:** Exposición ≥ 50 → Alta (🔴) · 25-49 → Media (🟡) · &lt; 25 → Baja (🟢)

## 📐 Criterios de Evaluación y Escalado Porcentual

Para objetivar la estimación de **Probabilidad (P)** e **Impacto (I)**, se establecen las siguientes equivalencias porcentuales:

### 1\. Criterio de Probabilidad de Ocurrencia ($P$)

| Valor (1-10) | Rango Porcentual (%) | Definición Cualitativa                                            |
| ------------ | -------------------- | ----------------------------------------------------------------- |
| **1 - 2**    | 10% – 20%            | **Muy Baja:** Evento atípico o raro.                              |
| **3 - 4**    | 30% – 40%            | **Baja:** Poco probable, pero posible en condiciones específicas. |
| **5 - 6**    | 50% – 60%            | **Moderada:** Ocurrencia probable (50% de probabilidad estimada). |
| **7 - 8**    | 70% – 80%            | **Alta:** Muy probable de ocurrencia durante la ejecución.        |
| **9 - 10**   | 90% – 100%           | **Casi Segura:** Evento inminente si no se aplican controles.     |

### 2\. Criterio de Impacto en el Proyecto ($I$)

| Valor (1-10) | Desviación Porcentual Estimada | Definición de Impacto                                                         |
| ------------ | ------------------------------ | ----------------------------------------------------------------------------- |
| **1 - 2**    | Impacto &lt; 5%                   | **Despreciable:** Demora de un día o menos, absorbible inmediatamente. |
| **3 - 4**    | Impacto 5% – 15%               | **Menor:** Demora de 2 días, o un 15% extra del presupuesto.               |
| **5 - 6**    | Impacto 15% – 25%              | **Moderado:** Consume holguras previstas, dejando sin margen para futuros incidentes sin mover la fecha final. Consume 20% extra del presupuesto  |
| **7 - 8**    | Impacto 25% – 40%              | **Mayor:** Afecta tareas críticas modificando la fecha final a 2 semanas o menos. Incrementos de 50% extra del presupuesto total  |
| **9 - 10**   | Impacto &gt; 40%               | **Crítico / Catastrófico:** Paro total del proyecto o pérdida del prototipo.  |
## Tabla de riesgos

| ID | Sentencia del riesgo | Categoría | Probabilidad (1-10) | Impacto (1-10) | Exposición (P×I) | Prioridad |
|----|---------------------|-----------|:-------------------:|:--------------:|:----------------:|:---------:|
| R1 | **Si** ocurren precipitaciones intensas o tormentas en las reservas de prueba, **entonces** se interrumpirán las mediciones en terreno y se retrasarán las pruebas de autonomía en campo. | Externo | 6 | 6 | 36 | Media |
| R2 | **Si** ocurren fluctuaciones económicas severas o variaciones cambiarias en Argentina, **entonces** aumentará el costo de los insumos electrónicos e importados, desajustando el presupuesto estimado. | Económico/Externo | 8 | 6 | 48 | Media |
| R3 | **Si** el clasificador de IA presenta un alto nivel de falsos positivos por ruidos de fondo (tránsito/viento), **entonces** no se alcanzará la precisión deseada, exigiendo re-entrenar el modelo y ajustar el dataset. | Técnico | 7 | 8 | 56 |  Alta |
| R4 | **Si** la tarjeta SD se corrompe por escrituras continuas de archivos `.wav` o fallas de alimentación, **entonces** se interrumpirá la grabación continua o se generarán datos inauditables. | Técnico | 6 | 9 | 54 |  Alta |
| R5 | **Si** ocurre una descarga electrostática o caída de rayo en la zona de montaje en campo, **entonces** se destruirán los componentes electrónicos (placa/sensores) y se perderá el prototipo físico. | Técnico/Externo | 3 | 8 | 24 | Baja |
| R6 | **Si** existen demoras de importación o falta de stock local de insumos secundarios (gabinete o conectores), **entonces** se deberá adaptar un gabinete alternativo, requiriendo reajustes mecánicos menores. | Organizaional | 5 | 4 | 20 | Baja |
| R7 | **Si** el prototipo es sujeto de robo o vandalismo (gabinete o conectores), **entonces** se deberá rastrear, reacondicionar, suplir o rehacer el prototipo nuevamente | Externo | 5 | 9 | 45 | Media |
| R8 | **Si** un integrante clave del equipo se enferma o sufre indisponibilidad prolongada durante una fase crítica (ej. desarrollo del clasificador de IA o ensamblaje de hardware), **entonces** se generará un cuello de botella en las tareas asignadas a su rol, demorando el avance del camino crítico. | Gestión/Recursos Humanos | 5 | 7 | 35 | Media |

> **Escala de prioridad:** Exposición ≥ 50 → Alta · 25-49 → Media · < 25 → Baja

## Riesgos ordenados por exposición

| Posición | ID | Exposición | Nivel |
|:--------:|----|:----------:|-------|
| 1º | R1 | 56 | 🔴 Alta |
| 2º | R2 | 56 | 🔴 Alta |
| 3º | R3 | 54 | 🔴 Alta |
| 4º | R4 | 48 | 🟡 Media |
| 5º | R7 | 45 | 🟡 Media|
| 6º | R8 | 40 | 🟡 Media |
| 7º | R5 | 36 | 🟡 Media |
| 8º | R6 | 20 | 🟢 Baja |



---

*Cátedra Gestión de Proyectos · FIUNER · 2026*
