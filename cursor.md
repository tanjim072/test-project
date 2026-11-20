# Project

Node.js project built with TypeScript and Next.js (App Router).

## Stack

- Runtime: Node.js
- Language: TypeScript (`strict`)
- Framework: Next.js (App Router)
- Styling: keep it simple unless asked otherwise

## Conventions

- Use the App Router (`app/`), not the Pages Router.
- Prefer Server Components. Add `"use client"` only when the component needs browser APIs, state, or event handlers.
- Put server-only logic (data access, secrets) in Server Components, Route Handlers, or server modules. Do not import secrets into client components.
- Use TypeScript for all source files (`.ts` / `.tsx`). Avoid `any`; type props, API responses, and function returns.
- Use the Next.js `Link` component for internal navigation and `next/image` for images.
- Keep components small and colocate them near the route that uses them.
- Name files in kebab-case for routes and PascalCase for React components.
- Validate external input on the server before using it.

## Commands

```bash
npm install
npm run dev
npm run build
npm run lint
```

## When changing code

- Match existing patterns in the repo.
- Do not add dependencies unless they are needed for the task.
- After UI changes, verify the affected page in the browser.
