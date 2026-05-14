# Skill Discovery Fix

Date: 2026-05-14

## Summary

Codex only had one top-level skill in `.codex/skills`: `project-workflow`. The remaining rules were stored under `project-workflow/references/github-skills`, which makes them useful as references but not discoverable as separate skills.

## Changes

- Added top-level Codex skills for backend, frontend, planning, documentation, logging, push, and README style.
- Added short slash aliases for `/backend`, `/push`, `/frontend`, `/plan`, `/docs`, `/log`, and `/readme`.
- Added `user-invocable: true` to generated skill entrypoints so tools can expose slash commands.
- Kept `project-workflow` as the coordinating skill.
- Added missing `SKILL.md` files for GitHub skill mirror directories.
- Added a CI workflow that validates every skill directory has `SKILL.md`, YAML frontmatter, `name`, and `description`.

## Verification

- Checked `.codex/skills` now exposes all project skills as top-level directories.
- Checked `.github/skills` now has `SKILL.md` in every skill directory.
- Ran local PowerShell validation for Codex skill frontmatter.
