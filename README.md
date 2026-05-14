# Skill Agent Coding

Minimal skill source for project workflow rules. The repository keeps matching Codex and GitHub skill entrypoints so the same rules can be used from both environments.

## Skills

| Skill | Purpose |
| --- | --- |
| `project-workflow` | Coordinator for selecting the right project skill. |
| `backend-skill` | Backend coding, structure, testing, security, and cleanup rules. |
| `frontend-skill` | Frontend coding, UI, accessibility, SEO, and performance rules. |
| `plan-skill` | Project planning and phased task workflow rules. |
| `documentation-skill` | Documentation storage, cleanup, and summary rules. |
| `logging-skill` | Work-session logging rules. |
| `push-code-skill` | Push, CI/CD, setup, commit, README, and versioning rules. |
| `readme-style` | README structure and style rules. |

Use the full skill names above.

## Repository Layout

```text
.codex/
  skills/
    <skill-name>/
      SKILL.md
.github/
  skills/
    <skill-name>/
      SKILL.md
  workflows/
    validate-skills.yml
```

Each `SKILL.md` contains the rule body directly. The `.github/skills` tree mirrors the full skill names from `.codex/skills`. There are no short alias skill directories, generated task docs, task logs, or task plans in this source tree.

## Validate

```powershell
$ErrorActionPreference = "Stop"
foreach ($root in @(".codex/skills", ".github/skills")) {
  Get-ChildItem $root -Directory | ForEach-Object {
    $skillFile = Join-Path $_.FullName "SKILL.md"
    if (!(Test-Path $skillFile)) { throw "Missing SKILL.md in $($_.FullName)" }
    if (!(Select-String -Path $skillFile -Pattern "^name:\s*.+" -Quiet)) { throw "Missing name in $skillFile" }
    if (!(Select-String -Path $skillFile -Pattern "^description:\s*.+" -Quiet)) { throw "Missing description in $skillFile" }
    if (!(Select-String -Path $skillFile -Pattern "^user-invocable:\s*true\s*$" -Quiet)) { throw "Missing user-invocable true in $skillFile" }
  }
}
```
