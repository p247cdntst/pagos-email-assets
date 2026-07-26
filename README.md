# pagos-email-assets

Imágenes públicas para las campañas de email de Pagos247 (lanzamiento PIX Brasil).
Se sirven por HTTPS vía jsDelivr — los clientes de correo (Gmail, Outlook) bloquean base64,
así que todo `<img src>` de los emails apunta aquí.

## Base URL

```
https://cdn.jsdelivr.net/gh/p247cdntst/pagos-email-assets@main/
```

## Archivos

| Archivo | Tamaño real | Uso |
|---|---|---|
| `logo-navy.png` | 487×98 | Logo horizontal navy (header sobre fondo claro) |
| `logo-white.png` | 487×98 | Logo horizontal blanco (footer oscuro) |
| `logo-white-mark.png` | 278×186 | Isotipo blanco |
| `logo-lime-mark.png` | 278×186 | Isotipo lime |
| `hero-pix.png` | 1040×360 | Hero del email de lanzamiento |
| `step-1.png`, `step-2.png`, `step-3.png` | 2084×1324 | Capturas de los 3 pasos de activación |
| `activation-loop.gif` | 1040×708 | Los mismos 3 pasos animados (3 frames, 3,5 s cada uno, bucle infinito, 124 KB) |
| `icon-instant.png`, `icon-free.png`, `icon-key.png` | 80×80 | Iconos de beneficios |
| `push-icon.png` | 120×120 | Icono de notificación push |

## Notas

- Rama `main` fijada en la URL. Si se reemplaza una imagen conservando el nombre, jsDelivr
  seguirá sirviendo la versión cacheada: purgar en https://www.jsdelivr.com/tools/purge
  o pasar a un tag de versión (`@v2`) en vez de `@main`.
- Las imágenes están sobredimensionadas para retina; el ancho de render se fuerza con los
  atributos `width`/`height` en el HTML del email.
- `activation-loop.gif`: Outlook de escritorio en Windows no anima los GIF, muestra solo el
  primer frame (el diálogo «Add Recipient»). El paso de la clave PIX está en el frame 3, así
  que si el mensaje depende de verlo, conviene mantener los `step-*.png` estáticos al lado
  o aceptar que esa parte se pierde en Outlook.
