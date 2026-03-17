# ljg-skills

My custom skills for [Claude Code](https://docs.anthropic.com/en/docs/claude-code).

## Skills

| Skill | Description |
|-------|-------------|
| **ljg-card** | Content caster — transforms content into PNG visuals (long card, infograph, poster). Infograph mode uses a content-adaptive design system: the AI analyzes content density, structure, and emotion to generate unique visual compositions from scratch — no fixed template, style serves thought. |
| **ljg-paper** | Paper reader — academic paper analysis pipeline |
| **ljg-paper-flow** | Paper workflow — reads papers + casts cards in one go (combines ljg-paper and ljg-card) |
| **ljg-plain** | Plain language rewriter — makes complex content accessible |
| **ljg-skill-map** | Skill map viewer — visual overview of all installed skills |
| **ljg-word** | English word mastery — deep-dive word deconstruction |
| **ljg-writes** | Writing engine — think through an idea by writing it out |

## Install

Copy any skill directory into `~/.claude/skills/`, then restart Claude Code.

```bash
# Example: install a single skill
cp -r ljg-plain ~/.claude/skills/

# Or clone the whole repo
git clone https://github.com/lijigang/ljg-skills.git /tmp/ljg-skills
cp -r /tmp/ljg-skills/ljg-* ~/.claude/skills/
```

Note: `ljg-card` requires Playwright for screenshot capture. Run `cd ~/.claude/skills/ljg-card && npm install` after installing.
