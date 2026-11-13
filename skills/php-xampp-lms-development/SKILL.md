---
name: php-xampp-lms-development
description: Build, debug, and extend PHP and MySQL educational platforms running locally on XAMPP. Use when working on LMS features such as roles, courses, lessons, exams, homework uploads, grading, progress reports, dashboards, and notifications.
---

# PHP/XAMPP LMS Development

## Goal

Deliver safe, maintainable LMS changes while preserving the existing application's behavior, database structure, and user-facing features unless a change is explicitly requested.

## Before changing code

1. Inspect the repository structure and identify the PHP entry points, routing approach, templates, assets, database layer, and current authentication/session model.
2. Read the relevant files in full, including shared configuration, authorization helpers, and related database queries. Search for every caller of a function or route before changing its contract.
3. Confirm the runtime version, enabled PHP extensions, MySQL/MariaDB version, and whether the project uses PDO or MySQLi. Do not mix database APIs casually.
4. Inspect the existing schema and migrations before proposing SQL. Never assume a column or table exists.
5. State a concise plan and list the files and schema changes expected before broad edits.

## Implementation rules

- Preserve unrelated routes, features, styling, and existing data. Prefer small, reviewable changes.
- Use prepared statements for all values supplied by users or external devices.
- Hash passwords with PHP's password APIs; never store plaintext passwords.
- Enforce authorization on the server for every role-specific action. Hiding a button is not authorization.
- Validate ownership and course/subject membership on every read and write involving student, teacher, assistant, or administrator records.
- Escape untrusted output for its HTML context. Validate CSRF tokens for state-changing browser forms.
- Use transactions when a workflow must update multiple related records atomically.
- Keep secrets and production credentials outside the repository. Use placeholders in examples and never echo credentials into logs.
- For file uploads, check upload errors, size limits, allowed extensions and MIME types, generate server-side filenames, store files outside executable paths where possible, and prevent path traversal and direct execution.
- Validate invitation/enrollment codes server-side, make one-time codes single-use atomically, and avoid exposing predictable identifiers as authorization.
- For exams, validate start/end windows, duration, attempt limits, ownership, and server-side grading. Do not rely on client clocks or client-submitted scores.
- For progress calculations and grades, document the formula, handle zero denominators, and test boundary cases before changing existing semantics.

## UI and localization

- Preserve the project's existing design system unless redesign is requested.
- For Arabic screens, maintain `lang="ar"`, `dir="rtl"`, readable Arabic typography, correct mixed-direction handling for code and numbers, and keyboard-friendly controls.
- Make layouts responsive for phones as well as desktop. Do not rely on color alone to communicate status.
- Keep forms, validation messages, empty states, loading states, and error states consistent.

## Database changes

- Prefer additive, reversible schema changes. Include the exact SQL migration and explain backup requirements.
- Never drop or rename existing tables/columns without explicit approval and a migration plan.
- Use indexes for frequently filtered foreign keys and lookup fields when justified.
- Test queries against the actual schema; do not invent field names.

## Verification checklist

- Run PHP syntax checks on changed PHP files when the runtime is available.
- Exercise the affected flow with authorized and unauthorized accounts.
- Test empty, invalid, duplicate, boundary, and normal inputs.
- Verify upload rejection cases as well as a valid upload.
- Confirm database writes, redirects, messages, and reports.
- Check browser console/network errors and mobile RTL rendering.
- Summarize changed files, SQL steps, tests actually run, and remaining risks. Never claim a test passed unless it was run.

## Project-specific caution

A PHP/XAMPP LMS is not automatically compatible with React/Next.js packages. Borrow design ideas where useful, but implement them in the project's real stack unless a migration is explicitly requested.
