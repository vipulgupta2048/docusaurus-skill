# AGENTS.md

Guidance for AI coding agents working with this repository.

## What This Skill Is

An opinionated documentation skill built on the Diátaxis framework. Unlike reference-heavy skills, this one:

1. **Asks questions before generating.** Audience, outcome, and quadrant matter.
2. **Has strong opinions.** Structure, language, and patterns are prescribed.
3. **Refuses certain things.** Won't mix doc types, won't use exclusionary language.

## The Core Philosophy

Documentation enables. Every page answers: "What can the reader DO after?"

## Diátaxis Quadrants

Before creating any documentation, identify the quadrant:

- **Tutorial:** Learning-oriented. Reader says "teach me."
- **How-to:** Task-oriented. Reader says "help me do X."
- **Reference:** Information-oriented. Reader says "what is Y?"
- **Explanation:** Understanding-oriented. Reader says "why does Z?"

**Rule:** Don't mix them. One page, one quadrant.

## When Using This Skill

### Ask These Questions

1. Who is reading this?
2. What should they be able to DO after?
3. Which Diátaxis quadrant is this?
4. What do they already know?

### Apply These Rules

**Language:**
- No "simple," "easy," "just," "obviously"
- Use allowlist/blocklist, not whitelist/blacklist
- "You" for the reader, "they" for hypothetical users

**Structure:**
- Sidebar depth ≤ 3 levels
- One admonition per section max
- Title describes action, not topic

**Content:**
- Context before code
- Minimal examples first, comprehensive second
- Link to other quadrants, don't embed them

## File Structure

```
skills/docusaurus/
├── SKILL.md                    # Core guidance (~170 lines)
├── metadata.json               # Skill metadata
└── references/
    ├── diataxis-patterns.md    # Templates for each quadrant
    ├── writing-guide.md        # Voice, tone, inclusive language
    ├── config-reference.md     # docusaurus.config.ts essentials
    └── deployment.md           # Platform deployment guides
```

## Contributing

When editing this skill:

1. Keep SKILL.md under 200 lines
2. Opinions go in SKILL.md, details go in references
3. Don't add code examples that Docusaurus docs already have
4. Test on real documentation projects
