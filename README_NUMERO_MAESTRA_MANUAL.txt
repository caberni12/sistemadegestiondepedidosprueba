VERSIÓN CORREGIDA - NÚMERO COMO PEDIDO + MAESTRA EN PEDIDO MANUAL

Cambios principales:
1) Importación XLSX/CSV:
   - Si el archivo trae columna NÚMERO, NUMERO, Nº, N° o NRO, ese valor se usa como PEDIDO.
   - Se mantiene el respaldo original de columnas importadas para no perder información.

2) Pedido manual:
   - Se agregó botón Sincronizar Maestra.
   - Al digitar código en el modal de Pedido Manual, busca en MAESTRA y completa la descripción.
   - También se puede presionar Buscar en Maestra.
   - Se agrega datalist de códigos para facilitar la carga.

3) Apps Script:
   - El servidor también reconoce NÚMERO como PEDIDO para evitar diferencias entre front y backend.
   - Mantiene acciones listar_maestra, buscar_producto y buscar_maestra.
