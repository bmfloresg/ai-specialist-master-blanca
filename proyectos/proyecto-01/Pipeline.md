# Pipeline Completo — Proyecto 01 (ALIF)

## 1. Entrada del sistema
- Imagen nueva añadida al dispositivo.
- Carpeta de fotos existente para análisis periódico.
- Metadatos de la imagen (fecha, tamaño, resolución).

## 2. Preprocesamiento
- Normalización de la imagen.
- Extracción de metadatos.
- Generación de hash para detección de duplicados.

## 3. Análisis con IA
El sistema evalúa:
- Presencia de rostros.
- Detección de capturas de pantalla.
- Nivel de nitidez (borrosa o clara).
- Similitud con otras imágenes (duplicados).
- Presencia de texto relevante.

## 4. Clasificación
La imagen se clasifica en una de estas categorías:
- Rostro
- Captura de pantalla
- Borrosa
- Duplicada
- Documento
- Irrelevante

## 5. Motor de reglas
El motor aplica las reglas definidas:
- Sin rostro → posible eliminación.
- Captura de pantalla → mover a “Screenshots”.
- Borrosa → eliminar.
- Duplicada → conservar la mejor versión.
- Texto importante → mover a “Documentos”.

## 6. Acción final
- Eliminar imagen.
- Mover imagen a carpeta específica.
- Conservar imagen.
- Registrar acción en log.

## 7. Registro (Log)
Cada acción queda registrada con:
- Nombre de archivo.
- Acción realizada.
- Fecha y hora.
- Categoría asignada.

## 8. Reporte semanal
El sistema genera un informe con:
- Imágenes eliminadas.
- Imágenes movidas.
- Imágenes conservadas.
- Duplicados detectados.
- Estadísticas de limpieza.

## 9. Integraciones futuras
- Automatización en n8n o Make.
- Panel de control en Streamlit.
- Sincronización con nube.
- Notificaciones automáticas.
