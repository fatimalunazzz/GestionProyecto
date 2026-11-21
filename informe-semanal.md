# 📋 Ficha de Avance Semanal — Proyecto TRINO

**Período Reportado:** Semana N° 4 (19 a 23 de Abril de 2027)  
**Semáforo de Estado:** 🟡 **AMARILLO** (Atraso de +3 días hábiles en camino crítico — Absorbible por Reserva PERT)  
**Responsable de Emisión:** Director de Proyecto (PM) / Equipo Técnico Integrado  

---

## 1. Estado del Camino Crítico
* **Desvío Acumulado:** +3 días hábiles de demora acumulada en la Tarea `1.3` (Integración de Hardware y Firmware).
* **Impacto en Hito Final:** La fecha final del proyecto se mantiene dentro de la línea base extendida gracias al margen de la Reserva por Incertidumbre PERT (hasta 45 días hábiles totales).

---

## 2. Checklist de Trabajo en Campo y WBS

| Código WBS | Tarea / Entregable | Responsable (RACI) | % Avance Real | Estado |
|:---:|:---|:---:|:---:|:---:|
| **1.2.1** | Diseño e integración del módulo de alimentación autónoma (Batería + Solar) | Resp. Hardware | 100% | ✅ Finalizado |
| **1.3.1** | Ensamble del prototipo en gabinete estanco IP65 | Resp. Hardware | 100% | ✅ Finalizado |
| **1.3.2** | Programación de firmware para ciclos de grabado y guardado seguro en MicroSD | Resp. Hardware | 70% | 🟡 En Desarrollo |
| **2.1.1** | Estructuración del esquema de datos y metadatos de audio `.wav` | Resp. Datos | 100% | ✅ Finalizado |
| **3.1.2** | Pre-filtrado espectral de ruidos de fondo (viento y tránsito) | Resp. Software e IA | 60% | 🟡 En Desarrollo |

---

## 3. Cuellos de Botella y Bloqueos Activos (Máx. 3)

1. **Falla de escritura aleatoria en Tarjeta SD (Tarea 1.3.2):**
   * *Problema:* Corrupción esporádica de encabezados `.wav` por caídas de tensión al escribir bloques de audio en tarjetas MicroSD estándar.
   * *Acción Inmediata:* Reemplazo por unidades de grado industrial (*High Endurance*) y programación de cierre de archivo cada 5 minutos en el firmware (Mitigación Riesgo R4).

2. **Ruido ambiental elevado en dataset de validación de IA (Tarea 3.1.2):**
   * *Problema:* Falsos positivos por ruidos de viento en pruebas de laboratorio.
   * *Acción Inmediata:* Aplicación de filtros de banda pasante basados en índices NDSI/ACI antes de la clasificación binaria (Mitigación Riesgo R3).

---

## 4. Prioridades del Camino Crítico a 7 Días

1. **Finalizar Tarea 1.3.2:** Concluir las pruebas de escritura continua en MicroSD y cerrar la versión v1.0 del firmware.
2. **Iniciar Tarea 1.4:** Desplegar el banco de pruebas de autonomía en terreno durante 72 horas continuas.
3. **Ajustar Tarea 3.1.2:** Alcanzar el 80% de precisión (*F1-Score*) en el algoritmo de clasificación acústica.
