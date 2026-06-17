# EDocx Frontend — Commit Guide

Backend commits are documented in [BACKEND_COMMITS.md](./BACKEND_COMMITS.md).

| # | Commit message | What it adds |
|---|----------------|--------------|
| 10 | `chore: initialize EDocx frontend scaffolding` | Vite + React 19, routing shell, public assets, EDocx favicon/title |
| 11 | `feat: add design tokens and global styles` | CSS tokens, animations, component styles, editor ProseMirror rules |
| 12 | `feat: add shared UI components and utilities` | `components/ui/*`, `cn`, `user` helpers |
| 13 | `feat: add API services and auth context` | axios client, auth/document services, `AuthContext` |
| 14 | `feat: add login page and protected routing` | `LoginPage`, backgrounds, `ProtectedRoute`, `App` routes |
| 15 | `feat: add dashboard with document list` | `DashboardPage`, cards, new-doc strip, templates |
| 16 | `feat: add TipTap editor with rich-text toolbar` | `EditorPage`, `DocumentEditor`, toolbar, image extensions |
| 17 | `feat: add sharing, import/export, and app polish` | `ShareModal`, import/export utils, nav drawer, avatar menu |
| 18 | `chore: add root monorepo workspace` | Root `package.json` for `npm run dev` from repo root |

## Run locally

```bash
# From repo root — one-time setup
npm run setup
cp backend/.env.example backend/.env   # add Supabase credentials

# Start API + frontend together
npm run dev
```

Or run separately: `npm run dev:api` and `npm run dev:web`.

App: http://localhost:5173 · API docs: http://localhost:8000/api/docs

## Branding notes

- Logo wordmark shows **EDocx** (E + Doc + x)
- Internal CSS classes use `gdocx-*` prefixes for the shared design system
- Use a dedicated Supabase project for EDocx
