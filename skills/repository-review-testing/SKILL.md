---
name: repository-review-testing
description: Review an existing software repository before making changes, trace related code paths, identify defects and risks, and verify fixes with appropriate tests. Use for codebase audits, bug fixes, refactors, and pre-release checks.
---

# Repository Review and Testing

## Review before editing

1. Confirm the repository, branch, working tree state, framework, runtime, package manager, and deployment target.
2. Read the project README, configuration, dependency manifests, routing, data models, authentication/authorization, and relevant tests.
3. Map the user-visible flow to its routes, components, APIs, database operations, and background jobs.
4. Search for all usages of functions, fields, endpoints, and CSS classes that may be affected.
5. Separate confirmed defects from hypotheses. Cite file paths and line ranges where possible.
6. Produce a prioritized review: critical security/data-loss issues first, then correctness, compatibility, accessibility, performance, and maintainability.

## Safe change strategy

- Preserve existing behavior unless the requested change requires altering it.
- Avoid broad rewrites when a targeted fix is safer.
- Do not delete or replace files based only on their names; inspect their contents and callers.
- Keep public API contracts, route names, database semantics, and form fields stable unless migration is intentional.
- Add or update regression tests for each confirmed defect.
- Do not expose secrets in reports, screenshots, commits, or logs.

## Testing strategy

- Select tests based on the changed behavior: unit, integration, end-to-end, accessibility, visual, and manual checks as appropriate.
- If Playwright is available, use it to verify the real user flow, viewport behavior, console errors, and network failures.
- Do not assume a Playwright CLI command or configuration exists; inspect installed versions and project scripts first.
- Test normal, invalid, empty, boundary, unauthorized, and failure paths.
- For UI changes, compare desktop and mobile and verify keyboard/focus behavior.
- For database or file changes, verify persistence and safe failure/rollback behavior.

## Reporting

For every issue, provide severity, evidence, affected path, impact, and a practical fix.
For every change, list modified files, tests actually executed, test results, and anything not tested.
Never describe code as fully tested, secure, or production-ready without evidence.
