# Simplixity Portfolio

Portafolio creativo de Simplixity construido con Astro, Tailwind CSS, Lenis y GSAP. Incluye una landing inmersiva y una biblioteca de narrativas con bitácoras interactivas tipo flipbook.

## Comandos

```bash
npm install
npm run dev
npm run check
npm run build
npm run preview
```

Rutas principales:

- `/`: presentación de la agencia, trabajo, servicios, método y contacto.
- `/narrativas`: biblioteca de proyectos y bitácora interactiva.

## Estructura

```text
src/
  components/
    audio/        Reproductores reutilizables
    landing/      Secciones de la portada
    layout/       Navegación y loader globales
    narratives/   Flipbook, páginas y biblioteca
  data/           Contenido estructurado de la interfaz
  layouts/        Documento y metadatos compartidos
  pages/          Rutas de Astro
  scripts/        Lenis, GSAP y control global de audio
  styles/         Tokens, Tailwind y estilos base
public/
  brand/          Logos y tipografía de marca
  media/          Recursos optimizados usados en producción
docs/
  prototypes/     HTML de referencia, fuera del runtime
  references/     Brand sheet y composiciones visuales
```

La arquitectura y las decisiones de medios están descritas en [`docs/ARCHITECTURE.md`](docs/ARCHITECTURE.md). Los lineamientos visuales viven en [`DESIGN.md`](DESIGN.md) y el contexto de producto en [`PRODUCT.md`](PRODUCT.md).

## Contenido

- Datos de la agencia: `src/data/site.ts`.
- Proyectos, páginas y banda sonora: `src/data/narratives.ts`.
- Correo de contacto: `src/data/site.ts`.

Los recursos publicados deben usar nombres estables y formatos web: WebP para imágenes raster y MP3 para audio. Los archivos maestros no deben vivir en `public/` ni entrar al repositorio.
