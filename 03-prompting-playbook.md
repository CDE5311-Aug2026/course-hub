# Prompting playbook

A useful prompt gives Codex one job and a way to prove it finished. Before asking for code, ask for a short plan when the task has more than one step.

## A reliable prompt shape

- **Context:** which files, route or screen matter?
- **Task:** one change only.
- **Reference:** a screenshot, design link, example or existing component.
- **Constraints:** reuse styles, do not change unrelated files, no new dependencies, etc.
- **Done when:** what you will run or observe to check it.
- **Risk check:** ask, “What could break, and how will you avoid it?”

## Before → after

| Vague prompt | Better prompt |
| --- | --- |
| Make it look nicer. | Read DESIGN.md. Tighten spacing and type scale on /home to match this screenshot. Do not change copy or behaviour. Done when desktop and mobile match the reference hierarchy. |
| Build the login. | Propose a plan for a static /login screen from this reference. After I approve, build it using existing components. Done when email, password, submit button and error state render. |
| Add a button. | Add the “Save idea” button to the idea card using the primary button style in DESIGN.md. On click, show the existing success toast. Done when the button works without changing card layout. |
| Fix the form. | The /contact form submits twice. Inspect the submit handler and explain the cause before changing code. Fix only that cause. Done when one click produces one request. |
| Make it responsive. | Compare /profile at 1440px, 768px and 375px. Plan the smallest responsive changes; keep the desktop layout intact. Done when no content overflows. |
| Add a database. | First list the data the prototype truly must remember and a no-database alternative. Recommend the smallest option before implementing anything. |
| Copy this Figma. | Read DESIGN.md and reproduce only the visible settings panel in this screenshot at /settings. Start static; use placeholders for data. Tell me what is ambiguous. |
| Add animation. | Add a 150–200ms ease-out transition to the existing drawer. Respect reduced-motion settings. Done when open and close feel smooth and keyboard focus still works. |
| Fix this error. | When I run `npm run dev`, I get this full error: [paste]. I changed [what changed]. Explain the likely cause, propose the smallest fix, and tell me how to verify it. |
| Refactor everything. | Identify the one repeated card pattern on /explore. Propose a small reusable component without changing output. Done when the screen looks identical and the app still runs. |

## Guardrails

Ask one task per prompt. Keep a reference nearby. Name constraints early. If Codex proposes a large change, pause and split it into smaller prompts. After every change, run the app yourself.
