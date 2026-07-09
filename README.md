# Cursos MadridPatina ★ Estadísticas de la sección

Web estática con todos los datos de la sección de cursos del club (2012-2026):
693 cursos, gráficos interactivos, comparador por tipo de curso, perfiles de cara
a la temporada 2026-27 y recomendaciones.

## Estructura del proyecto

```
cursos-madridpatina/
├── index.html        ← la web (gráficos con Chart.js, estilo revista)
├── data.js           ← los 693 cursos en JSON (la web lee de aquí)
├── cursos.csv        ← los mismos datos en CSV para Excel (separador ;)
├── assets/
│   └── logo.svg      ← logotipo MadridPatina (vectorial)
├── datos/
│   └── Cursos_MadridPatina.xlsx  ← Excel completo con tabla y estadísticas
└── README.md
```

## Publicar en GitHub Pages (5 minutos)

1. Repositorio del proyecto: **github.com/madridpatina-mp/cursos**
2. En el repositorio: **uploading an existing file** (o Add file → Upload files)
   y arrastra TODO el contenido de esta carpeta (respetando las subcarpetas `assets` y `datos`).
   Pulsa **Commit changes**.
3. Ve a **Settings → Pages**. En *Source* elige **Deploy from a branch**,
   rama **main**, carpeta **/(root)**. Guarda.
4. En 1-2 minutos la web estará publicada en:
   `https://madridpatina-mp.github.io/cursos/`

### Alternativa con git (línea de comandos)

```bash
cd cursos-madridpatina
git init
git add .
git commit -m "Web de estadísticas de la sección de cursos"
git branch -M main
git remote add origin https://github.com/madridpatina-mp/cursos.git
git push -u origin main
```
Y después activa Pages como en el paso 3.

## Actualizar los datos cada temporada

1. Extrae los cursos nuevos del gestor y regenera `data.js` manteniendo los mismos
   campos (y `cursos.csv` si quieres).
2. Sube el archivo al repositorio (Upload files → reemplazar). La web se actualiza sola.

## Notas

- El logotipo es una reconstrucción vectorial: si tienes el archivo original
  (SVG/PNG), sustituye `assets/logo.svg` y todo seguirá funcionando.
- Datos extraídos del gestor de madridpatina.com el 09/07/2026. El gestor solo
  conserva histórico completo desde enero de 2024: exporta cada temporada para no perder datos.
