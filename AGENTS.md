# AGENTS.md

## Purpose
This file defines repository-local behavior for Codex when working in this project.

## Scope
- Applies to all files in this repository unless the user gives direct instructions that override it.

## Priorities
1. Follow direct user instructions first.
2. Keep game logic consistent with `Game_Rules.md`, and `LLM_Rules.md`.
3. Prefer minimal, targeted changes over broad refactors.

## Editing Rules
- Do not change game mechanics unless explicitly requested.
- Preserve existing file formats and naming conventions.
- Avoid introducing new dependencies unless requested.
- Keep Markdown readable and structured with clear headings/lists.
- When fixing formatting issues, avoid semantic changes.

## Markdown Metadata Update Rule
- Do not auto-increment `Revision` fields unless the user explicitly asks for a revision bump.
- Do not auto-update `Updated` timestamps unless the user explicitly asks for a timestamp update.

## Validation Rules
- If behavior rules are edited, ensure no contradiction across:
  - `Game_Rules.md`
  - `LLM_Rules.md`
- If a rule is duplicated in multiple files, keep wording aligned.

## Output Style for Codex
- Be concise and actionable.
- State assumptions when requirements are ambiguous.
- Summarize changed files and what was changed.

## Safety
- Never delete or rewrite large sections of content without explicit user request.
- If required context is missing, ask for clarification before making risky changes.
