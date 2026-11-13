# Prime Skills Developer
## Ibrahim's Personal Skills Library

> A growing, verified reference library of skills, tools, workflows, and quality standards for designing, building, improving, and testing websites and web applications.

**Owner:** Ibrahim  
**Repository:** `ibrahim-skills-developer`  
**Primary language:** Arabic documentation, with original technical names and commands preserved.

---

## Mission

This repository is the central reference for the skills used across Ibrahim's web projects. It is intended to help select the right tools, inspect their original instructions, combine compatible workflows, and apply them appropriately to each project's stack.

**Important:** Listing a tool here does not mean it is installed or automatically active. Before using any skill, verify its official source, current documentation, license, requirements, and compatibility with the project.

## How we maintain this library

For every new entry:

1. Record its exact name and official source/repository.
2. Classify it correctly: agent skill, library, framework, CLI, design resource, or testing tool.
3. Read the official README and, when present, `SKILL.md`.
4. Record installation and usage instructions from the source.
5. Note prerequisites, supported frameworks, limitations, and license.
6. Add a small practical example when it is useful.
7. Test compatibility with the target project before recommending integration.
8. Preserve existing entries when updating this document.

## Core collection — the original seven

These are the seven items Ibrahim selected as the initial collection. Their detailed source information is pending verification; no repository URL or installation command is assumed.

| # | Name | Initial category | Status |
|---|---|---|---|
| 1 | Impeccable | UI/design workflow or skill — verify exact project | Awaiting source |
| 2 | Taste Skill | Design skill/workflow — verify exact project | Awaiting source |
| 3 | GSAP Skills | Animation ecosystem / related skills — identify exact source | Awaiting source |
| 4 | React Bits | React component library/resource | Awaiting source |
| 5 | Designlang | Verify exact project and category | Awaiting source |
| 6 | Playwright CLI | Browser automation and testing CLI/tooling | Awaiting source |
| 7 | Transitions.dev | Verify exact project and category | Awaiting source |

### Entry template

Use this template for every verified item:

- **Name:**
- **Category:** Agent skill / library / framework / CLI / design resource / testing tool
- **Official website:**
- **GitHub repository:**
- **Documentation:**
- **Skill file:** (exact path, e.g. `SKILL.md`, if present)
- **Purpose:**
- **Best use cases:**
- **Supported stacks:**
- **Installation:**
- **Basic usage:**
- **Dependencies and prerequisites:**
- **License:**
- **Limitations / compatibility notes:**
- **Practical example:**
- **Verification date:**

## Skill categories

- **Design and UX:** visual direction, layout, typography, color, accessibility, responsive behavior.
- **Frontend components:** reusable components, interaction patterns, design systems.
- **Animation and transitions:** motion design, timelines, micro-interactions, page transitions.
- **Development workflow:** project structure, code quality, framework-specific practices.
- **Browser testing:** end-to-end tests, accessibility checks, visual regression, responsive testing.
- **Performance and accessibility:** loading speed, semantic HTML, keyboard navigation, WCAG practices.
- **Backend and integration:** APIs, databases, authentication, deployment, and security.

## Project workflow

When starting or improving a website:

1. Inspect the existing repository and identify its framework, language, build system, and constraints.
2. Review this library and select only relevant, compatible entries.
3. Read the selected tools' original instructions and documentation.
4. Prepare a short implementation plan before changing project files.
5. Implement in small, reviewable steps without removing unrelated features.
6. Run available checks and tests; use browser testing where appropriate.
7. Review desktop, mobile, RTL/LTR, accessibility, and performance as relevant.
8. Record what was used, what changed, and any remaining issues.

## Compatibility rules

- Do not assume a React library can be dropped into a plain PHP page.
- Do not install a package before checking the project's actual stack and package manager.
- Prefer official documentation and maintained repositories.
- Never invent source URLs, package names, commands, or capabilities.
- Keep secrets, API keys, passwords, and private tokens out of this repository.
- Respect each project's existing architecture and preserve unrelated functionality.

## Changelog

- **Initial version:** Created the Prime Skills Developer reference library and recorded Ibrahim's original seven-item collection pending source verification.

---

## External Skills & Website Resources

This section tracks useful external collections and selected resources without mixing third-party libraries, prompts, and installable Agent Skills.

