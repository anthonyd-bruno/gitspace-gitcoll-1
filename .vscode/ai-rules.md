# AI Agent Rules (Bruno Workspace)

These rules apply to all AI agents used in this repository via VSCode.

---

## ALWAYS

- Use the **existing codebase as primary context** before generating answers or code.
- Align with patterns already used in the repository (naming, structure, error handling, tests).
- Use **https://usebruno.com** and **https://docs.usebruno.com** as authoritative references when relevant.
- Assume this is a **Bruno workspace** and follow Bruno ecosystem conventions.
- Prefer minimal, review-friendly diffs.
- Reuse existing utilities/helpers before introducing new ones.
- Match the repo’s formatting, linting, and typing standards.
- Update or suggest updating tests when behavior changes.
- Clearly state assumptions if something is unclear.

---

## NEVER

- Invent APIs, configs, or behaviors (without explicitly being asked) that are not present in:
  - The current codebase
  - usebruno.com
  - docs.usebruno.com
- Introduce large refactors unless explicitly requested.
- Add new dependencies without checking for an existing solution.
- Change public interfaces without considering backward compatibility.
- Ignore existing architectural patterns in favor of “cleaner” but inconsistent solutions.

---

## WHEN UNCERTAIN

1. Search the codebase for similar implementations.
2. Check Bruno documentation for intended behavior.
3. Follow the simplest approach that aligns with current patterns.
4. Ask for clarification rather than guessing on product behavior.

---

## RESPONSE STYLE

- Be concise.
- Be implementation-focused.
- Reference relevant files and modules when possible.
- Provide concrete next steps instead of high-level theory.