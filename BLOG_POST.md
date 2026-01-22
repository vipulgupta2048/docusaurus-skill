# Blog Post: The Docusaurus Skill That Says "No"

---

**Title Options:**
1. "I Built a Documentation Skill That Refuses to Help (And That's The Point)"
2. "The Docusaurus Skill That Asks Questions Before Writing Code"
3. "Why I Taught Claude to Say 'No' to Documentation Requests"

**SEO Keywords:** docusaurus, diátaxis, documentation, ai agent, claude code, technical writing, inclusive language

---

## The Problem With Helpful AI

*Narrator: The AI was too eager to help.*

Ask Claude to "create documentation for my API" and it'll happily generate walls of markdown. Comprehensive? Sure. Frontmatter? Perfect. Useful? ...Maybe.

The problem isn't capability. It's context.

Documentation isn't typing—it's thinking. And when AI skips the thinking part, you get docs that technically exist but don't actually help anyone.

After managing 30+ Docusaurus sites at Balena, I decided to build a skill that does something unusual: it asks questions before it writes a single line.

## Enter Diátaxis

The [Diátaxis framework](https://diataxis.fr/) changed how I think about documentation. It splits docs into four quadrants:

| Type | Purpose | Reader Asks |
|------|---------|-------------|
| **Tutorial** | Learning | "Teach me" |
| **How-to** | Doing | "Help me do X" |
| **Reference** | Information | "What is Y?" |
| **Explanation** | Understanding | "Why does Z?" |

The key insight: **don't mix them**. A tutorial that becomes reference midway loses both audiences.

But here's the thing—AI doesn't know which quadrant you need. It'll happily combine all four into one page, creating something that serves no one well.

## A Skill With Opinions

The Docusaurus Skill I built has strong opinions:

**It asks questions first:**
- Who is reading this?
- What should they be able to DO after?
- Which Diátaxis quadrant is this?
- What do they already know?

**It refuses certain things:**
- Won't mix documentation types in one page
- Won't add "simple" or "easy" to instructions
- Won't skip the description field in frontmatter
- Won't create sidebars deeper than 3 levels

**It enforces inclusive language:**
- allowlist/blocklist, not whitelist/blacklist
- primary/replica, not master/slave
- No "guys," no "sanity check," no ableist language

## Why "Simple" Is Banned

Let me explain this one because it's close to my heart.

When documentation says "Simply run the command..." it implies the task is easy. For the person who wrote it, maybe it was. But for the reader who's stuck, who's been debugging for an hour, that word makes them feel stupid.

"If it's so simple, why can't I figure it out?"

Removing "simple" and "easy" from documentation is a small change that makes docs more welcoming. The skill enforces this automatically.

## The Skill In Action

Here's what happens when you ask the skill to create documentation:

**You:** "Create docs for our authentication API"

**Skill:** "Before I write anything, I need to understand:
1. Who's reading this? New users learning auth concepts, or developers implementing it?
2. What should they DO after reading? Understand how auth works, or integrate it into their app?
3. Is this a tutorial, how-to guide, reference, or explanation?"

Only after answers does it generate—and what it generates fits the actual need.

## What It Won't Generate

The skill won't create:
- Walls of code examples without context
- Pages that mix teaching and reference
- Documentation that assumes your audience
- Content using exclusionary language

If you ask for something that violates these principles, it'll explain why and suggest an alternative.

## Built From Real Experience

This isn't theoretical. It's built from:
- Managing 30+ Docusaurus sites at Balena
- Reviewing hundreds of documentation PRs
- Watching users struggle with "comprehensive" docs that didn't help
- Reading every Diátaxis principle twice

The skill encodes the judgment I wish I'd had when I started writing documentation.

## Get It

```bash
npx skills add vipulgupta2048/docusaurus-skill
```

Or clone it:
```bash
git clone https://github.com/vipulgupta2048/docusaurus-skill
cp -r docusaurus-skill/skills/docusaurus ~/.claude/skills/
```

The skill is MIT licensed. Fork it, adapt it, argue with its opinions.

## The Bigger Picture

AI is making documentation easier to produce. But easier production doesn't mean better documentation.

What we need is AI that understands the *purpose* of documentation—not just its format. AI that asks "who is this for?" before "what should it contain?"

This skill is my attempt at that. It's opinionated because good documentation requires opinions. It asks questions because good documentation requires understanding.

Try it. Argue with it. Make it better.

---

*Have thoughts? Find me on [Twitter](https://twitter.com/vipulgupta2048) or [open an issue](https://github.com/vipulgupta2048/docusaurus-skill/issues).*

---

## Social Media Content

### Twitter Thread

**Tweet 1:**
I built an AI skill that refuses to help.

Ask it to "create documentation" and it'll say: "Before I write anything, I need to understand who's reading this."

It has opinions. It bans words. It won't skip questions.

Here's why:

**Tweet 2:**
Most AI documentation tools are too helpful.

"Create API docs" → Walls of markdown

Technically correct. Actually useless.

Documentation isn't typing. It's thinking.

**Tweet 3:**
The skill uses Diátaxis—four types of docs:

🎓 Tutorial: "Teach me"
🔧 How-to: "Help me do X"
📖 Reference: "What is Y?"
💡 Explanation: "Why does Z?"

Rule: Don't mix them.

A tutorial that becomes reference loses both audiences.

**Tweet 4:**
It bans certain words:

❌ simple, easy, just
❌ whitelist/blacklist
❌ master/slave
❌ sanity check

"Simply run the command" makes struggling readers feel stupid.

**Tweet 5:**
Before generating anything, it asks:

1. Who is reading this?
2. What should they DO after?
3. Which documentation type?
4. What do they already know?

Only then does it write.

**Tweet 6:**
Built from managing 30+ Docusaurus sites.

MIT licensed. Has opinions. Will argue.

github.com/vipulgupta2048/docusaurus-skill

Install:
```
npx skills add vipulgupta2048/docusaurus-skill
```

---

### LinkedIn Post

**An AI skill that says "no"**

I built a documentation skill for AI coding agents that refuses to help until it understands the context.

Ask it to "create API documentation" and instead of generating walls of markdown, it asks:
- Who is reading this?
- What should they be able to DO after?
- Is this a tutorial, how-to, reference, or explanation?

Why? Because documentation isn't about typing—it's about thinking.

The skill is built on the Diátaxis framework and enforces:
→ Never mix documentation types in one page
→ Inclusive language (no "whitelist," no "simple," no "guys")
→ Questions before generation

After managing 30+ Docusaurus sites at Balena, I encoded the judgment I wish I'd had on day one.

MIT licensed: github.com/vipulgupta2048/docusaurus-skill

Install: `npx skills add vipulgupta2048/docusaurus-skill`

#Documentation #OpenSource #AI #TechnicalWriting #DeveloperExperience

---

## Distribution Checklist

- [ ] Publish on mixster.dev
- [ ] Tweet thread from @vipulgupta2048
- [ ] LinkedIn post
- [ ] Submit to Hacker News
- [ ] Post in Docusaurus Discord
- [ ] Share in Write the Docs Slack
- [ ] Cross-post to dev.to
