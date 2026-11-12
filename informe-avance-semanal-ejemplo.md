# 📄 Informe de Avance Semanal — Proyecto TRINO

**Nombre del Proyecto:** Trino — Sistema de Monitoreo Acústico Autónomo  
**Período Reportado:** Semana N° 4 (del 22/03/2027 al 26/03/2027)  
**Elaborado por:** Equipo Integrador del Proyecto (Hardware, Software/IA, Datos, Bioacústica y PM)  
**Fecha de Emisión:** 26/03/2027  

---

### 🟢 Estado de Avances Técnicos

#### Tareas Completadas:
* **1.1.1 Estandarización de parámetros de audio** *(Bioacústica — Esp. en Bioacústica)*: Finalizó la especificación técnica de captura acústica: tasa de muestreo fijada en 48 kHz, cuantización de 16 bits PCM en formato monofónico `.wav` no comprimido.
* **1.2.2 Selección e integración de componentes físicos** *(Hardware — Resp. Hardware)*: Concluyó el dimensionamiento y adquisición del micrófono omnidireccional comercial, tarjeta de desarrollo de bajo consumo, módulo MicroSD, gabinete estanqueizado (norma IP65) y herrajes de sujeción para árbol/poste.
* **2.1.1 Diseño de esquema de datos y metadatos** *(Software/Datos — Resp. de Datos)*: Se definió la estructura relacional de la base de datos y la taxonomía de metadatos estandarizada bajo el protocolo Audubon Core para la georreferenciación de puntos de muestreo.

#### Tareas en Desarrollo:
* **1.3.2 Configuración de firmware y almacenamiento SD** *(Hardware — Resp. Hardware)* | **Avance: 65%**  
  Se encuentra en fase de programación la rutina de guardado automático de archivos en bloques independientes de 5 minutos (para prevenir corrupción ante cortes de energía, riesgo R4) y el módulo de gestión de energía con corte seguro por bajo voltaje (*Low Voltage Disconnect*).
* **2.2.1 Algoritmo de cálculo de índices NDSI y ACI** *(Software/IA — Resp. Software e IA)* | **Avance: 80%**  
  Implementación del script en Python para la Transformada Rápida de Fourier (FFT) y separación de bandas de frecuencia: biofonía (2 kHz - 8 kHz) vs. antropofonía (100 Hz - 1.5 kHz).
* **3.1 Estandarización del dataset acústico inicial** *(Bioacústica — Esp. en Bioacústica)* | **Avance: 50%**  
  Curaduría y etiquetado manual de 300 muestras de audio de aves autóctonas del Jardín Botánico de Oro Verde para entrenamiento del clasificador.
* **2.3.1 Mapa interactivo de puntos de muestreo** *(Software/Datos — Resp. de Datos)* | **Avance: 40%**  
  Desarrollo del componente web en Leaflet/OpenStreetMap para renderizar las coordenadas GPS de los nodos de escucha.
* **4.2 Seguimiento y Control** *(Gestión de Proyecto — PM)* | **Avance: Continuo (Semana 4 de 9)**  
  Control periódico del camino crítico y monitoreo de la curva de avance acumulado.

---

### ⚠️ Registro de Incidentes y Bloqueos

#### Incidentes Resueltos:
* **INC-01 (Falla de I/O en tarjeta SD):** Durante las pruebas de firmware se detectó corrupción de archivos `.wav` por escrituras continuas en tarjetas SD convencionales. **Solución:** Se sustituyó la unidad por una tarjeta MicroSD de grado industrial *High Endurance (SLC)* y se ajustó el buffer de escritura en memoria RAM antes del *flush* a disco.

#### Incidentes Abiertos / No Resueltos:
* **INC-02 (Variación de costos en insumos de montaje - Riesgo R2):** Incremento del 12% en el costo del gabinete estanqueizado debido a fluctuaciones cambiarias. **Impacto:** Ninguno sobre el cronograma. **Acción:** Absorción mediante el Fondo de Reserva de Contingencia Financiera (PM).

---

### 🎯 Decisiones Requeridas y Próximos Pasos

#### Decisiones Pendientes:
1. **Definición de umbral NDSI (Para Gestión de Calidad / Sponsor):** Confirmar si el corte de frecuencia antropogénica para la zona periurbana de Paraná se fija en 1.5 kHz o 2.0 kHz para compensar el ruido de tránsito pesado de la Ruta 11.
2. **Validación de permisos de montaje:** Confirmar con el Administrador del Jardín Botánico de Oro Verde la fecha exacta de instalación en altura para las pruebas de campo.

#### Planificación Próxima Semana (Semana N° 5):
* Iniciar la **Tarea 1.3.3**: Montaje físico y comprobación de funcionamiento integrado de prototipo.
* Finalizar el **Algoritmo NDSI/ACI (Tarea 2.2.1)** y dar inicio al entrenamiento del **Clasificador Binario Aves vs. Perturbación (Tarea 2.2.2)**.
* Completar el etiquetado del **Dataset Acústico (Tarea 3.1)**.

#### Comentarios / Observaciones:
El proyecto se ejecuta en total conformidad con la línea base planificada. La ventana temporal operativa se mantiene en los **41 días hábiles de trabajo neto (62 días calendario continuos)**, conservando sin uso el margen de **4.7 días hábiles de la Reserva por Incertidumbre PERT (95% de confianza)**.
