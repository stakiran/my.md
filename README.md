# my.md
Add `.claude/rules/my.md` to `.gitignore`.

## Why my.md?

Claude Code officially provides `CLAUDE.local.md` for personal project overrides (gitignored, auto-loaded). But **my.md is a better convention**.

### The name says it all

- `my.md` — instantly clear that this is *your* personal file. No ambiguity.
- `CLAUDE.local.md` — what does "local" mean? Local machine? Local branch? You have to *know* the convention to understand it.

### Clean separation

With `my.md` in `.claude/rules/`, your personal rules live alongside other rule files — neatly organized and clearly scoped. There's no risk of confusing your personal config with the project-level `CLAUDE.md` that the whole team shares.

### Easy to adopt

Just two steps for any project:

1. Add `.claude/rules/my.md` to `.gitignore`
2. Write your personal rules in `.claude/rules/my.md`

That's it. Your rules are automatically loaded by Claude Code, kept out of version control, and unmistakably yours.

## Setup

Clone this repo (or just copy the `.gitignore`) and start writing your own `my.md`.
