# HyperFrames — heygen-com

- **Category:** Open-source HTML-to-video framework, CLI, desktop app, and Agent Skills
- **Repository:** https://github.com/heygen-com/hyperframes
- **Documentation:** https://hyperframes.heygen.com/introduction
- **Quick start:** https://hyperframes.heygen.com/quickstart
- **Core skill:** https://github.com/heygen-com/hyperframes/blob/main/skills/hyperframes/SKILL.md
- **Reviewed:** 2026-11-13

## Purpose
Turns HTML, CSS, media, and deterministic seekable animations into MP4 video. It includes a CLI, editable desktop/Studio workflow, a component and transition registry, and skills for coding agents.

## Best use
Product promos, explainers, kinetic typography, charts/maps, social clips, overlays, and reusable motion graphics.

## Requirements
The repository states Node.js 22+ and FFmpeg for CLI use.

## Rendering model
HyperFrames seeks a paused timeline frame by frame to make renders deterministic. Its skill requires timed elements to follow the framework's clip/timeline contract and disallows timers, live network fetches, unseeded randomness, and non-seekable animation behavior in the render timeline.

## Compatibility
This is a video-production runtime, not a normal interactive website animation library. It uses HTML/CSS/JS compositions to produce video output.

## License
Apache-2.0 for the repository.

## Adoption status
Saved as a reference; not installed or connected.
