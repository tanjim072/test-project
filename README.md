# Test Project

A Node.js application written in TypeScript, using Next.js with the App Router.

## Status

Early setup. Dependencies installed so far:

- `dotenv` for environment variables

Next.js and TypeScript are the intended stack and are not scaffolded yet. There is no `app/` directory and no `dev`, `build`, or `lint` scripts.

## Requirements

- Node.js (current LTS)
- npm

## Setup

```bash
npm install
```

Copy environment values into a local `.env` file when the app needs them. Do not commit `.env`.

## Scripts

| Command | What it does |
| --- | --- |
| `npm test` | Placeholder. No tests are configured yet. |

## Stack

- Runtime: Node.js
- Language: TypeScript (`strict`)
- Framework: Next.js (App Router)

## Conventions

- Use the App Router (`app/`), not the Pages Router.
- Prefer Server Components. Add `"use client"` only when a component needs browser APIs, state, or event handlers.
- Keep secrets and data access on the server. Do not import them into client components.
- Type props, API responses, and return values. Avoid `any`.
- Use `Link` for internal navigation and `next/image` for images.
- Validate external input on the server before using it.
