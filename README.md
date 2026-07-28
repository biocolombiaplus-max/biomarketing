# Bio Marketing — Landing y portafolio de servicios

Landing page única y compartible de **Bio Marketing**: presenta los cuatro
productos tecnológicos del grupo (Biosoft, BioFutbol, Bio Contador, Bio
Finanzas), el servicio de manejo de redes sociales para empresas de salud
(planes Básico, Intermedio y Empresarial), y los servicios de automatización
de procesos con IA y cursos/talleres de Inteligencia Artificial.

Sitio 100% estático (HTML/CSS/JS, sin build ni dependencias de servidor),
listo para publicarse con GitHub Pages.

## Estructura

- **`index.html`** — la landing completa (una sola página).
- **`assets/biofinanzas-logo.jpg`** — logo real de Bio Finanzas.

Cada producto y cada plan tiene su propio botón de WhatsApp con un mensaje
ya redactado, que abre `wa.me/573505457420` (WhatsApp de Bio Marketing) con
el texto correspondiente.

## Publicar el sitio (GitHub Pages)

1. En este repositorio ve a **Settings → Pages**.
2. En "Build and deployment" → Source, elige **Deploy from a branch**.
3. Selecciona la rama `main` y la carpeta **`/ (root)`** → **Save**.
4. En un par de minutos el sitio queda publicado en
   `https://biocolombiaplus-max.github.io/biomarketing/` — ese es el link
   que puedes compartir con cualquier persona que pida información de la
   empresa.

## Personalizar

- **Número de WhatsApp / correo**: aparecen repetidos a lo largo de
  `index.html` (`wa.me/573505457420` y `biomarketing.salud@gmail.com`).
  Reemplaza ambos con buscar y reemplazar si cambian.
- **Precios de los planes de redes sociales**: sección `id="redes-salud"`
  en `index.html`, dentro de `.pricing-grid` (tres bloques `.plan`).
- **Logos**: los de Biosoft, BioFutbol y Bio Contador son íconos SVG
  embebidos directamente en el HTML (fáciles de recolorear). El de Bio
  Finanzas es la imagen real en `assets/biofinanzas-logo.jpg`. Para poner
  un logo real de Biosoft o Bio Contador cuando existan, reemplaza el
  `<svg>` correspondiente por una etiqueta `<img>` apuntando a un archivo
  en `assets/`.
- **Logo de Bio Marketing**: hoy es un ícono SVG (anillo morado/naranja +
  "BM") inspirado en el logo real del grupo. Si quieres usar el archivo de
  logo original en PNG, agrégalo en `assets/biomarketing-logo.png` y
  reemplaza el bloque `<svg class="brand-mark">` (aparece en el `nav` y en
  el `footer`) por un `<img src="assets/biomarketing-logo.png">`.
