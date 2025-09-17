# Almacenamiento-web
Web estática educativa sobre tipos de almacenamiento de datos
# almacenamiento-web

Sitio estático educativo sobre tipos de almacenamiento de datos. Sin frameworks, solo HTML, Tailwind por CDN y JavaScript mínimo. Despliegue en Vercel sin CLI.

## Estructura

- `index.html` página principal con filtro, tarjetas, tabla comparativa, glosario y quiz.
- No hay subcarpetas ni dependencias. Puedes añadir más páginas luego.

## Cómo desplegar en Vercel sin CLI

1. Crea el repositorio en GitHub y sube `index.html` y este `README.md` a la rama `main`.
2. Ve a https://vercel.com e inicia sesión con tu cuenta de GitHub.
3. Pulsa **Add New Project** y luego **Import Git Repository**.
4. Autoriza a Vercel a acceder a tu cuenta si te lo pide y selecciona el repo `almacenamiento-web`.
5. Configuración del proyecto:
   - **Framework Preset**: `Other`.
   - **Build Command**: dejar vacío.
   - **Output Directory**: `.` (punto).
   - **Root Directory**: raíz del repo.
   - **Production Branch**: `main`.
6. Pulsa **Deploy**. Vercel construye y publica automáticamente.
7. Cuando termine, obtendrás una URL pública del tipo `https://almacenamiento-web.vercel.app/`.
8. Cada commit a `main` vuelve a desplegar automáticamente.

### Opcional recomendado

- **vercel.json** para URLs limpias y caché básica. Crea un archivo en la raíz con:
  ```json
  {
    "cleanUrls": true,
    "trailingSlash": false,
    "headers": [
      {
        "source": "/(.*)\\.html",
        "headers": [{ "key": "Cache-Control", "value": "public, max-age=3600" }]
      }
    ]
  }
