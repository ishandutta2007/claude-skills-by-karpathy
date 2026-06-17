# Using this repo with Cursor

This project includes a **Cursor project rule** so the Karpathy-inspired **Claude Skills** apply automatically when you work here.

## In this repository

1. Open the folder in Cursor.
2. The rule [**../.cursor/rules/claude-skills-karpathy.mdc**](../.cursor/rules/claude-skills-karpathy.mdc) is committed with `alwaysApply: true`, so you do not need extra installation steps.
3. In Cursor, you can confirm it under **Settings → Rules** (or the project rules UI), where `claude-skills-karpathy` should appear.

## Use the same guidelines in another project

**Cursor (recommended):** Copy `.cursor/rules/claude-skills-karpathy.mdc` into that project’s `.cursor/rules/` directory (create the folders if needed). Adjust or merge with existing rules as you like.

**Other tools:** If a stack only supports a root instruction file, copy [**../CLAUDE.md**](../CLAUDE.md) into that project instead (or merge its contents into your existing instructions).

## Optional: personal Agent Skills

If you want the same content as reusable skills under `~/.cursor/skills`, use the specialized files in [**../claude-skills/**](../claude-skills/). You can copy or symlink them into your personal skills directory:

- [Think Before Coding](../claude-skills/think-before-coding/SKILL.md)
- [Simplicity First](../claude-skills/simplicity-first/SKILL.md)
- [Surgical Changes](../claude-skills/surgical-changes/SKILL.md)
- [Goal-Driven Execution](../claude-skills/goal-driven-execution/SKILL.md)

## Claude Code vs Cursor

- **Claude Code:** Install via the plugin marketplace and [**../README.md**](../README.md) instructions; the plugin exposes the **Claude Skills** from this repo. Per-project use can also rely on `CLAUDE.md`.
- **Cursor:** Use the committed `.cursor/rules/` file as described above. Cursor does not read `.claude-plugin/` or `CLAUDE.md` by default.

## For contributors

When you change the principles, keep [**../CLAUDE.md**](../CLAUDE.md) and [**../.cursor/rules/claude-skills-karpathy.mdc**](../.cursor/rules/claude-skills-karpathy.mdc) in sync. If the published skill/plugin text should match, update the respective files in [**../claude-skills/**](../claude-skills/) as well.
