# Documentación Final — Proyecto 01 (ALIF)

## 1. Resumen ejecutivo
ALIF (Agente de Limpieza Inteligente de Fotos) es un sistema de automatización con IA aplicada que clasifica, organiza y limpia imágenes de forma autónoma. Reduce la basura digital, optimiza almacenamiento y elimina tareas repetitivas.

---

## 2. Problema detectado
Los dispositivos acumulan:
- Capturas de pantalla
- Fotos borrosas
- Imágenes duplicadas
- Contenido irrelevante

Esto consume memoria y tiempo de revisión manual.

---

## 3. Solución propuesta
Un agente operativo que:
- Detecta rostros
- Identifica capturas de pantalla
- Evalúa nitidez
- Detecta duplicados
- Clasifica imágenes
- Aplica reglas de limpieza
- Genera reportes semanales

---

## 4. Arquitectura del sistema
El sistema se compone de:
- Módulo de ingesta
- Módulo de análisis con IA
- Motor de reglas
- Módulo de acciones
- Módulo de logs y reportes
- Panel de control en Streamlit

---

## 5. Pipeline completo
Entrada → Preprocesamiento → Análisis IA → Clasificación → Reglas → Acción → Log → Reporte

---

## 6. Implementación en n8n
El flujo incluye:
- Trigger de carpeta
- Preprocesamiento
- Llamada a API de visión
- Switch de clasificación
- IF de reglas
- Acciones (mover, eliminar, conservar)
- Registro en archivo
- Cron para reporte semanal

---

## 7. Integración con APIs
El sistema usa APIs de visión para:
- Detección de rostros
- Detección de capturas
- OCR
- Detección de duplicados

---

## 8. Panel de control
Streamlit permite:
- Ver estadísticas
- Revisar imágenes clasificadas
- Consultar reportes
- Ajustar reglas
- Ver estado del agente

---

## 9. Impacto del proyecto
- Ahorro de tiempo
- Reducción de memoria ocupada
- Organización automática
- Menos tareas repetitivas
- Mayor claridad en la gestión de fotos

---

## 10. Próximos pasos
- Implementación real del flujo en n8n
- Construcción del panel Streamlit
- Integración con almacenamiento en la nube
- Versión móvil del panel
