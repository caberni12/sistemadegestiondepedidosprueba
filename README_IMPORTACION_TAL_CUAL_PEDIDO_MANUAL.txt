VERSIÓN ORDEN DE PEDIDOS - IMPORTACIÓN TAL CUAL + PEDIDO MANUAL

Cambios principales:
1. Importación XLSX/CSV preserva la fila original:
   - La previsualización muestra todas las columnas del archivo.
   - Se envían __raw y __rawHeaders al Apps Script.
   - Apps Script guarda import_raw_json e import_headers_json.
   - Si el archivo trae columnas extra que no existen en PEDIDOS, se agregan como columnas nuevas de forma segura.

2. Pedido manual:
   - Nuevo botón: ➕ Pedido manual.
   - Modal para crear pedido manual con fecha, pedido, cliente, vendedor, pikeador y estado.
   - Permite agregar múltiples productos antes de guardar.
   - Muestra previsualización con total de productos y unidades.
   - Guarda en PEDIDOS usando la misma validación de duplicados/cambios.

3. Protección de datos cruzados:
   - Estado solo acepta estados permitidos.
   - Pikeador no se carga desde Cliente.
   - Mapeo por encabezados, no por posición.

Recuerda reemplazar apps_script.gs y publicar una Nueva implementación Web App.
