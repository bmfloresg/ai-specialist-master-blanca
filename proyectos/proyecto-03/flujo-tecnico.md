# Flujo Técnico — Proyecto 03 (AORA)

## 1. Trigger
El flujo se activa cuando:
- Se carga un documento (PDF, TXT, DOCX).
- Se recibe un texto o correo.
- El usuario solicita un resumen.
- El usuario solicita detección de tareas.
- El usuario solicita ejecución automática.

---

## 2. Ingesta de información
Acciones:
- Lectura del archivo o texto.
- Validación del formato.
- Extracción de contenido.
- Conversión a texto interno.

---

## 3. Resumen automático
El sistema:
- Genera un resumen ejecutivo.
- Identifica puntos clave.
- Detecta información relevante.
- Reduce ruido y redundancia.

---

## 4. Detección de tareas
El agente:
- Busca acciones explícitas (“enviar”, “actualizar”, “hacer”).
- Detecta tareas implícitas.
- Clasifica por prioridad.
- Asigna categoría (operativa, administrativa, técnica).
- Identifica dependencias entre tareas.

---

## 5. Ejecución automática
El motor de acción:
- Ejecuta tareas simples:
  - mover archivos,
  - generar reportes,
  - crear notas,
  - registrar tareas,
  - actualizar panel.
- Solicita confirmación para tareas críticas.
- Marca tareas como completadas.
- Registra resultados.

---

## 6. Generación del reporte operativo
El sistema produce:
- Resumen del documento.
- Lista de tareas detectadas.
- Acciones ejecutadas.
- Tareas pendientes.
- Conclusiones operativas.

---

## 7. Salida del sistema
El usuario recibe:
- Resumen.
- Tareas detectadas.
- Acciones realizadas.
- Reporte operativo.
- Registro de actividad.

---

## 8. Registro y trazabilidad
El sistema guarda:
- Fecha de ejecución.
- Documento procesado.
- Tareas detectadas.
- Acciones ejecutadas.
- Resultados.
- Logs completos.

---

## 9. Flujo completo
Trigger → Ingesta → Resumen → Tareas → Acción → Reporte → Salida → Log
