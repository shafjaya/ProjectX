# ProjectX

## What is this
A personal project built with Claude Code.

## How we work
- Files in `docs/` are the project's memory:
  - `readme.md` = what is this
  - `changelog.md` = what's been built
  - `ideas.md` = what's next
  - `decisions.md` = non-obvious choices and why
- At the end of every session: update `docs/`, commit, push.
- One change per prompt. Don't stack features.

## Tech
Plain HTML/CSS/JS — no frameworks, no build step.

## Always
- Before starting work, read `docs/changelog.md` to know current state.
- When making non-obvious choices, append it to `docs/decisions.md` with the reasoning.
- When done, update `docs/`, commit, push.
