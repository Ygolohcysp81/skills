---
name: add-or-update-skill
description: Workflow command scaffold for add-or-update-skill in skills.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /add-or-update-skill

Use this workflow when working on **add-or-update-skill** in `skills`.

## Goal

Adds a new skill or updates an existing skill, including documentation, references, scripts, and marketplace metadata.

## Common Files

- `skills/*/SKILL.md`
- `skills/*/references/*.md`
- `skills/*/examples/*`
- `skills/*/scripts/*.py`
- `.claude-plugin/marketplace.json`
- `README.md`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Create or update SKILL.md in the skill directory.
- Add or update reference files (e.g., references/*.md) relevant to the skill.
- Add or update example files (e.g., examples/*.md, examples/*.json, examples/.env.example) if needed.
- Add or update scripts (e.g., scripts/*.py) for the skill.
- Update .claude-plugin/marketplace.json to register or rename the skill.

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.