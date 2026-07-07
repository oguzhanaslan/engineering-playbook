# Engineering Playbook

Claude config for an engineering manager who codes and reviews.

## Rules
- Concise, checklist-first output. Reasoning only when asked.
- Small, reviewable changes. Ask before large refactors or destructive actions.
- Use each skill's own `references/` and `templates/` only when needed.
- Never output secrets or private data.

## Map
- `skills/` — one skill per task; Claude picks by description, loading its references/templates only when needed.
