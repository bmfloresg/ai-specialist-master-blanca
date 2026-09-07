# Documentación del Proyecto — ALIF (Agente de Limpieza Inteligente de Fotos)

## 1. Descripción general
ALIF es un agente operativo diseñado para automatizar la clasificación y limpieza de imágenes en dispositivos móviles y ordenadores. Reduce la basura digital, organiza fotos y optimiza el almacenamiento mediante análisis con IA y reglas inteligentes.

## 2. Problema que resuelve
La acumulación de capturas de pantalla, fotos borrosas, duplicados y contenido irrelevante ocupa memoria y requiere tiempo para ser revisado manualmente. ALIF elimina esta tarea repetitiva.

## 3. Objetivos del proyecto
- Automatizar la limpieza de imágenes.
- Clasificar fotos según su contenido.
- Detectar rostros, capturas de pantalla y duplicados.
- Aplicar reglas de eliminación o movimiento.
- Generar reportes semanales de actividad.

## 4. Arquitectura del sistema
El sistema se compone de:
- Módulo de ingesta de imágenes.
- Módulo de análisis con IA.
- Motor de reglas.
- Módulo de acciones (mover, eliminar, conservar).
- Módulo de registro y reportes.

## 5. Flujo técnico
Trigger → Análisis IA → Motor de reglas → Acción → Log → Reporte

## 6. Reglas aplicadas
- Sin rostro → posible eliminación.
- Captura de pantalla → mover a “Screenshots”.
- Borrosa → eliminar.
- Duplicada → conservar la mejor versión.
- Texto importante → mover a “Documentos”.

## 7. Impacto esperado
- Ahorro de tiempo.
- Reducción de memoria ocupada.
- Organización automática.
- Menos tareas repetitivas.
- Mayor claridad en la gestión de fotos.

## 8. Próximas mejoras
- Integración con n8n o Make.
- Panel de control en Streamlit.
- Sincronización con almacenamiento en la nube.
- Notificaciones automáticas.
