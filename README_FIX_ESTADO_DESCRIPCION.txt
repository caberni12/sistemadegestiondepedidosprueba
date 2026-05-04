CORRECCIÓN IMPORTADOR - CAMPO ESTADO

Problema corregido:
El campo ESTADO podía copiar valores de DESCRIPCIÓN cuando el importador tomaba columnas por posición.

Correcciones:
1. El importador ahora detecta ESTADO sólo por encabezado: status, estado, estado pedido, estado del pedido.
2. Si no existe columna ESTADO, usa PENDIENTE por defecto o el estado seleccionado en el modal.
3. Si viene un valor no permitido en ESTADO, lo ignora y no lo guarda como estado.
4. Apps Script valida nuevamente el estado antes de guardar en PEDIDOS.
5. Estados permitidos: PENDIENTE, PREPARACION, RECIBIDO, RECEPCIONADO, DESPACHADO, EN RUTA, ENTREGADO, TERMINADO, CANCELADO.

Después de subir apps_script.gs debes publicar Nueva implementación Web App.
