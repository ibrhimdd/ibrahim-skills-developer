# Unslop — Agent Skill for UI Design Refinement

**Status:** Verified reference entry; not installed in this library or in any project.  
**Reviewed:** 2026-11-13

## Official source

- Repository: https://github.com/heydamir/unslop
- Skill instructions: https://github.com/heydamir/unslop/blob/main/skills/unslop/SKILL.md
- Author attribution: Damir Sokolovsky (@heydamir)
- License: CC BY 4.0

## What it is

Unslop is an Agent Skill for Claude Code, OpenAI Codex, and Google Antigravity. It helps turn generic or AI-looking interfaces into more intentional product-specific designs. It audits visual issues (for example, excessive gradients and glows, emoji labels, inconsistent spacing, generic copy, typography, and layout), proposes a visual direction, and then refines the interface in ordered passes.

It is a workflow/instruction skill, not a standalone component library, browser extension, CSS framework, or automatic design plugin.

## Workflow requirements

1. Inspect the actual screen and identify the files that render it.
2. Audit the screen and list concrete issues with their locations.
3. Decide whether it needs a full redesign, light polish, or only small refinements.
4. Present the audit and proposed visual direction, then wait for the user's approval before editing.
5. Apply the refinement passes in the order specified by the official skill.
6. Render and compare the result against the audit checklist.
7. Report what changed and any remaining issues.

Do not skip the approval checkpoint unless the user has already explicitly authorized immediate implementation.

## Compatibility

The official README names Next.js, React, Vue, Svelte, Tailwind, and plain HTML/CSS. It can also work from a live website URL.

For Ibrahim's PHP/XAMPP projects, use it as an agent-guided design review for the rendered HTML/CSS. Do not assume framework-specific scripts or commands will work unchanged in a PHP project. Inspect the skill's scripts and project prerequisites before running them.

## Installation

### Codex

```text
$skill-installer install https://github.com/heydamir/unslop/tree/main/skills/unslop
```

Manual user-wide installation:

```bash
git clone https://github.com/heydamir/unslop
mkdir -p ~/.agents/skills
cp -r unslop/skills/unslop ~/.agents/skills/
```

### Claude Code

```bash
git clone https://github.com/heydamir/unslop
mkdir -p ~/.claude/skills
cp -r unslop/skills/unslop ~/.claude/skills/
```

For a project-only installation, the README documents copying the skill folder into that project's `.claude/skills/` directory.

### Google Antigravity

The repository README documents copying the skill folder into `~/.gemini/antigravity/skills/`. Check the current README for project-local placement before installing.

## Optional tooling

For live-site snapshots or story-video generation, the README calls for Playwright and Chromium. Story videos additionally require ffmpeg. These are optional; do not install them unless the relevant workflow is requested.

## License and attribution

The source repository states CC BY 4.0. When reusing or adapting its material, retain attribution to **Damir Sokolovsky (@heydamir)** and a link to https://github.com/heydamir/unslop. This library records a summary and links to the original; it does not redistribute the complete upstream skill.

## Suggested use in Ibrahim's projects

- **edu-k:** Audit dashboard contrast, spacing, typography, cards, charts, navigation, and RTL consistency before making UI changes.
- **PHP/XAMPP applications:** Apply the design-review process to the rendered HTML/CSS while preserving PHP routes, database logic, authentication, and existing behavior.
- **New websites:** Use the audit and direction phase before implementing a visual redesign.

## First-use prompt

```text
Use the Unslop skill to review this screen. First inspect the project and identify the files that render the screen. Audit the concrete visual issues and classify the work as a full redesign, light polish, or small refinements. Propose a product-specific visual direction and wait for my approval before changing any files. Preserve all existing functionality and verify desktop, mobile, and RTL behavior.
```

## Source verification

- README: https://github.com/heydamir/unslop/blob/main/README.md
- SKILL.md: https://github.com/heydamir/unslop/blob/main/skills/unslop/SKILL.md
