# Team prototype starter

Copy this folder into a new team repository, then rename or move its files to the repository root. Complete the three planning files before building screens.

> **Do not begin building a screen until the team has completed and agreed `DESIGN.md` and `brief.md`.** A small, shared design system is the minimum input for consistent AI-built screens.

## Recommended default stack

Use **React + TypeScript + Vite**, with npm and plain CSS/CSS variables. This gives teams components, useful error checking, a quick local dev loop, and few moving parts. Use local mock data first; add a backend or database only when the prototype needs saved, shared or real information.

## Suggested repository layout

```text
team-prototype/
├── .codex/skills/       # reusable Codex workflow instructions
├── src/
│   ├── components/      # reusable UI
│   ├── pages/           # one file per screen/route
│   ├── data/            # temporary local data
│   └── styles/          # tokens and global styles
├── public/              # images and static files
├── references/          # key screen exports and design notes
├── DESIGN.md
├── AGENTS.md
├── CODE-PRINCIPLES.md
├── TECH-STACK.md
└── brief.md
```

## Setup order

1. Complete `brief.md`.
2. Add Figma links and key exports to `references/`; complete `DESIGN.md`.
3. Read and keep `TECH-STACK.md` and `CODE-PRINCIPLES.md`.
4. Create the app, run it, then ask Codex to read the project files before planning one screen.
