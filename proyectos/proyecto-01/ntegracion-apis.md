# Integración con APIs — Proyecto 01 (ALIF)

## 1. Objetivo de la integración
Conectar ALIF con servicios externos de visión por computadora y almacenamiento para analizar imágenes y gestionar archivos de forma automática.

---

## 2. APIs de visión posibles
- API de detección de rostros.
- API de clasificación de imágenes.
- API de OCR (texto en imágenes).

Cada API debe permitir:
- Enviar una imagen.
- Recibir etiquetas (rostro, captura, documento, etc.).
- Recibir confianza del modelo.

---

## 3. Puntos de integración en el sistema

### A. En el análisis con IA
Desde n8n:
- Nodo HTTP Request → envía la imagen a la API.
- Recibe respuesta con:
  - `has_face`
  - `is_screenshot`
  - `is_blurry`
  - `is_duplicate`
  - `has_text`

### B. En el panel de control
Desde Streamlit:
- Consultar resultados de la API.
- Mostrar etiquetas y confianza.
- Permitir revisar casos dudosos.

---

## 4. Flujo de llamada a la API

1. ALIF detecta nueva imagen.
2. Preprocesa y normaliza.
3. Envía la imagen a la API de visión.
4. Recibe respuesta con atributos.
5. Pasa los atributos al motor de reglas.
6. Ejecuta acción (mover, eliminar, conservar).

---

## 5. Consideraciones técnicas
- Manejo de errores de la API.
- Límites de uso (rate limits).
- Seguridad y privacidad de las imágenes.
- Logs de llamadas a la API.

---

## 6. Próximos pasos
- Seleccionar API concreta.
- Definir formato de petición y respuesta.
- Implementar nodo HTTP en n8n.
- Probar con un conjunto pequeño de imágenes.
