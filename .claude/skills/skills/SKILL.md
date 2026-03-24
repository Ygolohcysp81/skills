---
name: skills-conventions
description: Development conventions and patterns for skills. Python project with freeform commits.
---

# Skills Conventions

> Generated from [Ygolohcysp81/skills](https://github.com/Ygolohcysp81/skills) on 2026-03-24

## Overview

This skill teaches Claude the development patterns and conventions used in skills.

## Tech Stack

- **Primary Language**: Python
- **Architecture**: hybrid module organization
- **Test Location**: separate

## When to Use This Skill

Activate this skill when:
- Making changes to this repository
- Adding new features following established patterns
- Writing tests that match project conventions
- Creating commits with proper message format

## Commit Conventions

Follow these commit message conventions based on 200 analyzed commits.

### Commit Style: Free-form Messages

### Message Guidelines

- Average message length: ~41 characters
- Keep first line concise and descriptive
- Use imperative mood ("Add feature" not "Added feature")


*Commit message example*

```text
jobs: add scheduled jobs CLI commands to Quick Reference table
```

*Commit message example*

```text
docs: fix Agent Skills grammar in README (#67)
```

*Commit message example*

```text
feat: add SECURITY.md for coordinated vulnerability disclosure
```

*Commit message example*

```text
fix: prevent SQL injection in sql_manager.py
```

*Commit message example*

```text
Update generate_agents.py
```

*Commit message example*

```text
Document gradio CLI commands for info and predict in Gradio skill (#91)
```

*Commit message example*

```text
[ENHANCEMENT] rename skills for simplicity (#99)
```

*Commit message example*

```text
Merge pull request #89 from huggingface/ben/eval-skill-scope
```

## Architecture

### Project Structure: Monorepo

This project uses **hybrid** module organization.

### Configuration Files

- `.github/workflows/generate-agents.yml`
- `.github/workflows/push-evals-leaderboard.yml`
- `.github/workflows/push-hackers-leaderboard.yml`
- `.github/workflows/push-quests.yml`

### Guidelines

- This project uses a hybrid organization
- Follow existing patterns when adding new code

## Code Style

### Language: Python

### Naming Conventions

| Element | Convention |
|---------|------------|
| Files | snake_case |
| Functions | camelCase |
| Classes | PascalCase |
| Constants | SCREAMING_SNAKE_CASE |

### Import Style: Relative Imports

### Export Style: Named Exports


*Preferred import style*

```typescript
// Use relative imports
import { Button } from '../components/Button'
import { useAuth } from './hooks/useAuth'
```

*Preferred export style*

```typescript
// Use named exports
export function calculateTotal() { ... }
export const TAX_RATE = 0.1
export interface Order { ... }
```

## Common Workflows

These workflows were detected from analyzing commit patterns.

### Feature Development

Standard feature implementation workflow

**Frequency**: ~7 times per month

**Steps**:
1. Add feature implementation
2. Add tests for feature
3. Update documentation

**Files typically involved**:
- `**/*.test.*`

**Example commit sequence**:
```
update cursor version
Added transformer.js (#82)
docs: fix Agent Skills grammar in README (#67)
```

### Add Or Update Skill

Adds a new skill or updates an existing skill, including documentation, references, scripts, and marketplace metadata.

**Frequency**: ~3 times per month

**Steps**:
1. Create or update SKILL.md in the skill directory.
2. Add or update reference files (e.g., references/*.md) relevant to the skill.
3. Add or update example files (e.g., examples/*.md, examples/*.json, examples/.env.example) if needed.
4. Add or update scripts (e.g., scripts/*.py) for the skill.
5. Update .claude-plugin/marketplace.json to register or rename the skill.
6. Update README.md and agents/AGENTS.md to reflect the new or changed skill.

**Files typically involved**:
- `skills/*/SKILL.md`
- `skills/*/references/*.md`
- `skills/*/examples/*`
- `skills/*/scripts/*.py`
- `.claude-plugin/marketplace.json`
- `README.md`
- `agents/AGENTS.md`

**Example commit sequence**:
```
Create or update SKILL.md in the skill directory.
Add or update reference files (e.g., references/*.md) relevant to the skill.
Add or update example files (e.g., examples/*.md, examples/*.json, examples/.env.example) if needed.
Add or update scripts (e.g., scripts/*.py) for the skill.
Update .claude-plugin/marketplace.json to register or rename the skill.
Update README.md and agents/AGENTS.md to reflect the new or changed skill.
```

### Sync Or Update Hf Cli Skill

Synchronizes or updates the Hugging Face CLI skill documentation with upstream changes.

**Frequency**: ~3 times per month

**Steps**:
1. Update skills/hf-cli/SKILL.md (and sometimes skills/hugging-face-cli/SKILL.md).
2. Optionally update related reference files (e.g., references/commands.md, references/examples.md).
3. Commit with a message referencing the upstream commit or version.

**Files typically involved**:
- `skills/hf-cli/SKILL.md`
- `skills/hugging-face-cli/SKILL.md`
- `skills/hugging-face-cli/references/commands.md`
- `skills/hugging-face-cli/references/examples.md`

**Example commit sequence**:
```
Update skills/hf-cli/SKILL.md (and sometimes skills/hugging-face-cli/SKILL.md).
Optionally update related reference files (e.g., references/commands.md, references/examples.md).
Commit with a message referencing the upstream commit or version.
```

### Update Skill Cli Documentation

Updates CLI command documentation tables or help output in a skill's documentation.

**Frequency**: ~2 times per month

**Steps**:
1. Edit SKILL.md to update CLI command tables or help output.
2. Verify against upstream or source CLI implementation.
3. Commit with a message referencing the commands or verification.

**Files typically involved**:
- `skills/*/SKILL.md`

**Example commit sequence**:
```
Edit SKILL.md to update CLI command tables or help output.
Verify against upstream or source CLI implementation.
Commit with a message referencing the commands or verification.
```

### Merge Or Sync Main Branch

Merges changes from the main branch into a feature or refactor branch, updating many files for consistency.

**Frequency**: ~2 times per month

**Steps**:
1. Merge main into feature/refactor branch.
2. Update a wide set of files across skills, scripts, and metadata.
3. Resolve conflicts and ensure consistency.

**Files typically involved**:
- `.claude-plugin/marketplace.json`
- `.claude-plugin/plugin.json`
- `.cursor-plugin/plugin.json`
- `README.md`
- `agents/AGENTS.md`
- `skills/*/SKILL.md`
- `skills/*/references/*`
- `skills/*/scripts/*`

**Example commit sequence**:
```
Merge main into feature/refactor branch.
Update a wide set of files across skills, scripts, and metadata.
Resolve conflicts and ensure consistency.
```


## Best Practices

Based on analysis of the codebase, follow these practices:

### Do

- Use snake_case for file names
- Prefer named exports

### Don't

- Don't deviate from established patterns without discussion

---

*This skill was auto-generated by [ECC Tools](https://ecc.tools). Review and customize as needed for your team.*
