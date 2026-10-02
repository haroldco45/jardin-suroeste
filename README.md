# Jardín, Hispania y Andes en un día

App (PWA) para promocionar el pasadía al Suroeste antioqueño de **Viajamax**.
Asesora: **Alba Rosa Durán** — WhatsApp 317 676 8210.

Publicada en: https://haroldco45.github.io/jardin-suroeste/

## Qué hace
- Muestra los planes Básico ($150.000) y Full ($165.000) con lo que incluye cada uno.
- Arma la reserva (nombre, plan, personas, fecha, punto de encuentro) y la manda por WhatsApp a Alba.
- Puntos de encuentro con enlace al mapa, qué llevar y el flyer oficial.
- Galería de fotos de Jardín, Andes e Hispania traídas de Wikimedia Commons (licencia libre). El autor y la licencia de cada foto salen debajo automáticamente.
- Videos de YouTube de los tres pueblos, que se cargan solo cuando la persona toca el video.
- Se instala en el celular y abre sin señal la última versión vista.
- No guarda datos personales: solo viajan en el mensaje de WhatsApp que envía la persona.

## Archivos
```
index.html              la app
manifest.webmanifest    datos para instalarla
sw.js                   service worker
favicon.png
.nojekyll
img/hero.jpg            foto de portada
img/flyer.jpg           flyer oficial
img/og-image.jpg        imagen al compartir (1200×630)
img/icon-*.png          íconos
```

## Publicar en GitHub Pages
1. En GitHub (cuenta **haroldco45**) crea el repositorio público **jardin-suroeste**.
2. Botón **Add file → Upload files**. Sube todo el contenido de la carpeta, incluida la carpeta `img`. Ojo: `.nojekyll` es un archivo oculto; si no se ve, créalo con **Add file → Create new file** y déjalo vacío.
3. **Commit changes**.
4. **Settings → Pages → Source: Deploy from a branch → main / (root) → Save**.
5. A los 1–2 minutos queda en https://haroldco45.github.io/jardin-suroeste/

Si el repositorio lleva otro nombre, cambia la dirección en `index.html` (etiquetas `og:` y `twitter:` y `canonical`).

## Fotos y videos
- Las fotos se listan en `index.html`, en la lista `FOTOS` (pueblo + nombre exacto del archivo en Wikimedia Commons). Para agregar una, busca la foto en commons.wikimedia.org y copia el nombre del archivo tal cual.
- Los videos están en la lista `VIDEOS` (el código que va después de `watch?v=` en YouTube).
- No borres el crédito debajo de las fotos: es la condición de la licencia.
- Las fotos y videos solo se ven en la versión de GitHub Pages; en la vista previa de Claude aparecen enlaces.

## Actualizar
1. Cambia lo que necesites (precios, fechas, textos) en `index.html` y súbelo de nuevo.
2. En `sw.js` sube la versión: `jardin-suroeste-v2` → `jardin-suroeste-v3` (va en v2). Así los celulares que ya la tienen instalada reciben el cambio.
3. Si WhatsApp sigue mostrando la vista previa vieja, comparte el enlace con `?v=2` al final.

## Por confirmar con Alba
- Si el valor del plan es por persona (la calculadora lo multiplica por persona).
- Horario de atención fuera del viernes.

---
Desarrollada por **Vibras Positivas HM** — Derechos de Autor Reservados
