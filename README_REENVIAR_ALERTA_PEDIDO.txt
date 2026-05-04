AJUSTE: BOTÓN ENVIAR ALERTA NUEVAMENTE

Se agregó la opción para reenviar la alerta de una orden ya existente sin duplicar el pedido.

FUNCIONAMIENTO:
1. En Orden de Pedidos, cada pedido activo muestra el botón "Enviar alerta nuevamente".
2. En el modal de detalle también aparece el botón "Enviar alerta nuevamente".
3. Al presionarlo, el sistema marca el pedido en la hoja PEDIDOS con:
   - alerta_token
   - alerta_ts
4. Los otros dispositivos, al cargar o sincronizar la lista, detectan ese nuevo token y vuelven a mostrar la tarjeta de alerta tipo Uber/Didi.
5. No duplica productos ni cambia la ubicación.
6. No cambia el estado del pedido, sólo reactiva la alerta.

IMPORTANTE:
- Reemplaza el apps_script.gs en Google Apps Script.
- Guarda y vuelve a desplegar el Web App.
- Usa la URL publicada actual en config.txt.
