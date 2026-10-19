# YK LIQUORS

Sitio web de la licorería YK LIQUORS. Es un sitio estático: solo archivos HTML y CSS, sin instalación ni base de datos.

## Archivos

| Archivo | Qué contiene |
| --- | --- |
| `index.html` | Página principal (portada y datos de la tienda) |
| `catalogo.html` | Catálogo de productos con filtro por categoría |
| `combos.html` | Combos y paquetes |
| `nosotros.html` | Quiénes somos |
| `contacto.html` | WhatsApp, dirección y horario |
| `styles.css` | Estilos y colores de todo el sitio |

## Cómo verlo

Abre `index.html` con doble clic en cualquier navegador. Todas las páginas deben estar en la misma carpeta.

## Cómo editar

**Productos y precios.** Abre `catalogo.html` y busca la lista `items` dentro de la etiqueta `<script>`. Cada producto es una línea:

```js
{ n: "Ron añejo 12 años", c: "Ron", d: "Descripción corta.", s: "750 ml · 40% vol", p: 260 }
```

- `n`: nombre
- `c`: categoría (los botones de filtro se crean solos con las categorías que uses)
- `d`: descripción
- `s`: presentación y grado de alcohol
- `p`: precio en quetzales
- `img`: foto del producto (opcional), por ejemplo `img: "img/ron-anejo.jpg"`

Para agregar un producto, copia una línea y cambia sus datos. Para quitarlo, borra la línea.

**Fotos.** Crea una carpeta `img` junto a los archivos y guarda ahí las fotos. Usa imágenes verticales (proporción 4:5) y de menos de 300 KB cada una para que la página cargue rápido.

**Combos.** Edita los bloques `<div class="combo">` en `combos.html`.

**Teléfono, dirección y horario.** Edita `contacto.html`. Los valores actuales son de ejemplo.

**Colores.** Cambia las variables al inicio de `styles.css`. La paleta actual es blanco y negro.

## Pendiente

- Reemplazar los productos, precios y combos de ejemplo por los reales.
- Poner el número de WhatsApp, la dirección y el horario reales.
- Agregar las fotos de los productos.

## Aviso legal

El sitio muestra el aviso de venta solo a mayores de 18 años en la parte superior y en el pie de cada página. Mantenlo visible.

## Publicarlo

Para ponerlo en internet, sube toda la carpeta a un servicio de hosting estático (por ejemplo GitHub Pages, Netlify o Cloudflare Pages). `index.html` debe quedar en la raíz.
