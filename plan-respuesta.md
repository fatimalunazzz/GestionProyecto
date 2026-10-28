# 🛡️ Plan de Respuesta a Riesgos

> Se documenta el plan para los **3 riesgos de mayor exposición**.

## R1 — [Nombre del riesgo]

| Campo | Detalle |
|-------|---------|
| **Sentencia** | Si ocurren fluctuaciones económicas severas o variaciones cambiarias en Argentina, entonces aumentará el costo de los insumos electrónicos e importados, desajustando el presupuesto estimado. |
| **Exposición** | 8 × 7 = 56 |
| **Estrategia** | ☑ Mitigar · ☐ Evitar · ☐ Transferir · |
| **Acciones** | 1\. Realizar la compra anticipada de componentes electrónicos e insumos importados durante la fase inicial de gobernanza. · 2\. Constituir un fondo de reserva de contingencia presupuestaria en moneda dura o cobertura. · 3\. Acordar precios y cotizaciones garantizadas con proveedores locales de hardware. |
| **Responsable** | Director / Líder de Proyecto (PM) |
| **Indicador de monitoreo** | Variación semanal del tipo de cambio oficial/financiero superior al 5% o alertas inflacionarias en el sector de componentes electrónicos. |
| **Plan de contingencia** | Reasignar fondos de la reserva de contingencia del proyecto y renegociar especificaciones secundarias de componentes no críticos (ej. gabinete) sin afectar las funcionalidades del prototipo. |

## R2 — Falsos positivos y baja precisión en el clasificador de IA

| Campo | Detalle |
|-------|---------|
| **Sentencia** | Si el clasificador de IA presenta un alto nivel de falsos positivos por ruidos de fondo, entonces no se alcanzará la precisión deseada, exigiendo re-entrenar el modelo y ajustar el dataset. |
| **Exposición** | 7 × 8 = 56|
| **Estrategia** | ☑ Mitigar · ☐ Evitar · ☐ Transferir  |
| **Acciones** | 1\. Aplicar técnicas de *Data Augmentation* agregando capas de ruido ambiental real (tránsito, lluvia, viento) al dataset de entrenamiento. · 2\. Implementar un pre-filtrado espectral basado en índices bioacústicos (NDSI y ACI) previo a la clasificación binaria. · 3\. Ejecutar pruebas de validación cruzada temprana con grabaciones de prueba.|
| **Responsable** | Responsable de Software e IA |
| **Indicador de monitoreo** | Métrica de precisión (*F1-Score*) inferior al 80% en las pruebas de validación preliminares del modelo de IA. |
| **Plan de contingencia** | Absorber el tiempo de re-entrenamiento en la Reserva por Incertidumbre PERT (hasta 45 días hábiles totales) y re-calibrar los umbrales de sensibilidad del clasificador binario. |

## R3 — Corrupción de tarjeta SD o falla en almacenamiento de audio

| Campo | Detalle |
|-------|---------|
| **Sentencia** | Si la tarjeta SD se corrompe por escrituras continuas de archivos `.wav` o fallas de alimentación, entonces se interrumpirá la grabación continua o se generarán datos inauditables. |
| **Exposición** | 6 × 9 = 54 |
| **Estrategia** | ☑ Mitigar · ☐ Evitar · ☐ Transferir |
| **Acciones** | 1\. Adquirir e instalar tarjetas MicroSD de grado industrial (*High Endurance / SLC*) diseñadas para escritura continua. · 2\. Programar una rutina en el firmware para cerrar y guardar archivos de audio en bloques independientes de 5 minutos, previniendo la pérdida de datos ante cortes de energía. · 3\. Incorporar un módulo de protección de voltaje con corte seguro (*Low Voltage Disconnect*). |
| **Responsable** | Responsable de Hardware e Infraestructura de Campo |
| **Indicador de monitoreo** | Errores de lectura/escritura (I/O) en los logs de prueba de firmware o caídas de tensión de la batería por debajo del umbral de seguridad. |
| **Plan de contingencia** | | Reemplazar la tarjeta SD afectada por la unidad de repuesto del kit de campo y realizar el formateo de bajo nivel para recuperación del almacenamiento. |
| ------------------------------------------------------------------------------------------------------------------------------------------------------- | |

---

*Cátedra Gestión de Proyectos · FIUNER · 2026*
