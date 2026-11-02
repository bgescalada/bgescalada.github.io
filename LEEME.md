# CalistenIA — PWA

## Despliegue
1. Copiá el contenido de esta carpeta a `/srv/calistenia` (o al root de GitHub Pages / Netlify).
2. Servilo por **HTTPS** (obligatorio para service worker / offline). Ver `Caddyfile.example` o `nginx.conf.example`.
3. En el iPhone: Safari → URL → Compartir → **Añadir a pantalla de inicio**.

## Actualizar
Reemplazá `index.html` y subí `VERSION` en `sw.js`. La app toma la nueva versión al reabrirla (a veces hace falta cerrarla y abrirla dos veces).

## Datos
- Se guardan en `localStorage` del origen. La PWA instalada en iOS tiene su **propio almacenamiento**, separado de Safari.
- Export backup → abre la hoja de compartir → "Guardar en Archivos".
- Si migrás desde la versión en claude.ai, los datos no se trasladan solos: no hay export allí; anotá a mano o empezá limpio.
- iOS puede borrar datos de webs no usadas en ~7 días, pero las apps añadidas a pantalla de inicio están exentas. Igual, hacé backups.
