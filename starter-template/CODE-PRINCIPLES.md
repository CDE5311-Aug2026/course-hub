# Simple code principles

These rules make AI-generated code easier to understand, review and recover.

## Build small, readable pieces

- One component should have one clear job.
- Use names that explain purpose: `IdeaCard`, not `Box2`.
- Keep screen-specific code near the screen; move something to `components/` only when it is genuinely reused.
- Reuse design tokens and components instead of copying styles.

## Protect behaviour

- Change one thing at a time; keep each PR focused.
- Keep loading, empty and error states visible where relevant.
- Validate input and show useful feedback; do not hide failures.
- Preserve keyboard access, labels, focus and readable contrast.
- Use fake local data until real data is essential.

## Keep the project safe

- Do not add a dependency without naming the problem it solves.
- Do not put secrets in code, commits or screenshots; use `.env` files that stay ignored.
- Do not replace large files, rename broad folders or “refactor everything” without approval.
- Before a PR, run the app and check the changed flow at desktop and mobile widths.

## Codex check-out

At the end of each task, Codex must report:

1. What changed and which files changed.
2. How it follows `DESIGN.md` and these principles.
3. What was run or checked.
4. Any remaining risk or assumption.
