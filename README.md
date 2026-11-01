# hub

Página de inicio personal de Mauricio Romero Torres: un panal de hexágonos violeta en el que las celdas naranjas (naranja Princeton, `#E77500`) son enlaces a mis sitios y perfiles.

Es un solo archivo, `index.html`, sin dependencias ni paso de compilación. La foto es `profile.jpeg`.

## Editar los enlaces

Cada celda-enlace es un `<a class="cell link">` dentro de `<nav class="cluster">`. Su posición en el panal la dan las coordenadas axiales `data-q` y `data-r`; la foto ocupa la celda `(0, 0)`.

```html
<a class="cell link" data-q="1" data-r="-1" href="https://mromerot.github.io/SIDRo/"
   data-desc="Texto que aparece en la barra inferior al pasar el cursor.">
  <span class="face"><span class="label">SIDRo</span><span class="sub">Los Rosales, Bogotá</span></span>
  …
</a>
```

Las seis celdas vecinas de `(0, 0)` son `(0,-1)`, `(1,-1)`, `(1,0)`, `(0,1)`, `(-1,1)` y `(-1,0)`.

## Publicar

En GitHub: **Settings → Pages → Build and deployment → Deploy from a branch**, rama `main`, carpeta `/ (root)`. La página queda en `https://mromerot.github.io/hub/`.
