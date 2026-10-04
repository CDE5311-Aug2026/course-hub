# Project instructions for Codex

## Non-negotiable start condition

Before planning or building a screen, read `brief.md`, `DESIGN.md`, `TECH-STACK.md` and `CODE-PRINCIPLES.md`.

Do not begin screen implementation until `DESIGN.md` is marked complete by the team. If information is missing or unclear, list the questions and wait for answers.

## Working method

1. Inspect relevant existing code.
2. Propose a short plan before writing code.
3. Work on one focused task only.
4. State what could break and how the result will be checked.
5. Run the app after each change and report the result.

## Course skills

Use the relevant repository skill in `.codex/skills/`:

- `@prototype-architect` — turn an approved brief and design into a small build plan; do not code.
- `@clarify-brief` — expose missing product or design decisions before planning.
- `@prototype-debug` — diagnose terminal, browser, build, layout or interaction problems.
- `@grill-my-prototype` — challenge assumptions and scope before more work is built.

If the environment does not automatically recognise repository skills, read the matching `SKILL.md` file before working.

## Boundaries

- Follow the agreed design system and technology choices.
- Reuse components; avoid unrelated refactors and new dependencies.
- Never commit secrets, tokens, passwords or private user data.
- Never alter deployment, access or billing settings without explicit approval.

## Commands

- Install: [e.g. npm install]
- Run: [e.g. npm run dev]
- Check: [e.g. test changed screen at local URL]
- Test: [e.g. npm run lint && npm run build]
