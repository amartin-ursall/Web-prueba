# Portfolio en Astro

Portfolio estático construido con Astro. Incluye secciones de presentación, habilidades, proyectos y contacto en una sola página.

## Scripts disponibles

- `npm run dev` — entorno de desarrollo en `http://localhost:4321`.
- `npm run build` — genera la versión estática en `dist/`.
- `npm run preview` — sirve la carpeta `dist/` de forma local.

## Docker

```sh
docker build -t astro-portfolio .
docker run -p 3000:80 astro-portfolio
```

La imagen utiliza una fase de build con Node.js y sirve los archivos estáticos con Nginx.

### Docker Compose

```sh
docker compose up --build
```

Publica la web en `http://localhost:3000`.

## Estructura

- `src/pages/index.astro`: página principal con la vista de portfolio.
- `public/`: recursos públicos.
- `Dockerfile` y `.dockerignore`: configuración para generar la imagen de producción.
