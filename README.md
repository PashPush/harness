Custom harness for different tasks.

## Files

| File | Purpose |
| --- | --- |
| [CLAUDE.md](CLAUDE.md) | Project rules: code style (minimal code, no new deps, "why"-only comments, CSS Modules, i18next) and workflow (plan before editing, surgical edits, no tests until approved). |
| [.claude/commands/plan.md](.claude/commands/plan.md) | `/plan` — planning mode: investigate, list affected files and a 2–5 point plan, no code until approved. |
| [.claude/commands/finalize.md](.claude/commands/finalize.md) | `/finalize` — clean up the approved diff (remove leftovers, trim comments), run typecheck/lint, show final diff and summary. |
| [.claude/commands/tests.md](.claude/commands/tests.md) | `/tests` — after `/finalize`: agree on test cases, write them in the project's style, run to green. |

Order of work: `/plan` → implement → `/finalize` → `/tests`.
