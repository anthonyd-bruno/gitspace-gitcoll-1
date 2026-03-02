# AI Agent Instructions (Bruno Workspace)

These instructions apply to any AI assistant/agent used inside VSCode for this repository.

## Context requirements (must follow)
1. **Use the codebase as primary context**
   - Prefer answers grounded in the actual repository: existing modules, patterns, conventions, naming, and prior art.
   - When unsure, inspect nearby files and follow established approaches rather than inventing new ones.

2. **Use Bruno documentation as supporting context**
   - Treat these as authoritative references when they apply:
     - https://usebruno.com
     - https://docs.usebruno.com
     - https://github.com/usebruno/bruno
   - If behavior, terminology, or APIs are unclear in the codebase, align guidance with these sites.

3. **This is a Bruno workspace**
   - Assume the project is part of the Bruno ecosystem and should reflect Bruno standards and conventions.
   - Keep changes consistent with Bruno product expectations (UX, naming, configuration style, error handling, and documentation tone).

## How to answer
- Be specific and actionable: file paths, functions, interfaces, and exact next steps.
- Prefer minimal, safe changes that fit existing architecture.
- If you propose code, ensure it matches repo conventions (linting, formatting, testing patterns).
- When you make assumptions, state them clearly and suggest what to check in the codebase to confirm.

## Implementation guidance
- Before adding dependencies or new patterns, check if the repo already has a preferred solution.
- When editing:
  - Avoid broad refactors unless explicitly requested.
  - Keep diffs focused and easy to review.
- When writing docs/comments:
  - Keep them concise and aligned with Bruno terminology.

## Quality checks
- Update or add tests when logic changes.
- Run or suggest the repo’s standard checks (lint/test/build) relevant to the change.
- Watch for backwards compatibility and config migration impacts when touching public interfaces.