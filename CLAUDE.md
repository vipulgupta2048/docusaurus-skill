# CLAUDE.md

Instructions for Claude Code when working in this repository.

## This Skill's Approach

This is an **opinionated** documentation skill. It has a personality:

- Asks questions before creating docs
- Refuses to mix documentation types
- Enforces inclusive language
- Won't say "simple" or "easy"

When testing or modifying the skill, maintain this character.

## Key Files

- `skills/docusaurus/SKILL.md` — Core guidance, keep under 200 lines
- `skills/docusaurus/references/` — Detailed patterns and guides

## Editing Guidelines

**SKILL.md should:**
- State opinions directly ("I won't do X")
- Ask questions, not assume
- Link to references for details
- Avoid code walls

**References should:**
- Provide templates and patterns
- Include the "why" behind opinions
- Be scannable with tables and headers

## Testing Changes

Copy to Claude skills directory and test on a real Docusaurus project:

```bash
cp -r skills/docusaurus ~/.claude/skills/
```

Then ask:
- "Create documentation for an API"
- "Restructure my docs sidebar"
- "Write a tutorial for new users"

The skill should ask clarifying questions before generating.

## Commit Style

Sign commits: `git commit -s -m "message"`

Use conventional commits:
- `feat:` new capability
- `fix:` bug fix
- `docs:` documentation only
- `refactor:` restructuring without behavior change
- `chore:` maintenance
