# Turpialcut · seguimiento de pedidos

Página pública y estática que muestra el avance de un pedido a partir de su código de seguimiento
(`?c=CODIGO` o `#CODIGO`). Solo lee el documento público `seguimiento/{código}` de Firestore; no muestra teléfono, RUT ni precios.

- No contiene claves ni datos de clientes.
- Publicada con GitHub Pages (rama `main`, carpeta raíz).


## /vender/ — página de ventas (Turpialcut)
Página para registrar ventas desde el navegador del teléfono/PC: inicia sesión con el mismo usuario de la app, usa el mismo local y los mismos
pedidos (Firebase), asigna folio atómico y publica el seguimiento. No contiene secretos: la clave pública del proyecto se entrega una sola vez en el
enlace (`/vender/#k=…`) y queda guardada solo en ese teléfono. Opcional: `&app=https://…` guarda el enlace de instalación de la app para invitar al cliente.
