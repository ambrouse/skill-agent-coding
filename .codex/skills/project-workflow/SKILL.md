---
name: project-workflow
description: Project workflow rules for this repository. Use when Codex works on this repo and needs to coordinate backend, frontend, documentation, logging, planning, README, and push rules.
argument-hint: "project task"
user-invocable: true
---

# Project Workflow

Use this skill when working in this repository.

## Discoverable Skills

Individual project skills are exposed as top-level Codex skills under `.codex/skills/`:

- `backend-skill`
- `backend`
- `frontend-skill`
- `frontend`
- `plan-skill`
- `plan`
- `documentation-skill`
- `docs`
- `logging-skill`
- `log`
- `push-code-skill`
- `push`
- `readme-style`
- `readme`

## Source Rules

The original rule files are preserved unchanged in this skill under `references/github-skills/`.
Read only the files relevant to the current task:

- Backend work: `references/github-skills/backend-skill/SKILL.md`
- Frontend work: `references/github-skills/frontend-skill/SKILL.md`
- Planning work: `references/github-skills/plan-skill/SKILL.md`
- Documentation work: `references/github-skills/documentation-skill/documentation-skill.md`
- Logging work: `references/github-skills/logging-skill/logging-skill.md`
- Push/release work: `references/github-skills/push-code-skill/push-code-skill.md`
- README style work: `references/github-skills/readme-style/readme-style.md`

## Usage

1. Identify the task type.
2. Read the matching source rule file from `references/github-skills/`.
3. Follow the preserved rules together with the active system and developer instructions.
4. If rules conflict, follow higher-priority instructions first, then the preserved project rules.
