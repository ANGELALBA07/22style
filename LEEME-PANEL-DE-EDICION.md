# 22 Style — Tienda con fotos reales, color y talla

Esta versión reemplaza COMPLETAMENTE la anterior: ya tiene tus 7 productos
reales, fotos optimizadas, tu logo, y selector de color + talla con stock.

## Qué cambió
- **7 productos reales** cargados con sus fotos: Body Coquette, Body Suite,
  Body Complete, Body Premium Lace, Body Premium Manga Corta, Body Premium
  Manga Larga y Body Zypper (cierre frontal).
- **Selector de color**: cada producto muestra sus colores reales como
  círculos de color; al tocar uno, cambia la foto principal.
- **Selector de talla con stock**: S / M / L / XL, cada uno mostrando las
  unidades disponibles. Las tallas agotadas aparecen tachadas y no se pueden
  elegir.
- **Fotos adicionales**: los productos que tenían más de una foto (detalle,
  con modelo, etc.) muestran una fila de miniaturas para verlas todas.
- **Logo real** ya cargado (`images/logo/logo.png`), visible en el header y
  el footer desde el primer momento.
- El carrito y el checkout ahora recuerdan el color y la talla elegidos.

## Qué hay en esta carpeta
- `index.html` → tu tienda
- `images/products/` → todas las fotos de producto, ya optimizadas
- `images/logo/logo.png` → tu logo real
- `data/products.json` → el catálogo completo (colores, tallas, stock, fotos)
- `data/site.json` → textos del banner principal, WhatsApp y TikTok
- `data/testimonials.json` → opiniones de clientas
- `data/faq.json` → preguntas frecuentes
- `admin/index.html` y `admin/config.yml` → el panel de edición
- `images/uploads/` → aquí se guardan las fotos nuevas que subas desde el panel

## Panel de edición — cómo se ve ahora
Dentro de "🛍️ Productos", cada producto se abre mostrando:
1. La **foto principal** de cada color (arriba, bien grande)
2. Un color con su **paleta visual** (tocas el cuadrito y eliges el tono)
3. Las **tallas y su stock**, con un menú desplegable para la talla y un
   número para el stock disponible
4. Un espacio para **fotos adicionales** de ese color (detalle, con modelo, etc.)

A la derecha, la **vista previa en vivo** muestra el producto tal cual se ve
en la web: foto, precio, y cada color con sus tallas — las agotadas se ven
en rosado y tachadas, igual que en la tienda real.

## Cómo subir esto a tu repositorio (reemplaza todo lo anterior)
1. Borra el contenido actual de tu repositorio en GitHub (o crea uno nuevo).
2. Sube **todo** el contenido de esta carpeta tal cual está (respetando las
   subcarpetas `images/`, `data/`, `admin/`).
3. Espera 1-2 minutos a que Netlify vuelva a publicar.
4. Entra a `tuweb.netlify.app/admin` con Ctrl+Shift+R (refresco sin caché)
   para confirmar que ves las 4 secciones y el nuevo editor de productos.

## Pendiente (opcional)
Tenías también una imagen de "efectos del producto" en chino/inglés para
traducir al español — no la incluí en esta versión porque es un gráfico con
texto superpuesto (no un simple texto), y reconstruirla con precisión requiere
que me compartas el texto exacto que quieres en cada etiqueta. Si me lo
mandas, te armo una sección de "beneficios" en español con ese contenido.
