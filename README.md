# Propuesta Clínica Jiménez · UNISOFT

Configurador de la propuesta modular. El cliente elige módulos, alojamiento y forma de pago, y envía su selección por correo.

- Publicación: GitHub Pages (rama `main`, carpeta raíz).
- Envío de correo: Google Apps Script (`apps-script/Code.gs`) publicado como aplicación web desde el Gmail de UNISOFT. La selección llega a UNISOFT y el cliente recibe una copia.
- Un solo envío: después de enviar, la página queda bloqueada en ese navegador y muestra la selección enviada.

## Configurar el envío (una sola vez)
1. En https://script.google.com crear un proyecto nuevo y pegar `apps-script/Code.gs`.
2. Implementar → Nueva implementación → Aplicación web. Ejecutar como: Yo. Quién tiene acceso: Cualquier usuario.
3. Autorizar el acceso y copiar la URL que termina en `/exec`.
4. Reemplazar `PEGAR_AQUI_URL_APPS_SCRIPT` en `index.html` por esa URL.
