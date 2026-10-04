---
name: prototype-debug
description: Diagnose and recover frontend prototype problems. Use when a student has a terminal, build, browser, layout, state, form, navigation, or interaction error while building a prototype.
---

# Prototype debugging

## Collect evidence

Ask for the exact error, where it appears, the command or action that caused it, the expected result, and what changed immediately before it. Read the relevant files before suggesting a fix.

## Diagnose before editing

State the likely cause and the smallest safe repair. If the cause is uncertain, explain the quickest check that distinguishes the likely causes. Do not change unrelated code or add a dependency to hide an error.

## Repair loop

1. Reproduce the problem once.
2. Make one small repair.
3. Run the relevant command and test the affected flow.
4. Check desktop and mobile layout when UI changed.
5. Report what changed, how it was checked, and any remaining risk.

## Recover safely

If a recent change caused multiple breaks or two repairs worsened it, identify the smallest saved version or commit to return to. Preserve working changes and restart with a narrower prompt. Never expose or commit secrets, tokens, or private user data.
