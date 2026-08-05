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
- **`assets/logos/`** — los 5 logos del sitio, cada uno con nombre fijo
  (ver abajo cómo reemplazarlos por los reales).

Cada producto y cada plan tiene su propio botón de WhatsApp con un mensaje
ya redactado, que abre `wa.me/573505457420` (WhatsApp de Bio Marketing) con
el texto correspondiente.

## Subir un logo real (sin tocar código)

Todos los logos son archivos independientes en `assets/logos/`, así que para
poner el logo real de cualquier producto **no necesitas editar el HTML**:
solo reemplaza el archivo por uno tuyo que tenga el **mismo nombre exacto**.

| Producto | Archivo a reemplazar | Formato |
|---|---|---|
| Bio Marketing | `assets/logos/biomarketing.png` | PNG, cuadrado (ideal 512×512) |
| Biosoft | `assets/logos/biosoft.png` | PNG, cuadrado |
| BioFutbol | `assets/logos/biofutbol.png` | PNG, cuadrado |
| Bio Contador | `assets/logos/biocontador.png` | PNG, cuadrado |
| Bio Finanzas | `assets/logos/biofinanzas.jpg` | JPG, cuadrado |

Pasos en GitHub (sin instalar nada):

1. Entra a la carpeta `assets/logos` en este repositorio.
2. Clic en **Add file → Upload files**.
3. Arrastra tu logo nuevo — debe llamarse **exactamente igual** al que vas a
   reemplazar (por ejemplo `biosoft.png`), GitHub te va a preguntar si quieres
   sobrescribirlo.
4. Confirma el commit ("Commit changes").
5. En 1-2 minutos GitHub Pages se actualiza solo y el logo nuevo aparece en
   la landing — no hace falta tocar `index.html` para nada.

Si tu logo no es cuadrado, igual funciona: se ajusta automáticamente dentro
de un marco cuadrado sin recortarse ni deformarse.

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
- **Logos**: ver la sección "Subir un logo real" arriba — se reemplazan
  subiendo un archivo con el mismo nombre, sin tocar `index.html`.
