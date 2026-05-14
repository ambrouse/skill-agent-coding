# Skill Discovery Fix Log

Date: 2026-05-14

## Work Completed

- Inspected current `.codex/skills` and `.github/skills` layouts.
- Found that most project rules were nested under `project-workflow/references` instead of being top-level Codex skills.
- Added discoverable top-level Codex skill wrappers.
- Added short alias skills after confirming slash commands need user-invocable skill entrypoints.
- Added missing GitHub mirror `SKILL.md` files.
- Added README/setup/CI files required by the push workflow.

## Validation

- Official `skill-creator` validator could not run because the local Python environment is missing `yaml`.
- Ran a PowerShell validation pass for `SKILL.md`, frontmatter delimiters, `name`, and `description`.
