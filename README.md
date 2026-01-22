# Docusaurus Skill

> Opinionated guidance for building documentation people actually read.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Diátaxis](https://img.shields.io/badge/Framework-Diátaxis-purple)](https://diataxis.fr/)

Built from managing 30+ Docusaurus sites. Has opinions. Will ask questions.

## Philosophy

Documentation isn't about documenting—it's about **enabling**.

Every page should answer: *What can the reader DO after reading this?*

## The Diátaxis Framework

This skill organizes docs into four quadrants:

| Type | Purpose | Reader's Question |
|------|---------|-------------------|
| **Tutorial** | Learning | "Teach me to..." |
| **How-to** | Doing | "How do I...?" |
| **Reference** | Information | "What is...?" |
| **Explanation** | Understanding | "Why does...?" |

**The rule:** Don't mix them. A tutorial that becomes reference loses both audiences.

## What Makes This Different

Most documentation skills give you code snippets. This one gives you opinions:

- **Asks questions first.** Who's reading? What should they DO after? Which quadrant?
- **Inclusive language required.** No "whitelist," no "simple," no "guys."
- **Structure that scales.** Learn → Do → Understand → Look up.
- **Won't generate walls of code.** Context first, examples second.

## Installation

```bash
npx skills add vipulgupta2048/docusaurus-skill
```

Or manually:
```bash
git clone https://github.com/vipulgupta2048/docusaurus-skill.git
cp -r docusaurus-skill/skills/docusaurus ~/.claude/skills/
```

## What It Does

Tell the skill what you're building:
```
"I need to document our authentication API for developers"
```

It'll ask:
1. Who's reading this? (New users? Experienced devs?)
2. What should they DO after? (Implement auth? Understand the flow?)
3. Which quadrant? (Tutorial? Reference?)
4. What do they already know?

Then it builds the right structure.

## What It Won't Do

- Create docs without understanding the audience
- Mix documentation types in one page
- Add "simple" or "easy" to instructions
- Skip the frontmatter description field
- Create sidebars deeper than 3 levels

## Skill Contents

```
skills/docusaurus/
├── SKILL.md                           # Core guidance (166 lines)
├── metadata.json
└── references/
    ├── diataxis-patterns.md           # Templates per quadrant
    ├── writing-guide.md               # Voice, tone, inclusive language
    ├── config-reference.md            # Essential config options
    └── deployment.md                  # Platform guides
```

## The Opinions

**On structure:**
```
docs/
├── getting-started/    # Tutorials
├── guides/             # How-tos
├── concepts/           # Explanation
├── reference/          # Reference
└── resources/          # Links, changelog
```

**On language:**

| Don't | Do |
|-------|-----|
| whitelist/blacklist | allowlist/blocklist |
| master/slave | primary/replica |
| simple, easy | *(just remove it)* |
| sanity check | confidence check |

**On admonitions:**
One per section. If everything is highlighted, nothing is.

## Credits

- [Diátaxis](https://diataxis.fr/) by Daniele Procida
- [Google's inclusive documentation guide](https://developers.google.com/style/inclusive-documentation)
- Lessons from 30+ Docusaurus sites at [Balena](https://balena.io)

## License

MIT

---

*Questions? Opinions of your own? [Open an issue](https://github.com/vipulgupta2048/docusaurus-skill/issues).*
