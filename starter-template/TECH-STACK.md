# Technology choices

## Default choice

| Area | Use | Why |
| --- | --- | --- |
| UI | React | clear component model for screens and reusable UI |
| Language | TypeScript | catches common mistakes before the browser does |
| Dev/build | Vite | quick local development and a simple production build |
| Package manager | npm | familiar, included with Node |
| Styling | CSS variables + CSS files | design tokens stay visible and easy to inspect |
| Data first | local TypeScript/JSON data | prove the interface before adding services |

Vite provides React and React + TypeScript starter templates, a fast development server, and a production build. genui{"citation":{"refs":["turn0search0","turn0search1"]}}

## Add complexity only when needed

- Need saved, individual data? Add authentication and a small backend after the static flows work.
- Need shared, real-time data? Agree the data model and privacy requirements before choosing a service.
- Need no saved data? Keep it frontend-only.

## Do not mix stacks

For this course, do not introduce a second frontend framework, a component library, a database, or an API merely because Codex suggests it. First ask: “What specific prototype requirement does this solve?”

## Starting commands

```bash
npm create vite@latest my-prototype -- --template react-ts
cd my-prototype
npm install
npm run dev
```
