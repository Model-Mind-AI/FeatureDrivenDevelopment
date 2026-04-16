# Agent notes (FeatureDrivenDevelopment)

This repository is set up to grow **Cursor skills** and **toolkit plugins** (MCP servers, CLIs, hooks helpers) that speed up software development.

## Layout

| Path | Purpose |
|------|---------|
| `.cursor/skills/` | Project skills loaded by Cursor. Each skill is `skill-name/SKILL.md` plus optional assets. |
| `.cursor/skills/_template/` | Copy to create a new skill folder. |
| `.cursor/rules/` | Project rules (`.mdc`); see `ai-dev-toolkit.mdc` when editing skills or toolkit code. |
| `.cursor/hooks/` | Optional project hooks and scripts (pair with `hooks.json` when you add hooks). |
| `toolkit/plugins/` | Source for non-skill “plugins”: editors, CLIs, bundlers, etc. |
| `toolkit/plugins/fdd-factory/` | FDD Factory skill pack: inventory and reuse notes for `.cursor/skills/` (see `README.md`). |
| `toolkit/mcp/` | MCP server implementations or wrappers intended for Cursor MCP config. |

## Adding a new skill

1. Copy `.cursor/skills/_template/` to `.cursor/skills/<new-skill-name>/`.
2. Edit `SKILL.md`: set `name`, `description`, and body. Remove template placeholder text.
3. Add `reference.md`, `examples.md`, or `scripts/` only if the workflow needs them.

## Adding a plugin or MCP server

1. Create a subfolder under `toolkit/plugins/` or `toolkit/mcp/`.
2. Add a minimal README in that subfolder when the component has build or run steps.
3. Wire Cursor via project MCP settings or deployment docs as appropriate.
