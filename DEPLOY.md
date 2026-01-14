# Deployment Guide

Este documento describe cómo construir y desplegar el portfolio localmente y automáticamente en GitHub Pages.

## Construcción Local

Para construir el proyecto localmente, sigue estos pasos:

```bash
# Instalar dependencias
npm ci

# Construir el proyecto
npm run build
```

La carpeta `./dist` contendrá los archivos estáticos listos para ser desplegados.

## Probar Localmente

Para probar la construcción localmente antes de desplegarla:

```bash
# Opción 1: Usar el servidor de preview de Vite
npm run preview

# Opción 2: Usar un servidor estático como serve
npx serve ./dist
```

Abre tu navegador y visita la URL que se muestre en la consola (normalmente `http://localhost:4173` para preview o `http://localhost:3000` para serve).

## Despliegue Automático

El sitio se despliega automáticamente en GitHub Pages cuando:
- Se hace push a la rama `main`
- El workflow de GitHub Actions (`pages.yml`) se ejecuta exitosamente

### URL de GitHub Pages

El portfolio está disponible públicamente en:

**https://JherreraHidalgo.github.io/my-portfolio/**

## Configuración

El proyecto está configurado con:
- **Base path**: `/my-portfolio/` (configurado en `vite.config.js`)
- **Build output**: `./dist`
- **Node.js version**: 18

## Solución de Problemas

Si el sitio no se muestra correctamente:

1. Verifica que el repositorio tenga GitHub Pages habilitado
2. Asegúrate de que el workflow tenga permisos para desplegar (Settings > Actions > General > Workflow permissions)
3. Revisa que la configuración de Pages use "GitHub Actions" como fuente (Settings > Pages > Source)
4. Comprueba los logs del workflow en la pestaña "Actions" del repositorio
