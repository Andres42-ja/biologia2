# Cuaderno de campo: cómo instalarla en el celular

Esta carpeta es una app web instalable (PWA). Funciona sin conexión una vez instalada.

## 1. Publícala (una sola vez, gratis)
Para poder instalarla, el celular debe abrirla desde una dirección `https://`. Opciones gratuitas:

- **Netlify Drop** (la más rápida): entra a app.netlify.com/drop y arrastra esta carpeta completa. Te da un enlace.
- **GitHub Pages** o **Cloudflare Pages**: sube la carpeta a un repositorio y activa Pages.

No abras `index.html` directamente desde el almacenamiento del teléfono: así no se puede instalar.

## 2. Instálala
- **Android (Chrome):** abre el enlace → menú ⋮ → **Instalar app** (o **Añadir a pantalla de inicio**).
- **iPhone (Safari):** abre el enlace → botón Compartir → **Añadir a pantalla de inicio**.

Después de instalarla, aparece el ícono en tu pantalla y abre a pantalla completa, sin barra del navegador.

## 3. Importante
- Abre la app una vez con internet para que se guarde en el teléfono. Desde ahí funciona sin señal.
- Tus registros se guardan solo en ese teléfono. Usa **Ajustes → Descargar copia** de vez en cuando.
- Si cambias archivos de la app, sube el número de versión en `sw.js` (`const V`) para que los teléfonos se actualicen.

## Archivos
- `index.html`: la app completa.
- `manifest.webmanifest`: nombre, colores e íconos de la app.
- `sw.js`: permite el uso sin conexión.
- `logo.svg` e `icons/`: el logo en todos los tamaños.
