# Debugging and recovery

An error is evidence, not a dead end. Give Codex the evidence in a small, complete packet.

## What to send

- The exact error text (copy it; do not paraphrase).
- Where it appears: browser, terminal or build service.
- What you just changed.
- The command you ran and what you expected.
- The relevant file or screenshot, if the error points to one.

Ask: “Explain the likely cause, propose the smallest safe fix, and tell me how to verify it. Do not change unrelated files.”

## Recover in order

1. Re-run once to confirm the error is repeatable.
2. Read the first useful error, not every warning.
3. Ask Codex for an explanation and a small plan.
4. Apply one fix; run again.
5. Save the working state.

## When to revert

Return to a saved version when a change breaks several things, you no longer know what changed, or two repair attempts made the problem worse. Revert the smallest recent change that caused the break; then restart from that stable point with a better prompt and clearer success check.

## When to restart the request

Restart when the original task was too broad or the design reference was missing. Say what you learned: “The last approach altered three screens. Now change only the header on /home; preserve existing navigation.” A clean request is usually faster than a long repair conversation.

Never paste passwords, API keys, private student data or deployment secrets into a prompt or repository.
