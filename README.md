# Página pública de CV · Emilia Millón

Sitio estático en inglés (por defecto), español y portugués — botón EN / ES / PT arriba a la derecha; también `?lang=es` o `?lang=pt` en la dirección. Dos pestañas:
- `index.html` — CV completo en una página larga, con accesos a Research, Education, Publications, Teaching y Contact.
- `talks.html` — galería "Talks & seminars" con fotos de seminarios y presentaciones.

## Agregar fotos a la galería
1. Copiá la foto en `assets/gallery/` (jpg horizontal, ~1600 px de ancho alcanza).
2. Abrí `assets/gallery/gallery-data.js` con el Bloc de notas y escribí el nombre del archivo en `src:""` de la entrada que corresponda (o copiá una entrada y editá fecha, título, evento y lugar).
3. Las entradas sin foto muestran "Photo coming soon"; borrá las que no quieras.

## Archivos
- `assets/style.css` — estilos (paleta Mar del bosque, fondo oscuro, IBM Plex).
- `assets/CV_Emilia_Millon_EN.pdf`, `assets/CV_Emilia_Millon_ES.pdf` — CV descargables sin teléfono ni fecha de nacimiento.
- `.nojekyll` — publica los archivos tal cual.

## Publicar en GitHub Pages
Repositorio: https://github.com/emiliamillon/webpage → la página queda en https://emiliamillon.github.io/webpage/ (Settings → Pages → Deploy from a branch → `main` / root).
Después de cada cambio: commit + push (GitHub Desktop o `git add -A && git commit -m "update" && git push`).

## Actualizar el CV
Pedirle a Claude que regenere `index.html` desde la base (`CV_Master_Base_Emilia_Millon.md`) y los Word del CV.
