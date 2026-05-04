VERSION IMPORTACION XLSX ERGONOMICA Y VALIDADA

Cambios incluidos:
1. Plantilla Plantilla_Importar_Pedidos_Ergonomica.xlsx con columnas claras.
2. Modal de importación valida cada fila contra la hoja PEDIDOS.
3. Estados de previsualización: Nuevo, Cambio, Sin cambio, Error.
4. Al enviar a base de datos, no duplica.
5. Apps Script actualiza solo campos cambiados cuando encuentra el mismo PEDIDO + CODIGO.
6. Si el pedido existe pero llega un código nuevo, agrega solo esa línea de producto.

Reemplaza apps_script.gs en Google Apps Script y publica Nueva implementación Web App.
