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

Vite provides React and React + TypeScript starter templates, a fast development server, and a production build. See the official [Vite Getting Started guide](https://vite.dev/guide/).

## Install once per computer

Students need:

1. A current **Node.js LTS** installation; it includes `npm`.
2. **Git** for cloning, branches and pull requests.
3. A code editor and a modern browser.

Check Node is available with `node --version` and `npm --version`. In a cloud development environment, these may already be installed.

Do **not** install React, TypeScript or Vite globally. Create the project once, then run `npm install` inside its folder. That command reads `package.json` and downloads exactly the libraries the project declares.

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
