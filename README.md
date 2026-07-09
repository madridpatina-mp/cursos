# Cursos MadridPatina — web de estadísticas

Web estática con todos los datos de la sección de cursos (2012-2026).

## Archivos
- `index.html` — la web completa (gráficos interactivos con Chart.js)
- `data.js` — los 693 cursos en JSON
- `cursos.csv` — los mismos datos en CSV (Excel, separador `;`)

## Cómo publicarla en GitHub Pages
1. Crea un repositorio en github.com (p. ej. `cursos-madridpatina`).
2. Sube los 3 archivos de esta carpeta (`index.html`, `data.js`, `cursos.csv`).
3. En el repositorio: **Settings → Pages → Source: Deploy from a branch → Branch: main / (root) → Save**.
4. En 1-2 minutos la web estará en `https://TU-USUARIO.github.io/cursos-madridpatina/`.

## Cómo actualizar los datos
Regenera `data.js` (y `cursos.csv`) con los datos nuevos del gestor manteniendo el mismo formato
de campos y sube el archivo; la web se actualiza sola.

Datos extraídos del gestor de madridpatina.com el 09/07/2026.
