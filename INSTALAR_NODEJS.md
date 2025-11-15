# Cómo Instalar Node.js

## Pasos para Instalar Node.js en Windows

### 1. Descargar Node.js
1. Ve a: **https://nodejs.org/**
2. Haz clic en el botón verde que dice **"Download LTS"** (versión recomendada)
3. Se descargará un archivo `.msi`

### 2. Instalar Node.js
1. Abre el archivo descargado (ejemplo: `node-v20.x.x-x64.msi`)
2. Sigue el asistente de instalación:
   - Haz clic en "Next" en todas las pantallas
   - Acepta los términos y condiciones
   - Deja las opciones por defecto (incluye npm automáticamente)
   - Haz clic en "Install"
3. Espera a que termine la instalación
4. Haz clic en "Finish"

### 3. Verificar la Instalación
1. Cierra y vuelve a abrir PowerShell o CMD
2. Ejecuta estos comandos para verificar:
   ```bash
   node --version
   npm --version
   ```
3. Si ves números de versión (ejemplo: v20.10.0), ¡está instalado correctamente!

### 4. Ejecutar el Proyecto
Una vez instalado Node.js, en la carpeta del proyecto ejecuta:
```bash
npm install
npm run dev
```

## Nota Importante
- **Reinicia la terminal** después de instalar Node.js para que reconozca los comandos
- Si aún no funciona después de reiniciar, reinicia tu computadora

## ¿Problemas?
- Si el instalador no se ejecuta, haz clic derecho y selecciona "Ejecutar como administrador"
- Asegúrate de descargar la versión para Windows (64-bit)

