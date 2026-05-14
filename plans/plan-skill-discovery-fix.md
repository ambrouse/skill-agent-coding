# Plan: Skill Discovery Fix

Date: 2026-05-14

## Goal

Make all repository skills discoverable by Codex and prepare the repository for push according to the push workflow.

## Steps

1. Inspect current `.codex/skills` and `.github/skills` structure.
2. Identify why Codex does not recognize every skill.
3. Add top-level `.codex/skills/<skill>/SKILL.md` wrappers for each project rule.
4. Add missing `.github/skills/<skill>/SKILL.md` mirror files.
5. Add short user-invocable aliases for common slash commands.
6. Add basic setup and CI validation files.
7. Run local validation, review diff, commit, and push.

## Skills Used

- `skill-creator`
- `project-workflow`
- `push-code-skill`
- `readme-style`
- `documentation-skill`
- `logging-skill`
