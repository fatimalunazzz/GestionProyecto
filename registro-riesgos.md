# ⚠️ Registro de Riesgos

## Tabla de riesgos

| ID | Sentencia del riesgo | Categoría | Probabilidad (1-10) | Impacto (1-10) | Exposición (P×I) | Prioridad |
|----|---------------------|-----------|:-------------------:|:--------------:|:----------------:|:---------:|
| R1 | **Si** ocurren precipitaciones intensas o tormentas en las reservas de prueba, **entonces** se interrumpirán las mediciones en terreno y se retrasarán las pruebas de autonomía en campo. | Externo | 6 | 8 | 48 | Media |
| R2 | **Si** ocurren fluctuaciones económicas severas o variaciones cambiarias en Argentina, **entonces** aumentará el costo de los insumos electrónicos e importados, desajustando el presupuesto estimado. | Económico/Externo | 8 | 7 | 56 | Alta |
| R3 | **Si** el clasificador de IA presenta un alto nivel de falsos positivos por ruidos de fondo (tránsito/viento), **entonces** no se alcanzará la precisión deseada, exigiendo re-entrenar el modelo y ajustar el dataset. | Técnico | 7 | 8 | 56 |  Alta |
| R4 | **Si** la tarjeta SD se corrompe por escrituras continuas de archivos `.wav` o fallas de alimentación, **entonces** se interrumpirá la grabación continua o se generarán datos inauditables. | Técnico | 6 | 9 | 54 |  Alta |
| R5 | **Si** ocurre una descarga electrostática o caída de rayo en la zona de montaje en campo, **entonces** se destruirán los componentes electrónicos (placa/sensores) y se perderá el prototipo físico. | Técnico/Externo | 3 | 9 | 27 | Media |
| R6 | **Si** existen demoras de importación o falta de stock local de insumos secundarios (gabinete o conectores), **entonces** se deberá adaptar un gabinete alternativo, requiriendo reajustes mecánicos menores. | Organizaional | 5 | 4 | 20 | Baja |
| R7 | **Si** el prototipo es sujeto de robo o vandalismo (gabinete o conectores), **entonces** se deberá rastrear, reacondicionar, suplir o rehacer el prototipo nuevamente | Externo | 5 | 9 | 45 | Media |

> **Escala de prioridad:** Exposición ≥ 50 → Alta · 25-49 → Media · < 25 → Baja

## Riesgos ordenados por exposición

| Posición | ID | Exposición | Nivel |
|:--------:|----|:----------:|-------|
| 1º | R1 | 56 | 🔴 Alta |
| 2º | R2 | 56 | 🔴 Alta |
| 3º | R3 | 54 | 🔴 Alta |
| 4º | R4 | 48 | 🟡 Media |
| 5º | R7 | 45 | 🟡 Media|
| 6º | R5 | 36 | 🟡 Media |
| 7º | R6 | 20 | 🟢 Baja |


---

*Cátedra Gestión de Proyectos · FIUNER · 2026*
