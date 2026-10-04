# Prompt examples by task

Use these after the core playbook. Replace text in square brackets and attach a screenshot or Figma link where useful. Ask for a plan first whenever the job has several steps.

## Turn a Figma screen into a build

> Read `brief.md`, `DESIGN.md` and `AGENTS.md`. Study [Figma link or attached screenshots] for [screen name]. First list the layout, components, visible states and ambiguous details. Propose the smallest plan. After approval, build the static screen at [route]. Do not add data or behaviour yet. Done when it matches [desktop/mobile reference].

## Create design rules from Figma

> I have a Figma design but no coded design system. Read `templates/DESIGN.md`. From these [link/screenshots], extract only the reusable decisions: colour roles, typography, spacing scale, radius, button styles, card styles, form states and tone of voice. Show them as a proposed completed `DESIGN.md`; label any guess as “needs confirmation”. Do not write app code yet.

## Turn design rules into code tokens

> Read `DESIGN.md` and inspect the project’s styling approach. Propose the smallest set of reusable design tokens for the approved colours, type, spacing and radii. Explain where they will live and what existing files they affect. After approval, add them without changing visible screens. Done when an existing component can use the tokens.

## Reproduce one component

> From this reference, build only the [button/card/input] component. Reuse the design tokens and existing conventions. Include [normal, hover/focus, disabled] states. Do not change a full screen. Done when the component renders in all named states.

## Check visual drift

> Compare [route] with [reference]. List the five most important differences in hierarchy, spacing, type and components. Propose the smallest corrections in priority order; do not change the design system unless the reference proves it is wrong.

## Make an interaction usable

> Add [specific interaction] to [route]. Describe the happy path, loading, empty and error states first. Keep the visual design unchanged. Done when [user action] produces [observable outcome], and keyboard focus remains usable.

## Use temporary data safely

> Populate [screen] with realistic placeholder data so we can test layout and states. Keep the data local and clearly fake; do not add a database, authentication or external service. Done when normal, empty and long-content cases are visible.

## Prepare a clean PR

> Review my changes for this one task: [task]. Check that they follow `DESIGN.md`, do not include secrets or unrelated changes, and still run. Give me a concise PR title, summary, visual test steps and any risks. Do not modify code.

## Recover after a bad attempt

> The previous change drifted from the design. Inspect the diff and identify the smallest safe point to revert or correct. Preserve working parts. Propose a recovery plan before editing; the target is [specific screen and reference].