### Tencent EdgeOne — Website Prompts & Skills

- **Source:** https://github.com/TencentEdgeOne/awesome-website-prompts-and-skills
- **Collection type:** Community website-resource gallery maintained by Tencent EdgeOne.
- **Source README count at review:** 50 Skill entries + 116 Prompt entries.
- **Full index and evaluation:** [EXTERNAL-RESOURCES/TENCENT-EDGEONE-CATALOG.md](EXTERNAL-RESOURCES/TENCENT-EDGEONE-CATALOG.md)
- **Reviewed:** 2026-11-13

#### Selected resources for our core workflow

| Resource | Category | Why we keep it | Stack / limitation |
|---|---|---|---|
| [Tech Stack Analyzer](https://github.com/nitai2plipala/tech-stack-analyzer) | Agent skill | Inspect unfamiliar repositories and understand architecture and dependencies before editing. | Broad analysis; PHP-specific detection must be checked. MIT. |
| [Website Skeleton Skill](https://github.com/liuboacean/website-skeleton-skill) | Agent skill / project scaffold | Reference for modular authentication, admin, AI, and full-stack application architecture. | Next.js + EdgeOne Pages; adapt concepts, not a direct PHP/XAMPP install. MIT No Attribution badge in source README. |
| [PortfolioFlow](https://github.com/xixi241225-crypto/portfolio-flow) | Agent skill / project generator | Reference for themes, polished pages, admin dashboard, JWT, analytics, and AI assistant patterns. | EdgeOne Pages + Edge Functions + KV; adapt UI/product patterns only. MIT. |
| [Academic Hub Skills](https://github.com/zixilee666-svg/academic-hub-skills-v1) | Agent skill / educational project generator | Educational-product reference for project management, progress charts, themes, AI-assisted academic workflows, and admin views. | React 19 + TypeScript + Vite + Tailwind; not a drop-in for PHP. MIT. |

#### Adoption rules

1. Tech Stack Analyzer is the first-choice helper when reviewing an unfamiliar repository.
2. Use Website Skeleton and PortfolioFlow as architecture/UI references only when their runtime and deployment assumptions fit.
3. Use Academic Hub as an educational-product feature reference; translate suitable patterns into the target stack.
4. Do not add EdgeOne-specific deployment or storage requirements to projects that use another host or database.
5. Keep source links, license details, and attribution requirements with every adopted resource.
6. The complete 50-entry source index is maintained separately; entries are not all verified installable packages.

### Unslop — AI UI design refinement

- **Category:** Agent Skill — UI/UX audit and visual refinement workflow.
- **Official repository:** https://github.com/heydamir/unslop
- **Skill file:** https://github.com/heydamir/unslop/blob/main/skills/unslop/SKILL.md
- **Purpose:** Audits AI-generated or generic-looking interfaces, identifies visual issues, proposes a product-specific design direction, and refines the screen in ordered passes.
- **Supported agents documented by source:** Claude Code, OpenAI Codex, and Google Antigravity.
- **Supported UI stacks stated by source:** Next.js, React, Vue, Svelte, Tailwind, plain HTML and CSS. It can also inspect a live site from a URL.
- **Workflow:** Audit first; classify the needed change (full redesign, light polish, or no redesign); present the proposed direction and wait for approval before editing; apply ordered refinement passes; render and check the result.
- **Installation — Codex:** `$skill-installer install https://github.com/heydamir/unslop/tree/main/skills/unslop`
- **Installation — Claude Code:** Clone the repository and copy `skills/unslop` into `~/.claude/skills/`; for one project, use `.claude/skills/` in that project.
- **Installation — Google Antigravity:** Copy `skills/unslop` into `~/.gemini/antigravity/skills/`; for one project, the source README also documents `.agents/skills/`.
- **Optional screenshot/story-video prerequisites:** Playwright + Chromium; ffmpeg is additionally required for story videos.
- **License:** CC BY 4.0. Preserve credit to Damir Sokolovsky (@heydamir) and link to the original repository when reusing or adapting it.
- **Compatibility notes:** This is an agent workflow, not a UI component library or automatic site plugin. It can guide changes in PHP-rendered HTML/CSS, but framework-specific instructions and scripts must be checked before use. It does not install itself into ChatGPT automatically.
- **Adoption status:** Added to Ibrahim's reference library; not installed or executed in any project.
- **Reviewed:** 2026-11-13

See [EXTERNAL-RESOURCES/UNSLOP.md](EXTERNAL-RESOURCES/UNSLOP.md) for the focused record and usage notes.


### Scrolltide — UI/UX, Motion Design & Interaction Reference

- **Category:** Design Resource Library — not an Agent Skill, framework, or standalone website builder.
- **Official website:** https://www.scrolltide.co/
- **Library:** https://www.scrolltide.co/templates
- **MCP documentation:** https://www.scrolltide.co/mcp
- **Purpose:** Reference library for scroll-driven website templates, animated components, page sections, UI screens, 3D scenes, and shader backgrounds. Use it to discover motion concepts and interaction patterns, then adapt suitable ideas to the current project.
- **Technology ecosystem shown by the source:** React, Vite, Next.js, Tailwind, Framer Motion, GSAP, Three.js, WebGL, shaders, and Lenis.
- **MCP endpoint:** `https://www.scrolltide.co/api/mcp`; official instructions say it supports Claude, Cursor, Codex, and VS Code, with browser-based account approval and no API key. Access is limited to Yearly and Lifetime plans; fair use is up to 40 different items per account per 24 hours; MCP access is read-only.
- **Motion workflow for Ibrahim's projects:**
  1. When Ibrahim asks for animations, motion, transitions, scroll effects, micro-interactions, or a more dynamic UI, consult Scrolltide's current library when access is available.
  2. Find relevant examples by page purpose and interaction type (e.g. hero reveal, scroll-scrubbed storytelling, parallax, animated cards, navigation transitions, hover/cursor response, 3D scenes, shader backgrounds).
  3. Present or explain the selected motion direction when design approval is useful; do not copy a whole template blindly.
  4. Recreate/adapt the underlying idea to the actual project's framework, dependencies, visual identity, RTL layout, accessibility, and performance budget.
  5. Prefer restrained, purposeful motion; support reduced-motion preferences and avoid adding heavy WebGL/3D effects where they harm mobile performance.
  6. Verify the finished interaction on desktop and mobile and check scroll behavior, keyboard usability, and reduced-motion behavior.
- **Stack compatibility:** Scrolltide prompts are primarily designed for AI coding workflows and modern web stacks. For PHP/XAMPP projects, use the visual/motion concept and translate the implementation into the existing HTML/CSS/JavaScript stack; do not assume React/Next.js code can be pasted directly into PHP.
- **License and usage:** The official Terms state that generated websites may be used, deployed, and monetized for personal or client work, but the source templates/prompts and marketing assets must not be redistributed or resold as standalone products or used to build a competing template/prompt library. Review current terms before paid or commercial adoption.
- **Plans / access note (reviewed 2026-11-13):** Official pages describe Monthly, Yearly, and Lifetime plans; MCP is included with Yearly and Lifetime only. Pricing and entitlements can change; confirm the live pricing page before purchase. Do not imply Ibrahim has purchased a plan or connected MCP.
- **Adoption status:** Saved as a design and motion reference. Not purchased, installed, or connected to this ChatGPT session.
- **Reviewed:** 2026-11-13

**Standing instruction:** Treat Scrolltide as a preferred inspiration source whenever Ibrahim requests UI/UX motion or animation work. Browse its current examples if available, then implement an original, project-compatible adaptation rather than blindly copying assets or code.


## Frontend Design, Motion & Video Production Collection

These resources were selected by Ibrahim and reviewed on 2026-11-13. They are deliberately separated by purpose: frontend visual design, motion-design principles, cinematic video production, React-based video creation, and HTML-to-video rendering. Listing them here does not mean they are installed or connected.

### Frontend Design — Anthropic Skills

- **Category:** Agent Skill — frontend visual design and UI direction.
- **Repository:** https://github.com/anthropics/skills
- **Skill file:** https://github.com/anthropics/skills/blob/main/skills/frontend-design/SKILL.md
- **Purpose:** Creates distinctive, intentional interfaces by grounding visual choices in the product and audience; covers typography, palette, layout, content, critique, responsive quality, accessibility, and restrained motion.
- **Workflow:** Prepare a compact design plan (color, typography, layout, principles), critique it against the brief for generic patterns, then implement.
- **Best use:** New website/page design, redesigns, visual direction, and avoiding generic AI-generated layouts.
- **Compatibility:** Primarily design guidance; can inform React, Vue, and PHP-rendered HTML/CSS. It does not require a specific frontend runtime by itself.
- **License:** No root `LICENSE` file was found at the checked repository path; verify the applicable terms before copying or redistributing skill content.
- **Adoption status:** Reference added; not installed.
- **Reviewed:** 2026-11-13

### Motion Design with Claude and Codex — LobzyJay

- **Category:** Agent Skills — motion-design principles, After Effects, Blender, and motion critique.
- **Repository:** https://github.com/LobzyJay/motion-design-with-claude-and-codex
- **Foundation skill:** https://github.com/LobzyJay/motion-design-with-claude-and-codex/blob/main/skills/motion-design/SKILL.md
- **Specialist skills:** `aftereffects-motion`, `blender-motion`, and `motion-design-critique`.
- **Purpose:** Teaches motion timing, spacing, easing, anticipation, follow-through, composition, and critique; specialist workflows cover After Effects scripting/MCP and Blender animation.
- **Best use:** Motion graphics, title sequences, product animation, 3D scenes, and evaluating animation craft.
- **Important scope limit:** The repository explicitly says web motion (GSAP, Framer Motion, R3F) is out of scope. For website interactions, use Scrolltide and web-animation tools instead.
- **Optional integrations:** After Effects MCP and Blender MCP; these require separate local setup and running applications. Skills can still be used as reference without those MCP servers.
- **Installation:** Follow the repository's current instructions; Codex skill files are provided in the repo. Do not claim MCP control until the corresponding local server is installed and connected.
- **License:** MIT.
- **Adoption status:** Reference added; not installed and no local AE/Blender MCP configured.
- **Reviewed:** 2026-11-13

### Video Shotcraft — Vincentwei1021

- **Category:** Agent Skill and production toolkit — cinematic product-video workflow.
- **Repository:** https://github.com/Vincentwei1021/video-shotcraft
- **Skill entry:** https://github.com/Vincentwei1021/video-shotcraft/blob/main/SKILL.md
- **Purpose:** Creates cinematic product promos from frontend projects or webpages using real page captures, shot recipe cards, storyboards, Remotion demos/templates, music beat-sync, sound design, and quality review.
- **Library contents stated by source:** 124 shot recipe cards, demo implementations, motion-preview gallery, a complete video template, reusable components, and sound/music workflows.
- **Best use:** Promotional videos for websites/apps, feature walkthroughs, product launches, and individual cinematic shots or sound-design work.
- **Workflow:** Understand the product, define visual direction, map features to shots, storyboard, capture assets, implement shots, design sound, and perform independent final review. The source offers direct-template, autonomous, and guided-creation modes.
- **Requirements / compatibility:** Remotion-based production workflow; check the current README and project setup for Node, browser, FFmpeg, and rendering prerequisites. Some optional JianYing export tooling is marked Mac-tested / Windows-untested in the repository; do not assume that optional path works on Windows.
- **License:** Apache-2.0.
- **Adoption status:** Reference added; not installed or run.
- **Reviewed:** 2026-11-13

### Remotion Agent Skills — remotion-dev

- **Category:** Agent Skills for the Remotion video framework.
- **Repository:** https://github.com/remotion-dev/skills
- **Documentation:** https://www.remotion.dev/docs/ai/skills
- **Install command documented by source:** `npx skills add remotion-dev/skills`
- **Purpose:** Official skills for creating Remotion projects and compositions, writing React-based video markup, previewing in Studio, rendering, maps, captions, SaaS integrations, interactivity, documentation lookup, licensing, and upgrades.
- **Best use:** Programmatic video creation with React, animated explainers, product promos, captions, data/map animations, and automated video pipelines.
- **Compatibility:** Requires a React/Remotion project and its supported Node/browser/rendering environment. It is not a drop-in animation library for a plain PHP page.
- **License note:** No root `LICENSE` file was found at the checked skills repository path. Check the skills repository terms and the separate Remotion framework licensing requirements before commercial rendering or redistribution; do not assume the framework is unrestricted.
- **Adoption status:** Reference added; not installed.
- **Reviewed:** 2026-11-13

### HyperFrames — heygen-com

- **Category:** Open-source HTML-to-video framework, CLI, desktop editor, and Agent Skills.
- **Repository:** https://github.com/heygen-com/hyperframes
- **Documentation:** https://hyperframes.heygen.com/introduction
- **Quick start:** https://hyperframes.heygen.com/quickstart
- **Skill entry:** https://github.com/heygen-com/hyperframes/blob/main/skills/hyperframes/SKILL.md
- **Purpose:** Turns HTML, CSS, media, and deterministic seekable animations into MP4 video; includes a CLI, editable Studio workflow, component/transition registry, and skills for coding agents.
- **Best use:** Product promos, animated explainers, kinetic typography, charts/maps, social clips, overlays, and reusable motion graphics.
- **Requirements stated by source:** Node.js 22+ and FFmpeg for CLI use.
- **Important implementation rule:** Every rendered frame must be deterministic; the skill forbids timers, live network fetches, unseeded randomness, and non-seekable animation behavior in the render timeline.
- **Compatibility:** HTML/CSS/JS video compositions; distinct from a normal website animation runtime. It can reuse web-development skills and concepts, but its output is video rather than an interactive website.
- **License:** Apache-2.0 for the repository.
- **Adoption status:** Reference added; not installed or connected.
- **Reviewed:** 2026-11-13

### Selection rules for future work

1. **Designing a website UI:** start with Frontend Design; use Unslop for auditing/refinement.
2. **Animating a website:** use Scrolltide for inspiration and web-native tools such as GSAP/Framer Motion; do not use the Blender/After Effects skill as a web-animation implementation guide.
3. **Motion graphics / 3D animation:** use Motion Design with Claude and Codex, with After Effects or Blender specialists as appropriate.
4. **Making a product promo from an existing website:** consider Video Shotcraft for its shot library and production pipeline.
5. **Creating a video directly with React:** use Remotion Agent Skills.
6. **Creating a video from HTML/CSS compositions:** use HyperFrames.
7. Before installing or running any resource, inspect the actual project stack, operating system, dependencies, current upstream instructions, and license. Never install every tool just because it is listed here.


## Agent Skills — First-Party Workflows

This repository now includes first-party Agent Skills maintained for Ibrahim's recurring development and creative workflows. The skills follow the Agent Skills directory convention: each skill has its own folder and a `SKILL.md` with YAML frontmatter (`name` and `description`).

**Skill catalog:** [skills/README.md](skills/README.md)

| Skill | Directory | Main purpose |
|---|---|---|
| PHP/XAMPP LMS Development | `skills/php-xampp-lms-development/` | Maintain and extend PHP/MySQL educational platforms safely |
| Arabic RTL Frontend Design | `skills/arabic-rtl-frontend-design/` | Build readable, accessible Arabic-first responsive interfaces |
| Web Motion Design | `skills/web-motion-design/` | Select and implement purposeful website motion |
| Repository Review & Testing | `skills/repository-review-testing/` | Inspect existing code, make safe changes, and verify fixes |
| Video Production Workflow | `skills/video-production-workflow/` | Choose and validate product-video and motion-graphics workflows |

### How to use these skills

1. Give the agent access to this repository or copy the relevant skill directory into a location supported by the agent/client.
2. Ask the agent to use the relevant skill for the task.
3. The agent should read the complete `SKILL.md` before planning or editing.
4. Check the target project's stack, operating system, dependencies, and license before installing external tools.
5. Treat these files as workflow instructions, not as proof that any tool, package, MCP server, or integration is installed.

### Standard and maintenance

- Format reference: https://agentskills.io/specification
- Creation guide: https://agentskills.io/skill-creation/quickstart
- Best practices: https://agentskills.io/skill-creation/best-practices
- Keep skill names lowercase and hyphenated, matching their directory names.
- Keep descriptions specific enough for an agent to identify when the skill applies.
- Add scripts, references, and assets only when they materially improve the workflow; document their purpose and requirements.
- Test each skill against representative tasks and revise it when instructions are ambiguous or ineffective.
- Review external source instructions and licenses whenever referenced tools change.

