Corrección aplicada:

- En la importación XLSX/CSV, la columna NÚMERO / NUMERO / Nº / N° / NRO / NO ahora se interpreta como PEDIDO.
- También se siguen aceptando PEDIDO, NRO PEDIDO, NUMERO PEDIDO, NÚMERO PEDIDO y ORDEN.
- El valor original del archivo se conserva en import_raw_json/import_headers_json para no perder información.
- El Apps Script también acepta numero/número/NUMERO/NÚMERO/N°/Nº como pedido al guardar.

Después de reemplazar apps_script.gs, publica una Nueva implementación Web App.
