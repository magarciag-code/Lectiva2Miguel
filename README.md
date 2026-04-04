# Prueba Lectiva

Base SvelteKit con arquitectura `feature-first/domain-first` para integrar la API de Rick and Morty.

## Run

```bash
npm install
npm run dev
```

## Check

```bash
npm run check
npm run build
```

## CI/CD

El proyecto queda preparado para GitHub Pages con GitHub Actions:

```bash
.github/workflows/deploy.yml
```

- Ejecuta `npm ci`, `npm run check` y `npm run build`.
- Publica automaticamente en GitHub Pages cada vez que hay un push a `main`.
- Usa `BASE_PATH` con el nombre del repositorio para que funcione en `/<repo>`.

## Estructura

- `src/lib/core`: cliente HTTP, configuracion y adaptadores.
- `src/lib/entities`: tipos y mapeos de dominio.
- `src/lib/features`: features por caso de uso.
- `src/routes`: composicion de rutas y carga de datos.
