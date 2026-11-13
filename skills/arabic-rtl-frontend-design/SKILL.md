---
name: arabic-rtl-frontend-design
description: Design or redesign polished, responsive Arabic-first web interfaces with correct RTL behavior, strong contrast, clear hierarchy, and accessible interactions. Use for dashboards, educational platforms, landing pages, forms, and component-level visual improvements.
---

# Arabic RTL Frontend Design

## Design process

1. Identify the product, audience, primary task, existing brand, framework, and constraints before choosing a visual direction.
2. Inspect the current pages and shared styles. Reuse established tokens and components where they are sound; do not create a second competing design system.
3. Define a compact visual direction: palette, typography, spacing scale, surfaces, borders, shadows, icon style, and interaction principles.
4. Design the information hierarchy around the user's primary task, not decoration.
5. Implement one representative page or component first, then extend the approved system consistently.
6. Review at mobile and desktop widths and refine based on actual rendered output when browser tools are available.

## Arabic and RTL requirements

- Set document language and direction correctly: Arabic content should normally use `lang="ar"` and `dir="rtl"`.
- Choose a legible Arabic typeface appropriate to the existing brand (for example Cairo or Tajawal only when suitable and available).
- Check alignment, navigation order, breadcrumbs, icons, form labels, tables, pagination, drawers, and modal placement in RTL.
- Use `dir="ltr"` or CSS direction isolation for URLs, email addresses, code, serial numbers, and Latin identifiers when needed.
- Avoid mechanically mirroring icons whose meaning is not directional.
- Ensure focus order follows the visual and reading order.

## Visual quality

- Establish strong text/background contrast. Test muted text, placeholders, disabled states, badges, chart labels, and overlays—not only body copy.
- Use a restrained, intentional palette with semantic colors for success, warning, danger, and information.
- Build hierarchy through type scale, whitespace, grouping, and consistent component patterns.
- Prefer meaningful whitespace and a clear grid over excessive cards, gradients, borders, or shadows.
- Use realistic Arabic interface copy and useful empty/loading/error states.
- Make data-heavy dashboards scannable; label chart axes and values and provide a text alternative for important findings.
- Avoid generic AI-looking layouts, arbitrary decorative elements, and motion that distracts from the task.

## Accessibility and responsive behavior

- Use semantic HTML and correctly associated form labels.
- Provide visible keyboard focus, sufficient target sizes, keyboard-operable controls, and accessible names for icon-only buttons.
- Do not use color as the only status signal.
- Respect `prefers-reduced-motion`.
- Test narrow mobile screens, zoom, long Arabic labels, and mixed Arabic/English text.

## Implementation constraints

- Inspect the actual stack before selecting libraries. Do not introduce React, Tailwind, Bootstrap, or an icon package unless the project uses it or the user approves adding it.
- Keep styles scoped and avoid destructive global overrides.
- Preserve working functionality, route names, form field names, and backend contracts while improving appearance.
- Verify the rendered result rather than relying only on source-code inspection.

## Completion report

List the design decisions, changed files, responsive/accessibility checks performed, and any remaining visual issues.
