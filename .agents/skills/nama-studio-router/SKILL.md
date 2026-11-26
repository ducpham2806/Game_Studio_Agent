---
name: nama-studio-router
description: Route game work in Game Studio Agent Hub to the right engine, game-development role, repository evidence and QA gate. Use for game prototypes, gameplay features, architecture tracing with Graphify, sprite animation with Agent Sprite Forge, pixel VFX with PixelFX, or coordinating game subagents.
---

# Nam Á Game Studio Router

1. Find the actual game project and identify engine + version from its manifests. The Hub is a toolbox, not the game. If the target is not established and the work could modify files, ask before editing. Read applicable project instructions and only the Hub skills needed for the task.
2. Record the request as a handoff: target, engine, output, success checks, owned files, known risks. For a quick prototype keep one playable loop; defer optional systems.
3. For investigation, read [graph-and-evidence.md](references/graph-and-evidence.md). For sprites or effects, read [sprite-and-vfx.md](references/sprite-and-vfx.md).
4. Use the smallest set of roles needed. Coordinate with `studio_director`; hand read-only dependency tracing to `studio_graph_mapper`; send implementation to `studio_gameplay`; send character sheets to `studio_sprite_artist`; send coded effects to `studio_pixel_vfx`. Ask `studio_qa` to review independently after the artifacts are ready. If custom agents are unavailable, follow the same role boundaries serially. Keep overlapping writes serial and use separate directories for independent work.
5. Report which exact version/files were tested and where the evidence is. Use **PASS**, **NEEDS WORK**, or **NOT VERIFIED**; a missing engine, provider, dependency, or visual check is not a pass. Never merge, publish, install a dependency, enable background watchers, or send project files to a new external tool merely because a reference suggests it. Do not infer consent from an available API key.

The Hub's existing catalog lives under `skills/`. For standard routing and QA, consult `skills/00-orchestration-and-workflows/game-studio-orchestrator/SKILL.md` and `skills/00-orchestration-and-workflows/game-qa-playtest/SKILL.md`. Use the source versions recorded in [source-pins.md](references/source-pins.md) when comparing behavior, not to install anything implicitly.
