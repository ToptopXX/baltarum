# BALTARUM

BALTARUM is a small web monorepo containing the project's public landing page and a separate browser-game demo. The two applications are intentionally independent and can be developed or deployed from their own directories.

## Applications

- `apps/landing` — a Next.js 14 landing site using React 18.
- `apps/game` — a Vite and React browser demo with Framer Motion and Tailwind CSS.

## Local development

Each application manages its own dependencies.

### Landing site

```bash
cd apps/landing
npm install
npm run dev
```

Create a production build with `npm run build`, then run it with `npm start`.

### Browser demo

```bash
cd apps/game
npm install
npm run dev
```

Create a production build with `npm run build` and inspect it locally with `npm run preview`.

## Repository structure

```text
.
|-- apps/
|   |-- game/       # Vite browser demo
|   `-- landing/    # Next.js landing site
`-- README.md
```

## Deployment

The applications can be imported into separate Vercel projects by selecting the corresponding app directory as the project root:

- `apps/landing` for the landing site.
- `apps/game` for the browser demo.

The existing project documentation maps `baltarum.com` to the landing app and `play.baltarum.com` to the game app.
