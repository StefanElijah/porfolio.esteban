# Porfolio de Esteban Pacheco Vega

Portfolio personal de Esteban Pacheco Vega, Ingeniero de Software Full Stack y Líder Técnico radicado en Santiago, Chile.

## Enlaces

- [Repositorio](https://github.com/StefanElijah/porfolio.esteban)
- [LinkedIn](https://www.linkedin.com/in/esteban-elias-pacheco-vega/)
- [GitHub](https://github.com/StefanElijah)
- [Email](mailto:esteban.pachecovega@gmail.com)

## Stack

![Astro Badge](https://img.shields.io/badge/Astro-FF3E00?logo=astro&logoColor=fff&style=flat)
![Tailwind CSS Badge](https://img.shields.io/badge/Tailwind%20CSS-06B6D4?logo=tailwindcss&logoColor=fff&style=flat)

Sitio construido con Astro, TypeScript y Tailwind CSS.

## Desarrollo

```bash
npm install
npm run dev
```

Para generar la versión de producción:

```bash
npm run build
```

Define la variable de entorno `SITE_URL` con tu dominio de producción para generar correctamente canonical, Open Graph y `robots.txt`:

```bash
SITE_URL=https://estebanpacheco.pages.dev npm run build
```

## Despliegue en Cloudflare Pages

El sitio es estático y no requiere adaptador. Configuración del proyecto:

| Opción | Valor |
| --- | --- |
| Production branch | `main` |
| Framework preset | Astro |
| Build command | `npm run build` |
| Output directory | `dist` |
| Root directory | `/` |

Variables de entorno en Production:

- `SITE_URL=https://estebanpacheco.pages.dev` (ajústala si el proyecto usa otro nombre)
- `NODE_VERSION=20`

Cada push a `main` se despliega automáticamente.

## Flujo de trabajo

- `Develop`: rama de desarrollo diario. Los pushes no generan despliegues.
- `main`: producción. Solo recibe merges desde `Develop` y dispara el despliegue en Cloudflare Pages.

## Licencia

MIT © 2026 Esteban Pacheco Vega.
