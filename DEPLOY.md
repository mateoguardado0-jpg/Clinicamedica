# Cómo Publicar el Sitio Web

## Estado Actual
El sitio actualmente solo funciona en **localhost** (solo accesible desde tu computadora). Para que sea público en internet, necesitas desplegarlo en un servicio de hosting.

## Opciones de Hosting Gratuito

### 1. Vercel (Recomendado - Más Fácil)
**Gratis y muy fácil de usar**

1. Ve a https://vercel.com
2. Crea una cuenta (puedes usar GitHub)
3. Instala Vercel CLI:
   ```bash
   npm install -g vercel
   ```
4. En la carpeta del proyecto, ejecuta:
   ```bash
   vercel
   ```
5. Sigue las instrucciones en pantalla
6. ¡Listo! Tu sitio estará en línea en minutos

### 2. Netlify
**También gratis y fácil**

1. Ve a https://www.netlify.com
2. Crea una cuenta
3. Arrastra la carpeta `dist` (después de hacer build) a su sitio
4. O conecta tu repositorio de GitHub

### 3. GitHub Pages
**Gratis si tienes GitHub**

1. Crea un repositorio en GitHub
2. Sube tu código
3. Ve a Settings > Pages
4. Selecciona la rama y carpeta `dist`

## Pasos para Preparar el Sitio

### 1. Crear Build de Producción

Antes de desplegar, necesitas crear la versión optimizada:

```bash
npm run build
```

Esto creará una carpeta `dist` con los archivos listos para producción.

### 2. Probar el Build Localmente

```bash
npm run preview
```

Esto te permite ver cómo se verá el sitio en producción.

### 3. Desplegar

Elige una de las opciones de hosting arriba y sigue sus instrucciones.

## Configuración para React Router

Si usas Vercel o Netlify, necesitas crear un archivo de configuración:

### Para Vercel: `vercel.json`
```json
{
  "rewrites": [
    { "source": "/(.*)", "destination": "/index.html" }
  ]
}
```

### Para Netlify: `netlify.toml`
```toml
[[redirects]]
  from = "/*"
  to = "/index.html"
  status = 200
```

## Nota Importante

- El sitio en desarrollo (`npm run dev`) solo funciona en tu computadora
- Para que sea público, DEBES desplegarlo en un servicio de hosting
- La mayoría de servicios ofrecen planes gratuitos

