# Diseño del Agente Operativo — Proyecto 03 (AORA)

## 1. Nombre del agente
AORA — Agente Operativo de Resumen y Acción

## 2. Objetivo del agente
Leer información (correos, documentos, notas), resumirla, detectar tareas y ejecutar acciones automáticas, manteniendo trazabilidad y reportes operativos.

---

## 3. Capacidades principales
- Lectura de documentos (PDF, TXT, DOCX).
- Lectura de correos o mensajes.
- Resumen automático de contenido.
- Detección de tareas y acciones.
- Clasificación de tareas por prioridad.
- Ejecución de acciones automatizadas.
- Generación de reportes operativos.
- Registro de actividad.
- Panel de control en Streamlit.

---

## 4. Entradas del sistema
- Documentos cargados por el usuario.
- Correos o textos.
- Parámetros operativos (prioridad, tipo de acción).
- Preguntas del usuario.
- Solicitudes de ejecución.

---

## 5. Procesos internos del agente

### A. Ingesta
- Recibe documentos o textos.
- Valida formato.
- Extrae contenido.

### B. Resumen
- Genera resumen ejecutivo.
- Identifica puntos clave.
- Detecta información relevante.

### C. Detección de tareas
- Busca acciones explícitas (“hacer”, “enviar”, “actualizar”).
- Detecta tareas implícitas.
- Clasifica por prioridad.
- Asigna categoría (operativa, administrativa, técnica).

### D. Ejecución automática
- Ejecuta acciones simples:
  - mover archivos,
  - generar reportes,
  - crear notas,
  - registrar tareas,
  - enviar información al panel.
- Marca tareas como completadas.

### E. Reporte operativo
- Genera un informe de:
  - tareas detectadas,
  - tareas ejecutadas,
  - tareas pendientes,
  - resumen del documento,
  - acciones automáticas realizadas.

### F. Registro y trazabilidad
- Guarda logs de:
  - fecha,
  - documento,
  - tareas,
  - acciones,
  - resultados.

---

## 6. Salidas del sistema
- Resumen del documento.
- Lista de tareas detectadas.
- Acciones ejecutadas.
- Reporte operativo.
- Registro de actividad.
- Visualización en el panel.

---

## 7. Reglas de decisión
- Priorizar tareas urgentes.
- No ejecutar acciones sin confirmación si son críticas.
- Resumir siempre antes de actuar.
- Registrar todo lo que hace.
- Mantener claridad y trazabilidad.

---

## 8. Impacto esperado
- Reducción de carga operativa.
- Menos tareas manuales.
- Mayor claridad en documentos.
- Automatización de acciones repetitivas.
- Flujo operativo más eficiente.
