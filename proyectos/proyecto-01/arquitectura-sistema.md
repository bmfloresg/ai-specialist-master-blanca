# Arquitectura del Sistema — Proyecto 01 (ALIF)

## 1. Visión general
El sistema ALIF está compuesto por módulos independientes que trabajan juntos para clasificar, procesar y limpiar imágenes de forma automática.

## 2. Módulos principales

### Módulo A — Ingesta de imágenes
- Detecta nuevas imágenes en el dispositivo.
- Extrae metadatos (fecha, tamaño, resolución).
- Envía la imagen al módulo de análisis.

### Módulo B — Análisis con IA
- Detecta rostros.
- Identifica capturas de pantalla.
- Evalúa nitidez (borrosas).
- Detecta duplicados mediante hashing.
- Clasifica la imagen en una categoría.

### Módulo C — Motor de reglas
Aplica las reglas definidas:
- Sin rostro → posible eliminación.
- Captura de pantalla → mover a “Screenshots”.
- Borrosa → eliminar.
- Duplicada → conservar la mejor.
- Texto importante → mover a “Documentos”.

### Módulo D — Acciones del sistema
- Mover imagen.
- Eliminar imagen.
- Guardar en carpeta específica.
- Registrar acción en log.

### Módulo E — Registro y reportes
- Guarda cada acción en un archivo de log.
- Genera un reporte semanal con:
  - Imágenes eliminadas.
  - Imágenes movidas.
  - Imágenes conservadas.
  - Duplicados detectados.

## 3. Flujo de datos
Ingesta → Análisis IA → Motor de reglas → Acción → Log → Reporte

## 4. Integraciones futuras
- Conexión con n8n o Make.
- Integración con almacenamiento en la nube.
- Panel de control en Streamlit.
- Notificaciones automáticas.
