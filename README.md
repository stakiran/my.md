# my.md
Add `.claude/rules/my.md` to `.gitignore`.

## Why my.md?

Claude Code officially provides `CLAUDE.local.md` for personal project overrides (gitignored, auto-loaded). But **my.md is a better convention**.

### The name says it all

- `my.md` — instantly clear that this is *your* personal file. No ambiguity.
- `CLAUDE.local.md` — what does "local" mean? Local machine? Local branch? You have to *know* the convention to understand it.

### Right-sized for what you actually write

Your personal rules are usually short — things like "reply in Japanese" or "use this commit format." A root-level `CLAUDE.local.md` feels like overkill for a few one-liners. A small file in `rules/` matches the actual granularity of what you're writing.

### Clean separation

With `my.md` in `.claude/rules/`, your personal rules live alongside other rule files — `team-conventions.md`, `code-style.md`, and `my.md`. The structure tells the story at a glance: team rules + your rules, all in one place with consistent granularity.

### No workaround needed

Some suggest using `@import` in `CLAUDE.md` to include a personal file (e.g., `@~/.claude/my-preferences.md`) as an alternative to `CLAUDE.local.md`. But this has a fundamental problem: where do you write the `@import` line? If you add it to the shared `CLAUDE.md`, it gets committed. If you add it to `CLAUDE.local.md`, you might as well write your rules there directly.

With `my.md`, there's nothing to wire up. Files in `.claude/rules/` are auto-loaded — no import lines, no indirection, and no worktree issues since rules are picked up from every worktree automatically.

### Easy to adopt

Just two steps for any project:

1. Add `.claude/rules/my.md` to `.gitignore`
2. Write your personal rules in `.claude/rules/my.md`

That's it. Your rules are automatically loaded by Claude Code, kept out of version control, and unmistakably yours.

## Setup

Clone this repo (or just copy the `.gitignore`) and start writing your own `my.md`.
