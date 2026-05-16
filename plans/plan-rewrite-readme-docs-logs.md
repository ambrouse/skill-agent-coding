# Plan: Rewrite README, Docs, Logs

Date: 2026-05-17
Scope: `skill-agent-coding` repository documentation cleanup and review-ready README rewrite.

## Goal

- Rewrite `README.md` so it matches the current repository structure.
- Add minimal but useful task documentation under `docs/`.
- Add a concise task log under `logs/`.
- Keep content truthful: no overclaiming about generated docs/logs/plans as permanent product features beyond this task.

## Required Skills

- `readme-style`: README layout, hero, navigation, repo map, docs index, accuracy notes.
- `plan-skill`: phase-based workflow and required plan file.
- `documentation-skill`: docs storage in `docs/`, dated, concise, cleaned.
- `logging-skill`: task logs in `logs/`, dated and concise.
- `testing-skill`: manual verification of documentation structure and commands, if available as raw skill.
- `push-code-skill`: only if user later asks to commit/push.

## Phase 1: Inspect Current State

Estimated time: 5 minutes.

Steps:
- Read current `README.md`.
- Check whether `docs/`, `logs/`, and `plans/` exist.
- Compare README claims against current repo structure.

Testing:
- Verify README mentions only existing top-level skill directories and raw review folders.

Documentation:
- Record task summary in `docs/task/rewrite-readme-docs-logs.md` after changes.

Logging:
- Record key actions in `logs/documentation/rewrite-readme-docs-logs.md`.

## Phase 2: Rewrite README

Estimated time: 15 minutes.

Steps:
- Add centered hero/title and badges using GitHub Markdown.
- Add quick navigation.
- Explain repository purpose and supported skill roots.
- Add Mermaid flow for authoring/review/sync workflow.
- Add skill matrix based on current files.
- Add quick start validation command.
- Add repository map including `.claude`, `.codex`, `.github`, `raw-skills`, `docs`, `logs`, and `plans`.
- Add docs index and accuracy notes.

Testing:
- Ensure README does not mention deleted `project-workflow` as an active skill.
- Ensure paths match actual repo layout.

## Phase 3: Add Docs And Logs

Estimated time: 10 minutes.

Steps:
- Create dated task documentation summary in `docs/task/`.
- Create dated task log in `logs/documentation/`.
- Keep both concise and focused on review context.

Testing:
- Verify files exist and contain date/scope/result sections.

## Phase 4: Final Verification

Estimated time: 5 minutes.

Steps:
- Run repository skill validation command if possible.
- Check git status.
- Report changed files and note that no commit/push is done unless requested.

Testing:
- PowerShell validation for `SKILL.md` metadata in `.claude`, `.codex`, and `.github` if command is compatible.
