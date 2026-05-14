---
name: push-code-skill
description: Push and release preparation rules for this repository. Use when Codex prepares commits, checks CI/CD, validates tests, updates README/setup files, manages versioning, writes commit descriptions, or pushes code.
argument-hint: "push task"
user-invocable: true
---

# Push Code Skill

Follow the preserved push rules at `../project-workflow/references/github-skills/push-code-skill/push-code-skill.md`.

Before pushing, check repository status, review the diff, run the available validation for this repository, commit with a clear timestamped message, and push to the configured remote.

Use those rules together with active system and developer instructions. If instructions conflict, follow higher-priority instructions first.
