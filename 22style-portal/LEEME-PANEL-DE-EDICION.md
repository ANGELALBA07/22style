# Cómo activar tu portal de edición — 22 Style

Este paquete incluye tu tienda (`index.html`) más un panel de edición en
`/admin` donde puedes cambiar productos, precios, textos y fotos con
formularios, sin tocar código.

## Qué hay en esta carpeta
- `index.html` → tu tienda
- `data/products.json` → el catálogo (lo edita el panel automáticamente)
- `admin/index.html` y `admin/config.yml` → el panel de edición
- `images/uploads/` → aquí se guardan las fotos que subas desde el panel

## Pasos para activarlo (una sola vez)

1. **Sube esta carpeta a GitHub**
   - Crea una cuenta en https://github.com si no tienes.
   - Crea un repositorio nuevo y sube todos estos archivos y carpetas tal cual están.

2. **Conecta el repositorio a Netlify**
   - Entra a https://app.netlify.com
   - "Add new site" → "Import an existing project" → elige GitHub → selecciona tu repositorio.
   - Déjalo publicar con la configuración por defecto (no hace falta build command).

3. **Activa el login (Netlify Identity)**
   - En el panel de tu sitio en Netlify: `Site settings` → `Identity` → `Enable Identity`.

4. **Activa Git Gateway** (permite que el panel guarde los cambios)
   - Dentro de `Identity` → `Services` → `Git Gateway` → `Enable Git Gateway`.

5. **Invítate como usuaria**
   - En `Identity` → `Invite users` → escribe tu correo.
   - Te llega un email de Netlify: ábrelo y crea tu contraseña.

6. **Entra a tu panel**
   - Ve a `https://tu-sitio.netlify.app/admin`
   - Inicia sesión con tu correo y contraseña.
   - Ahí puedes: editar nombre, precio, precio anterior, descripción, color
     y foto de cada producto (la foto se sube arrastrándola, directo desde tu celular o PC).

7. Cada vez que guardes un cambio en el panel, tu tienda se actualiza sola
   en uno o dos minutos.

## Alternativa más simple (sin GitHub)
Si prefieres no usar GitHub, puedes conectar la tienda a una Google Sheet en
su lugar (más simple de configurar, pero sin login ni subida directa de fotos).
Esa opción está explicada dentro de `index.html`, al final del `<script>`,
en la constante `SHEET_CSV_URL`.
