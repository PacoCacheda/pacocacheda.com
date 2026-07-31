# pacocacheda.com

Sitio personal de Francisco López Cacheda, servido por **GitHub Pages** desde la rama `main`, carpeta raíz.

El dominio está registrado en Squarespace, que actúa **solo como proveedor de DNS** (4 registros `A` a las IPs de GitHub Pages + `CNAME` de `www`). No hay suscripción de hosting de Squarespace.

## Este repo es solo la salida publicada

El sitio **no se edita aquí**. Se genera por código desde un proyecto local (`CV 2026/`), donde `content.py` es la fuente única de verdad y `build_html.py` produce el `index.html`.

Este repositorio contiene únicamente el resultado: el contenido de la carpeta local `CV 2026/site/`.

## Regla importante

⚠️ **Este repositorio es público, y el historial de git es permanente.** Un archivo subido por error sigue siendo consultable aunque se borre en un commit posterior.

Por eso **solo se sube el contenido de `CV 2026/site/`**. Nunca nada de la carpeta padre — en particular:

- `content.py` y los demás scripts de build, que incluyen datos de contacto privados
- Las variantes `_personal` y `_kairos` de los PDF, que llevan teléfono y email

Los PDF publicados aquí son la variante **`_web`**, generada expresamente sin datos de contacto directo. La página tampoco expone email ni teléfono: solo LinkedIn, GitHub y ubicación.

## Publicar cambios

1. Editar `content.py` en el proyecto local, manteniendo ES y EN en paralelo
2. Regenerar: `build_pptx.py`, `build_html.py`, `build_md.py`, y convertir los PPTX a PDF con LibreOffice
3. Copiar los archivos generados a `CV 2026/site/`
4. Subir el contenido de `site/` a la raíz de este repo

## Contenido

| Archivo | Qué es |
|---|---|
| `index.html` | El sitio completo, autocontenido (foto incluida en base64) |
| `CV_..._ES_web.pdf` / `_EN_web.pdf` | CV descargable, variante sin datos de contacto |
| `404.html` | Página de error |
| `CNAME` | Dominio personalizado para GitHub Pages |
| `robots.txt` / `sitemap.xml` | Indexación |
