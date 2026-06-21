# Consulta de lineas registradas

Proyecto base para consultar lineas registradas desde una interfaz web simple.

## Estado actual

- Estructura inicial creada.
- Vista principal en `src/index.html`.
- Servidor de desarrollo configurado con Vite.

## Requisitos

- Node.js 18+ (recomendado 20+)
- pnpm

## Primeros pasos

1. Instala dependencias:
   `pnpm install`
2. Inicia el proyecto:
   `pnpm start`

Al ejecutar `pnpm start`, se abre automaticamente el navegador en `http://localhost:5173/` cargando `src/index.html`.

## Scripts disponibles

- `pnpm start`: inicia Vite en modo desarrollo.
- `pnpm run build`: genera el build optimizado para produccion.
- `pnpm run preview`: levanta una vista previa del build local.

## Deploy en Vercel

El proyecto esta configurado para compilar con Vite y publicar el resultado en `dist`.

- Comando de build: `pnpm run build`
- Directorio de salida: `dist`

Esta configuracion vive en `vercel.json` y usa `vite.config.js` con `root: 'src'`, por lo que Vercel renderiza correctamente `src/index.html` como entrada principal.
