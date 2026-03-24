---
name: sync-or-update-hf-cli-skill
description: Workflow command scaffold for sync-or-update-hf-cli-skill in skills.
allowed_tools: ["Bash", "Read", "Write", "Grep", "Glob"]
---

# /sync-or-update-hf-cli-skill

Use this workflow when working on **sync-or-update-hf-cli-skill** in `skills`.

## Goal

Synchronizes or updates the Hugging Face CLI skill documentation with upstream changes.

## Common Files

- `skills/hf-cli/SKILL.md`
- `skills/hugging-face-cli/SKILL.md`
- `skills/hugging-face-cli/references/commands.md`
- `skills/hugging-face-cli/references/examples.md`

## Suggested Sequence

1. Understand the current state and failure mode before editing.
2. Make the smallest coherent change that satisfies the workflow goal.
3. Run the most relevant verification for touched files.
4. Summarize what changed and what still needs review.

## Typical Commit Signals

- Update skills/hf-cli/SKILL.md (and sometimes skills/hugging-face-cli/SKILL.md).
- Optionally update related reference files (e.g., references/commands.md, references/examples.md).
- Commit with a message referencing the upstream commit or version.

## Notes

- Treat this as a scaffold, not a hard-coded script.
- Update the command if the workflow evolves materially.