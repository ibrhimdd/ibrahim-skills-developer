---
name: web-motion-design
description: Plan and implement purposeful animations and transitions for interactive websites, including scroll effects, page reveals, micro-interactions, and responsive motion. Use when a user asks to animate a website or make its interface feel more dynamic.
---

# Web Motion Design

## Choose the right motion

1. Identify the user purpose and the element being animated. Motion should explain hierarchy, state, continuity, or feedback—not merely decorate.
2. Inspect the project's stack and existing animation dependencies before choosing an implementation.
3. For inspiration, consult the saved Scrolltide reference when live access is available; select a pattern that fits the page and adapt it rather than copying an entire template.
4. For timeline-heavy web animation, consider GSAP. For React component transitions, consider a React-compatible motion library only if the project already supports it or the user approves the dependency. Use CSS transitions/keyframes for simple effects.
5. Keep Blender and After Effects specialist skills for motion graphics and 3D production, not as implementation instructions for ordinary website interactions.

## Motion design principles

- Define trigger, start state, end state, duration, easing, and interruption behavior.
- Use consistent timing and easing across related components.
- Prefer short, subtle feedback for hover, focus, and button states.
- Use scroll-driven motion sparingly; never trap scrolling or make essential content inaccessible until an animation completes.
- Avoid animating layout-heavy properties when transform/opacity can achieve the same effect.
- Prevent cumulative layout shift and avoid blocking interaction during decorative sequences.
- Ensure animations remain understandable with touch input and on low-powered mobile devices.

## Accessibility and performance

- Respect `prefers-reduced-motion: reduce`; provide a calm or static alternative.
- Never communicate essential information only through animation.
- Keep focus visible and preserve keyboard interaction during transitions.
- Avoid unnecessary WebGL, large video backgrounds, and continuous animation loops.
- Check scroll performance, memory use, and mobile behavior.

## RTL and localization

- Check directional movement in RTL layouts. A reveal or slide should reinforce the reading direction rather than blindly reuse an LTR motion.
- Do not mirror motion automatically when its meaning is not directional.
- Ensure animated navigation, drawers, and dialogs open from the expected side.

## Verification

- Test the initial state, completed state, rapid repeated interactions, interrupted transitions, reduced-motion mode, keyboard access, and mobile viewport.
- Confirm that content remains available if JavaScript or the animation library fails.
- Report which implementation technique and dependencies were used. Do not claim a live Scrolltide/MCP connection unless one is actually configured.
