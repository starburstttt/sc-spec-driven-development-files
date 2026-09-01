# Tech Stack

## Language

TypeScript everywhere — server and client share one language, one set of
types, and one toolchain.

## Framework: Next.js (App Router)

Recommended framework: **Next.js**, using the App Router with React Server
Components.

Why:

- It's server-side TypeScript by default — pages render on the server, so
  the dashboard and booking flow work without shipping a heavy client-side
  app.
- It's one of the most widely used TypeScript web frameworks, satisfying
  Mary's ask for a "popular stack" without inventing custom plumbing.
- Routing, API endpoints, and server-rendered pages live in a single
  codebase — appropriate for a small team building a dashboard, a content
  catalog, and a booking flow.
- Good defaults for the modern-browser, attractive-site goals Steve cares
  about (fast rendering, easy to style, works well without legacy
  browser workarounds).

## Runtime

Node.js (LTS).

## Data storage

**SQLite.** A single file-based database — no separate database server to
run or configure, which keeps setup trivial for students and for
conference-booth demos while still being a real, persistent store.

## Styling

Not yet decided — pick a lightweight, modern approach when the visual
design phase of the roadmap starts.

## Tooling

- `tsc` for type-checking (already in `package.json`).
- Package manager: npm (already in use via `package-lock.json`).
