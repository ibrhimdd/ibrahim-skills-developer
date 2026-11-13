---
name: video-production-workflow
description: Plan and produce product videos, explainers, motion graphics, and promotional clips by choosing an appropriate HTML, React, or professional motion workflow. Use when a user asks to turn a website, app, feature, or concept into a video.
---

# Video Production Workflow

## Select the production route

1. Clarify the deliverable: target platform, aspect ratio, duration, language, audience, source assets, and whether the user needs an editable project or only a rendered video.
2. Inspect available operating system, runtime, editing software, browser, and rendering dependencies before choosing a tool.
3. Select the workflow based on the source and required output:
   - **Video Shotcraft:** use as a cinematic shot-planning and product-video production reference, especially when capturing an existing website/app.
   - **Remotion:** use for programmatic, React-based video compositions and data-driven timelines.
   - **HyperFrames:** use for deterministic HTML/CSS/JavaScript compositions rendered to video.
   - **After Effects / Blender motion skills:** use for professional motion graphics, compositing, and 3D scenes.
4. Read the chosen tool's current official installation, rendering, and licensing instructions before setup.

## Production workflow

- Define the creative direction and one clear message for the video.
- Map product benefits or story beats to shots; avoid showing features without explaining their value.
- Create a storyboard with shot purpose, framing, movement, duration, text, and transition.
- Use real product captures or supplied assets when fidelity matters. Do not fabricate product UI and present it as a real screenshot.
- Design typography, pacing, transitions, sound effects, and music as one coherent system.
- Keep captions readable, safe areas clear, and visual contrast strong.
- For Arabic video, proofread Arabic copy and check RTL composition, font shaping, and mixed-direction text.

## Technical and licensing checks

- Check Node.js, browser, FFmpeg, GPU, and application requirements against the actual machine. Do not assume current tools run on legacy operating systems.
- Remotion and HyperFrames are separate production environments; do not treat them as interchangeable website animation libraries.
- For deterministic rendering, ensure every frame can be reproduced at a requested timestamp; avoid timers, live network dependencies, and unseeded randomness where the renderer requires deterministic output.
- Verify source assets, fonts, music, footage, templates, and generated media licenses before commercial use.
- Do not claim an export completed unless a rendered file exists and was checked.

## Quality control

- Watch the complete render, not only a preview frame.
- Check spelling, timing, audio levels, clipping, transitions, aspect ratio, frame rate, and platform-safe margins.
- Verify that the exported file opens and plays.
- Deliver the rendered output and, when requested, the editable project/source files. State any missing assets or checks clearly.
