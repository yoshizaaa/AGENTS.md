# Pluto Design Agent Host

This repository is the home base for a Pluto Design Agent setup.

It currently contains agent instructions and project conventions only. The actual app has not been scaffolded yet.

## Project Map

Planned locations:

- Admin dashboard: `apps/admin`
- Backend routes: `apps/api` or `apps/web/src/app/api`
- Database schema: `packages/db/schema`
- Database migrations: `packages/db/migrations`
- Shared UI package: `packages/ui`
- Design documentation: `docs`

These are conventions, not existing app files yet.

## Environment Variables

Environment variables are not wired to an app yet.

Use `.env.example` as the starter template when an app is added.

## Local Development

There is no local app command yet.

Once an app scaffold exists, document the exact command here. Expected examples:

```bash
npm install
npm run dev
```

or, for a monorepo:

```bash
pnpm install
pnpm dev
```

## Agent Docs

- Repo-level agent instructions: `AGENTS.md`
- Design-agent guide: `docs/design-agent.md`
- Project map: `docs/project-map.md`

## Next Step

Choose the app foundation:

- Next.js single app
- Turborepo monorepo
- Vite frontend plus separate API

For a dashboard-oriented product, the recommended default is a Turborepo-style Next.js setup with:

```text
apps/
  admin/
packages/
  ui/
  db/
docs/
```

