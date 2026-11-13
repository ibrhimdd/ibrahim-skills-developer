# Scrolltide — UI/UX & Motion Design Reference

**Category:** Design Resource Library  
**Official site:** https://www.scrolltide.co/  
**Templates:** https://www.scrolltide.co/templates  
**MCP:** https://www.scrolltide.co/mcp  
**Reviewed:** 2026-11-13

## What it is

Scrolltide describes itself as a curated library of scroll-driven website templates and prompts, animated components, page sections, UI screens, 3D scenes, and shader backgrounds. It is a design/reference library, not a standalone website builder and not an Agent Skill by itself.

Its homepage currently lists 145 templates, 95 components, 55 shaders, 24 sections, and 14 UI screens. These counts can change.

## Why it belongs in this library

Use Scrolltide as a preferred source of inspiration when Ibrahim asks for:
- UI/UX motion design or animation.
- Scroll-triggered reveals, scroll-scrubbed sequences, and storytelling.
- Parallax depth and layered movement.
- Animated hero sections and page transitions.
- Hover, cursor-following, and micro-interactions.
- Animated cards, navigation, buttons, and interactive sections.
- 3D/WebGL scenes or shader-based backgrounds.

## Technology ecosystem

The official site highlights React, Vite, Next.js, Tailwind, Framer Motion, GSAP, Three.js, WebGL, shaders, and Lenis.

## Working method for Ibrahim's projects

1. Inspect the current project and identify its real stack, layout direction, design system, and performance constraints.
2. Search Scrolltide for a relevant reference based on the page and desired interaction.
3. Extract the interaction idea and motion behavior; do not blindly copy a whole template.
4. Adapt it to the project's existing stack and visual identity.
5. For PHP/XAMPP projects, translate React/Next.js examples into compatible HTML, CSS, and JavaScript unless the project already uses React.
6. Keep motion purposeful and polished, not decorative noise.
7. Respect RTL layout, mobile touch behavior, keyboard accessibility, and `prefers-reduced-motion`.
8. Avoid expensive 3D/WebGL effects on mobile or low-powered devices unless they provide clear value.
9. Test scroll performance, responsive behavior, and the complete interaction after implementation.

## MCP integration

- **Endpoint:** `https://www.scrolltide.co/api/mcp`
- Official MCP instructions list Claude, Cursor, Codex, and VS Code support.
- Authentication is completed through a browser approval flow; the official page says no API key is required.
- MCP is read-only and can search/fetch library items; it cannot change account, plan, or billing.
- Fair-use limit stated by the official page: up to 40 different items per account in any 24-hour period.
- Access is limited to Yearly and Lifetime plans. If the plan expires, MCP access stops.
- This repository entry does not mean MCP has been configured or connected to ChatGPT.

Official setup instructions: https://www.scrolltide.co/mcp

## Plans and licensing notes

The official pricing page describes Monthly, Yearly, and Lifetime plans. MCP and the 3D collection are listed for Yearly and Lifetime tiers. Prices and plan details can change; check the live page before purchase: https://www.scrolltide.co/pricing

The official Terms state that websites created from the templates can be used, deployed, and monetized for personal or client work. However, the original templates/prompts and marketing assets may not be redistributed or resold as standalone products or used to create a competing template/prompt library. Read the current Terms before commercial use: https://www.scrolltide.co/terms

## Adoption status

Saved as a preferred UI/UX and motion-design reference. Not purchased, installed, or connected in this ChatGPT session.

## Source links

- https://www.scrolltide.co/
- https://www.scrolltide.co/templates
- https://www.scrolltide.co/mcp
- https://www.scrolltide.co/pricing
- https://www.scrolltide.co/terms
