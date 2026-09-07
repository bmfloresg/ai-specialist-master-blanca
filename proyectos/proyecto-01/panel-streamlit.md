# Diseño del Panel de Control — Proyecto 01 (ALIF)

## 1. Objetivo del panel
Proporcionar una interfaz clara y profesional para visualizar el estado del agente ALIF, revisar estadísticas y gestionar reglas de limpieza.

---

## 2. Secciones del panel

### A. Dashboard principal
- Total de imágenes analizadas.
- Imágenes eliminadas.
- Imágenes movidas.
- Imágenes conservadas.
- Duplicados detectados.
- Gráfica semanal de actividad.

### B. Vista de imágenes clasificadas
- Lista de imágenes recientes.
- Categoría asignada (rostro, captura, borrosa, duplicada, documento, irrelevante).
- Acción aplicada (mover, eliminar, conservar).

### C. Reglas del sistema
- Activar/desactivar reglas.
- Ajustar sensibilidad de detección de rostros.
- Ajustar tolerancia de nitidez.
- Configurar carpeta de destino para capturas de pantalla.
- Configurar carpeta de documentos.

### D. Reporte semanal
- Resumen de actividad.
- Estadísticas.
- Descarga del reporte.
- Historial de semanas anteriores.

### E. Estado del agente
- Agente activo / pausado.
- Última ejecución.
- Próxima ejecución programada.

---

## 3. Componentes técnicos en Streamlit

### Layout
- `st.sidebar` para navegación.
- `st.tabs` para dividir secciones.
- `st.metric` para estadísticas rápidas.
- `st.image` para mostrar imágenes clasificadas.
- `st.dataframe` para logs y reportes.

### Backend
- Lectura de logs generados por n8n.
- Lectura de carpetas del sistema.
- Carga de imágenes en tiempo real.
- Integración con API de visión (opcional).

---

## 4. Flujo de datos del panel
n8n → Logs → Panel Streamlit  
n8n → Carpeta de imágenes → Panel Streamlit  
n8n → Reporte semanal → Panel Streamlit

---

## 5. Próximas mejoras
- Autenticación de usuario.
- Panel responsive para móvil.
- Exportación de reportes.
- Integración con nube (Drive, OneDrive).
