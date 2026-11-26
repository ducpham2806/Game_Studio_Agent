# Game Studio Agent Hub

- This repository is the shared studio toolbox. Verify the actual game checkout and engine before editing or testing a game.
- Start game work with `$nama-studio-router`. Open only the playbooks in `skills/` required by the current task.
- Use the project-scoped Codex roles under `.codex/agents/`; see [Codex Studio](docs/CODEX-STUDIO.md). Keep role scopes and write sets separate. Review changes against real evidence when available.
- Do not run upstream installers, add dependencies, change permissions, connect external media providers, or publish merely because a playbook suggests it. Retain upstream license and provenance for any permitted reuse.
- Preserve existing Claude roles, scripts and skill catalog unless the user asks to change them.
