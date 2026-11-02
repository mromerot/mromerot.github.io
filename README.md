# mromerot.github.io

Página de inicio personal de Mauricio Romero Torres: un panal de hexágonos violeta en el que las celdas naranjas (naranja Princeton, `#E77500`) son enlaces a mis sitios y perfiles.

Es un solo archivo, `index.html`, sin dependencias ni paso de compilación.

## Editar los enlaces

Cada celda-enlace es un `<a class="cell link">` dentro de `<nav class="cluster">`. Su posición en el panal la dan las coordenadas axiales `data-q` y `data-r`; la celda central `(0, 0)` queda vacía, como parte del panal.

```html
<a class="cell link" data-q="1" data-r="-1" href="https://mromerot.github.io/SIDRo/"
   data-desc="Texto que aparece en la barra inferior al pasar el cursor.">
  <span class="face"><span class="label">SIDRo</span><span class="sub">Los Rosales, Bogotá</span></span>
  …
</a>
```

Las seis celdas vecinas de `(0, 0)` son `(0,-1)`, `(1,-1)`, `(1,0)`, `(0,1)`, `(-1,1)` y `(-1,0)`.

## Publicar

Este repositorio es el sitio de usuario de GitHub Pages: lo que esté en la rama `main` se publica en `https://mromerot.github.io/`. Si no se publica solo, actívalo en **Settings → Pages → Deploy from a branch**, rama `main`, carpeta `/ (root)`.

Los demás sitios (`/web/`, `/SIDRo/`, `/leticia/`, `/sincelejo/`, `/data.science/`) siguen publicándose desde sus propios repositorios.
