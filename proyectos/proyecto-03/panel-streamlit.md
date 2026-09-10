# Panel de Control en Streamlit — Proyecto 03 (AORA)

## 1. Objetivo del panel
Proporcionar una interfaz operativa donde el usuario pueda cargar documentos, revisar resúmenes, ver tareas detectadas, ejecutar acciones y consultar reportes operativos.

---

## 2. Secciones del panel

### A. Dashboard principal
- Estado del agente.
- Tareas detectadas recientemente.
- Acciones ejecutadas.
- Resumen operativo del último documento.
- Indicadores clave (tareas pendientes, completadas, críticas).

### B. Carga de documentos
- Subida de archivos PDF, TXT, DOCX.
- Validación del archivo.
- Vista previa del contenido.
- Botón “Procesar documento”.

### C. Resumen automático
- Visualización del resumen ejecutivo.
- Puntos clave detectados.
- Información relevante.

### D. Tareas detectadas
- Lista de tareas identificadas.
- Prioridad (alta, media, baja).
- Categoría (operativa, administrativa, técnica).
- Dependencias entre tareas.
- Botón “Ejecutar tareas simples”.

### E. Acciones ejecutadas
- Registro de acciones realizadas por el agente.
- Resultados de cada acción.
- Confirmaciones solicitadas.
- Estado de ejecución.

### F. Reporte operativo
- Resumen del documento.
- Tareas detectadas.
- Acciones ejecutadas.
- Tareas pendientes.
- Conclusiones operativas.
- Descarga del reporte.

### G. Historial
- Documentos procesados.
- Fecha de ejecución.
- Tareas detectadas.
- Acciones realizadas.
- Reportes generados.

---

## 3. Componentes técnicos en Streamlit

### Layout
- `st.sidebar` para navegación.
- `st.tabs` para dividir secciones.
- `st.metric` para indicadores.
- `st.dataframe` para vista de tareas.
- `st.text_area` para resúmenes y reportes.
- `st.button` para acciones del agente.

### Backend
- Lectura de documentos.
- Procesamiento de texto.
- Resumen automático.
- Detección de tareas.
- Motor de acción.
- Registro de actividad.

---

## 4. Flujo del panel
Carga → Resumen → Tareas → Acción → Reporte → Historial

---

## 5. Próximas mejoras
- Integración con correo real.
- Conexión con gestores de tareas.
- Panel responsive para móvil.
- Automatización avanzada con n8n.
