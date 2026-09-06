# Diseño del Agente — Proyecto 01 (ALIF)

## 1. Nombre del agente
Agente de Limpieza Inteligente de Fotos (ALIF)

## 2. Objetivo del agente
Reducir basura digital y optimizar almacenamiento mediante clasificación automática de imágenes.

## 3. Capacidades principales
- Detección de rostros
- Detección de capturas de pantalla
- Detección de imágenes borrosas
- Detección de duplicados
- Clasificación por categorías
- Aplicación de reglas de limpieza
- Generación de reportes semanales

## 4. Entradas del sistema
- Imagen nueva añadida al dispositivo
- Carpeta de fotos existente
- Metadatos de la imagen (fecha, tamaño, resolución)

## 5. Procesos internos
1. Análisis visual con IA
2. Clasificación por tipo de imagen
3. Evaluación de reglas
4. Decisión (conservar, mover, eliminar)
5. Registro en log
6. Preparación de reporte

## 6. Salidas del sistema
- Imagen movida
- Imagen eliminada
- Imagen marcada como importante
- Registro de acción
- Reporte semanal

## 7. Reglas de decisión
- Si no contiene rostro → posible eliminación
- Si es captura de pantalla → mover a “Screenshots”
- Si es borrosa → eliminar
- Si es duplicada → conservar la mejor versión
- Si contiene texto importante → mover a “Documentos”

## 8. Impacto esperado
- Ahorro de tiempo
- Reducción de memoria ocupada
- Organización automática
- Menos tareas repetitivas
