CORRECCIÓN DATOS ORDENADOS - ORDEN DE PEDIDOS

Cambios incluidos:
1. Mapeo estricto por encabezados en Apps Script y JavaScript.
2. Ya no se usa posición fija para ESTADO, DESCRIPCION, PIKEADOR ni CANTIDAD cuando hay encabezados.
3. Si la columna ESTADO no existe o viene inválida, se usa PENDIENTE y no se copia DESCRIPCIÓN.
4. Al importar XLSX, se compara contra PEDIDOS y solo se agregan nuevos o cambios.
5. Los campos se guardan en orden fijo:
   id, fecha, pedido, cliente, vendedor, pikeador, codigo, descripcion, ubicacion, cantidad, status, alerta_token, alerta_ts, alerta_tipo, alerta_mensaje

IMPORTANTE:
Después de pegar apps_script.gs, publicar NUEVA IMPLEMENTACIÓN WEB APP.
