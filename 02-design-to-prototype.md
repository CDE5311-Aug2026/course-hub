# From design to prototype

Your design comes first. Codex turns an agreed design into a runnable version; it should not invent a new product direction.

## Before the first prompt

1. Copy the templates into the team repo and complete `brief.md` and `DESIGN.md`.
2. Add links to the source design and a few key screenshots in `DESIGN.md`.
3. Tell Codex which framework already exists and how to run it.
4. Choose one important, self-contained screen: usually the first screen a user needs to complete the core task.

Do not begin with a dashboard just because it looks impressive. Begin with the shortest path that proves your idea works.

## Hand a screen to Codex

Give Codex the design link or screenshot, name the target route, and state the screen’s job. Ask it to read `DESIGN.md` and `brief.md` first, then propose a plan. Confirm the plan before it writes code.

Example: “Read DESIGN.md and brief.md. Study this screenshot. Plan the smallest implementation of the sign-up screen at /signup. Keep it static for now. It works when the page matches the layout at desktop and mobile widths.”

## Build in layers

1. **Static screen:** layout, typography, colour, images and placeholder content.
2. **Interactions:** navigation, validation, states, menus, drawers and feedback.
3. **Real data:** only then connect forms, APIs, accounts or saved content.

After each layer, run it and compare it with the source design. Check hierarchy first (layout and spacing), then components, then visual detail. Keep a screenshot beside the design; “looks right” is not a useful test.

If the build drifts, update `DESIGN.md`, show the reference again, and request a focused correction—not a total redesign.
