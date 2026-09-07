# Plan de Implementación en n8n — Proyecto 01 (ALIF)

## 1. Objetivo del flujo en n8n
Construir un sistema automatizado que clasifique, procese y limpie imágenes usando nodos de automatización y análisis con IA.

---

## 2. Trigger del flujo
**Nodo: Read Binary File / Watch Folder**
- Detecta nuevas imágenes añadidas a una carpeta del sistema.
- Envía la imagen al flujo para su análisis.

---

## 3. Preprocesamiento
**Nodo: Function**
- Normaliza la imagen.
- Extrae metadatos (fecha, tamaño, resolución).
- Genera hash para detección de duplicados.

---

## 4. Análisis con IA
**Nodo: HTTP Request (API de visión)**
El modelo devuelve:
- Si hay rostro.
- Si es captura de pantalla.
- Si está borrosa.
- Si es duplicada.
- Si contiene texto relevante.

---

## 5. Clasificación
**Nodo: Switch**
Clasifica la imagen en:
- Rostro
- Captura de pantalla
- Borrosa
- Duplicada
- Documento
- Irrelevante

---

## 6. Motor de reglas
**Nodo: IF**
Aplica reglas:
- Sin rostro → posible eliminación.
- Captura de pantalla → mover a “Screenshots”.
- Borrosa → eliminar.
- Duplicada → conservar la mejor versión.
- Texto importante → mover a “Documentos”.

---

## 7. Acciones del sistema
**Nodo: Move / Delete / Write Binary File**
- Mover imagen.
- Eliminar imagen.
- Guardar en carpeta específica.

---

## 8. Registro (Log)
**Nodo: Append to File**
Registra:
- Acción realizada.
- Fecha y hora.
- Categoría asignada.

---

## 9. Reporte semanal
**Nodo: Cron → Generate Report**
- Genera informe con estadísticas de limpieza.
- Envía reporte por email o lo guarda en carpeta.

---

## 10. Integraciones futuras
- Panel de control en Streamlit.
- Sincronización con nube.
- Notificaciones automáticas.
