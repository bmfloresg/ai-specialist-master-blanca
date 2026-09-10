# Arquitectura del Sistema — Proyecto 03 (AORA)

## 1. Visión general
AORA es un agente operativo avanzado que combina:
- lectura de documentos,
- resumen automático,
- extracción de tareas,
- ejecución de acciones,
- reporting operativo,
- panel de control.

El sistema se organiza en módulos independientes que se comunican mediante un flujo claro y trazable.

---

## 2. Módulos principales

### Módulo A — Ingesta de información
- Lectura de documentos (PDF, TXT, DOCX).
- Lectura de correos o mensajes.
- Validación de formato.
- Extracción de texto.

### Módulo B — Resumen automático
- Generación de resumen ejecutivo.
- Identificación de puntos clave.
- Detección de información relevante.

### Módulo C — Detección de tareas
- Identificación de acciones explícitas.
- Detección de tareas implícitas.
- Clasificación por prioridad.
- Asignación de categoría (operativa, administrativa, técnica).

### Módulo D — Motor de acción
- Ejecución de tareas simples:
  - mover archivos,
  - generar reportes,
  - registrar tareas,
  - crear notas,
  - actualizar panel.
- Confirmación para tareas críticas.
- Registro de acciones ejecutadas.

### Módulo E — Reporte operativo
- Resumen del documento.
- Lista de tareas detectadas.
- Acciones ejecutadas.
- Tareas pendientes.
- Conclusiones operativas.

### Módulo F — Panel de control
- Visualización de tareas.
- Estado del agente.
- Reportes generados.
- Historial de acciones.
- Interacción con el usuario.

### Módulo G — Registro y trazabilidad
- Logs de:
  - fecha,
  - documento,
  - tareas,
  - acciones,
  - resultados.

---

## 3. Flujo de datos
Ingesta → Resumen → Tareas → Acción → Reporte → Panel → Log

---

## 4. Integraciones futuras
- Conexión con correo real.
- Integración con gestores de tareas.
- Automatización avanzada con n8n.
- Panel responsive para móvil.
