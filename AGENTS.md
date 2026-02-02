# Agent Guidelines for founder-ops-toolkit

## Repository Overview

**Name:** founder-ops-toolkit
**Author:** Emilly Humphress / WhiteBoston
**License:** MIT
**Repository:** https://github.com/emillycunha/founder-ops-toolkit

Operations skills for service-based founders following the **Extract → Assign → Scale** framework.

## Structure

```
founder-ops-toolkit/
├── .claude-plugin/
│   └── marketplace.json
├── skills/
│   └── operations/
│       └── skill-name/
│           └── SKILL.md
├── AGENTS.md
├── CLAUDE.md
├── README.md
├── LICENSE
└── VERSIONS.md
```

## Skill Format

Each skill lives in `skills/operations/skill-name/` with a `SKILL.md` file.

### Required Frontmatter

```yaml
---
name: skill-name
version: 1.0.0
description: When the user wants to [trigger phrase]. Also use when [additional triggers].
---
```

**Constraints:**
- `name`: 1-64 chars, lowercase alphanumeric with hyphens, must match directory name
- `description`: 1-1024 chars, include trigger phrases for skill discovery

### Writing Guidelines

- Keep skill files under 500 lines
- Use H2 headers for sections
- Favor bullet lists over paragraphs
- Use active voice
- Be specific, not vague

## Git Workflow

### Commit Messages

Use conventional commits:
- `feat: add new skill`
- `fix: correct skill logic`
- `docs: update readme`

### Branch Names

Use descriptive names: `feat/skill-name`, `fix/skill-issue`

## Version Management

Check `VERSIONS.md` for skill version tracking. Update version when modifying skills.
