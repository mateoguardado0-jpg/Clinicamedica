# Instrucciones para Ejecutar el Sitio Web

## Requisitos Previos

Antes de ejecutar el proyecto, necesitas tener instalado:

1. **Node.js** (versión 16 o superior)
   - Descarga desde: https://nodejs.org/
   - Esto incluye npm (Node Package Manager)

## Pasos para Ejecutar

### 1. Verificar que Node.js está instalado

Abre PowerShell o CMD y ejecuta:
```bash
node --version
npm --version
```

Si ves números de versión, Node.js está instalado correctamente.

### 2. Instalar las dependencias

En la carpeta del proyecto, ejecuta:
```bash
npm install
```

Esto instalará todas las dependencias necesarias (React, Vite, React Router, etc.)

### 3. Ejecutar el servidor de desarrollo

Una vez instaladas las dependencias, ejecuta:
```bash
npm run dev
```

### 4. Abrir en el navegador

El comando anterior mostrará una URL, generalmente:
```
http://localhost:5173
```

Abre esta URL en tu navegador para ver el sitio web.

## Solución de Problemas

### Error: "npm no se reconoce"
- Significa que Node.js no está instalado o no está en el PATH
- Instala Node.js desde https://nodejs.org/
- Reinicia la terminal después de instalar

### Error: "Cannot find module"
- Ejecuta `npm install` nuevamente
- Asegúrate de estar en la carpeta correcta del proyecto

### El sitio no carga
- Verifica que el servidor esté corriendo (deberías ver un mensaje en la terminal)
- Asegúrate de usar la URL correcta que muestra Vite
- Revisa la consola del navegador (F12) para ver errores

## Comandos Útiles

- `npm run dev` - Inicia el servidor de desarrollo
- `npm run build` - Crea una versión de producción
- `npm run preview` - Previsualiza la versión de producción

