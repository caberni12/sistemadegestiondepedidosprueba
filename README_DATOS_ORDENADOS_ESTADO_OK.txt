CORRECCIÓN DATOS CRUZADOS - CAMPO ESTADO

Problema corregido:
- En algunas filas, la columna ESTADO/STATUS mostraba DESCRIPCIÓN de productos.
- Se dejó mapeo estricto por encabezado: ESTADO solo se lee desde status/estado/estado pedido/estado del pedido.
- Si el valor del estado no está permitido, se fuerza a PENDIENTE.
- El Apps Script agrega acción de reparación:
  ?accion=reparar_estados_pedidos

Estados permitidos:
PENDIENTE, PREPARACION, RECIBIDO, RECEPCIONADO, DESPACHADO, EN RUTA, ENTREGADO, TERMINADO, CANCELADO.

Pasos:
1. Reemplazar apps_script.gs en Apps Script.
2. Publicar nueva implementación Web App.
3. Ejecutar una vez:
   /exec?accion=reparar_estados_pedidos
4. Luego cargar:
   /exec?accion=listar_pedidos&mostrarTodo=1

La TD de Orden de Pedidos ahora mostrará el estado limpio y no descripción.
