# Choose the visual pipeline

| Request | First route | First artifact |
|---|---|---|
| Character, creature or prop with one visual identity | Agent Sprite Forge workflow | One master still at the expected viewing angle |
| Animation actions based on an approved master | Sprite/video workflow | One pilot action, registered to the master |
| Repeatable pixel-art effect such as a pickup, impact or cast | PixelFX workflow | Rendered contact sheet plus a short in-engine preview |
| Tiles, terrain or backdrop | Existing Hub map skill | Layer or tile contract; do not use the character pipeline |

## Sprite Forge

Read the Hub's `generate2dsprite`, `video2dsprite` or `generate2dmap` material under `skills/02-art-animation-ui-audio/` according to the task. Set facing, display dimensions, anchor, alpha, actions, frame timing and export target. Approve or verify the identity on the master before scaling to a full action set. Do not claim an approved master or successful generation without evidence. With no image/video integration authorized, use supplied frames or return the art brief and the exact missing capability. Record the master identity, frame bounds, pivot, palette if pixel, FPS, loop behavior and provenance in the handoff. Check outline/alpha at 1× and loop seam; engine collision state must not depend on art frame geometry.

## PixelFX

Read the existing Hub `pixelfx` skill for CLI syntax. Select one effect with a licensed source, render an isolated pilot if a reviewed pinned renderer is already present, inspect against light and dark backgrounds, and adjust palette, pivot and timing before integrating. Record effect ID, source revision, options/seed, frame size, FPS, loop state and license. When engine runtime import is unavailable, hand off a transparent strip/atlas and JSON rather than claiming that it plays in-engine. Preserve required license and attribution for reused upstream code/assets. Do not ship a third-party checkout, run unreviewed setup scripts, or publish to Patch or a store as part of this workflow.

## Worked example

[Blossom Blast in Arcade-x](https://github.com/ducpham2806/Arcade-x/blob/main/docs/qa/BLOSSOM-VIVID-EFFECTS-2026-11-26.md) uses a pinned PixelFX renderer, strict Forge frame checks and browser evidence for one game. Use it as a pattern, not as a requirement to copy effects or execute its build in other projects.
