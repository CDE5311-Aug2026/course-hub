# Vibe coding basics

Vibe coding means directing an AI coding partner in small, checkable steps. You are still the product designer and editor: you decide what matters, test what it made, and keep the version that works.

## The app in design language

| Part | What it does | Design analogy |
| --- | --- | --- |
| Frontend | The screens people see and use | Your frames, components and interactions |
| Backend | The rules behind the screens | The invisible logic in your prototype notes |
| Database | Information the app remembers | A structured content library |
| Deployment | Putting the app on a shareable URL | Publishing a prototype for others to try |

A usable prototype can start with just a frontend. Add the backend and database only when real behaviour or saved information is the point.

## What AI is good at

- Building a known screen or component from a clear reference.
- Explaining unfamiliar code and suggesting small changes.
- Generating repeated UI, placeholder content and simple interactions.
- Finding likely causes of a pasted error.

## What AI is bad at

- Guessing your product priorities or visual system.
- Making good trade-offs from a vague request.
- Knowing whether the result actually matches your design.
- Keeping context forever: it needs your design rules and reminders.

## The core loop

1. Make one small request.
2. Run the app.
3. Check the exact thing you asked for.
4. Save the working version: commit it or open a pull request.

Use plain language, but be precise about the screen, action and success check. Change one thing at a time. If you cannot explain what changed, do not move on yet.
