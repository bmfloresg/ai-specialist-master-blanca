# Panel de Control en Streamlit — Proyecto 02 (CRA)

## 1. Objetivo del panel
Proporcionar una interfaz clara y profesional para visualizar métricas, generar reportes, revisar insights y permitir interacción directa con el Copiloto Analítico.

---

## 2. Secciones del panel

### A. Dashboard principal
- Métricas clave (totales, medias, tendencias).
- Gráficas de evolución temporal.
- Indicadores de anomalías.
- Resumen ejecutivo generado automáticamente.

### B. Carga de datos
- Subida de archivos CSV o Excel.
- Subida de documentos PDF o TXT.
- Validación del archivo.
- Vista previa de los datos.

### C. Generación de reportes
- Selección de rango de fechas.
- Selección de métricas.
- Botón “Generar reporte”.
- Visualización del reporte completo.
- Descarga del reporte.

### D. Insights automáticos
- Lista de insights detectados.
- Explicación de tendencias.
- Señalización de anomalías.
- Recomendaciones generadas por el agente.

### E. Preguntas al copiloto
- Campo de texto para preguntas.
- Respuestas basadas en los datos cargados.
- Interpretación contextual.

### F. Historial de reportes
- Lista de reportes generados.
- Fecha de ejecución.
- Tipo de reporte.
- Descarga de versiones anteriores.

---

## 3. Componentes técnicos en Streamlit

### Layout
- `st.sidebar` para navegación.
- `st.tabs` para dividir secciones.
- `st.metric` para indicadores.
- `st.line_chart` para tendencias.
- `st.dataframe` para vista de datos.
- `st.text_area` para reportes.

### Backend
- Lectura de archivos.
- Procesamiento con pandas.
- Llamada al motor analítico.
- Generación de insights.
- Registro de reportes.

---

## 4. Flujo de datos del panel
Carga de archivo → Procesamiento → Interpretación → Reporte → Insights → Historial

---

## 5. Próximas mejoras
- Autenticación de usuario.
- Exportación en PDF.
- Panel responsive para móvil.
- Integración con bases de datos reales.
