# Consulta de lineas registradas

Proyecto base para consultar lineas registradas desde una interfaz web simple usando Vite y Tailwind CSS v4.

## Stack

- Vite
- Tailwind CSS v4 (`tailwindcss` + `@tailwindcss/vite`)
- HTML/CSS/JS modular

## Requisitos

- Node.js `>=22`
- pnpm `11.8.0`

## Instalacion y desarrollo

1. Instala dependencias:
   `pnpm install`
2. Inicia el servidor de desarrollo:
   `pnpm start`

Al ejecutar `pnpm start`, se abre automaticamente `http://localhost:5173/`.

## Scripts disponibles

- `pnpm start`: inicia Vite en modo desarrollo.
- `pnpm run build`: genera build optimizado para produccion.
- `pnpm run preview`: sirve localmente el build de `dist`.

## Tailwind CSS

La hoja `src/styles.css` importa Tailwind con:

`@import "tailwindcss";`

Importante: como `vite.config.js` usa `root: "src"`, los assets dentro de `src` se referencian desde `/`.
Ejemplo correcto en `src/index.html`:

`<link rel="stylesheet" href="/styles.css">`

## Deploy en Vercel

El proyecto esta configurado para compilar con Vite y publicar en `dist`.

- Build command: `pnpm run build`
- Output directory: `dist`

Configuracion en `vercel.json`.
