# pagos-email-assets

Imágenes públicas para las campañas de email de Pagos247 (lanzamiento PIX Brasil).
Se sirven por HTTPS vía jsDelivr — los clientes de correo (Gmail, Outlook) bloquean base64,
así que todo `<img src>` de los emails apunta aquí.

## Base URL

```
https://cdn.jsdelivr.net/gh/pdvarela/pagos-email-assets@main/
```

## Archivos

| Archivo | Uso |
|---|---|
| `logo-white.png` | Logo horizontal blanco (header sobre navy) |
| `logo-navy.png` | Logo horizontal navy (fondo claro) |
| `logo-white-mark.png` | Isotipo blanco |
| `logo-lime-mark.png` | Isotipo lime |
| `hero-pix.png` | Hero del email 01 (lanzamiento) |
| `step-1.png`, `step-2.png`, `step-3.png` | Capturas de los 3 pasos (email 02) |
| `icon-instant.png`, `icon-free.png`, `icon-key.png` | Iconos de beneficios |
| `push-icon.png` | Icono de notificación push |

## Notas

- Rama `main` fijada en la URL. Para invalidar caché de jsDelivr tras reemplazar una imagen,
  usar un tag de versión (`@v2`) en vez de `@main`, o purgar en https://www.jsdelivr.com/tools/purge
- Las imágenes están a 2x para pantallas retina; el ancho se fuerza por atributo `width` en el HTML.
