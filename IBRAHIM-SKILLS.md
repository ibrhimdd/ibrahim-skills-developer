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