# anti-ai-slop-design

An agent skill for designing, building, redesigning, and auditing frontend interfaces without generic AI-generated defaults.

Instead of "purple gradient hero + three feature cards", it grounds every visual decision in the product, audience, content, and use scene — while respecting the project's existing design contract (`DESIGN.md`, tokens, components) and accessibility.

## Contents

```
SKILL.md                         # entry point: authority order, task modes, workflow
references/
  aesthetic-directions.md        # choosing an art direction from the subject
  anti-patterns.md               # common AI tells and what to do instead
  product-ui.md                  # dashboards, forms, dense product UI
  verification.md                # how to check the result
  provenance.md                  # conceptual sources
assets/DESIGN.template.md        # template for a project-level design contract
agents/openai.yaml               # Codex / OpenAI agents metadata
```

## Install

Claude Code:

```bash
git clone https://github.com/f42gh/anti-ai-slop-design ~/.claude/skills/anti-ai-slop-design
```

Codex and other agents that read `~/.agents/skills`:

```bash
git clone https://github.com/f42gh/anti-ai-slop-design ~/.agents/skills/anti-ai-slop-design
```

Then ask for UI work as usual — the skill triggers on frontend design tasks — or invoke it explicitly with `/anti-ai-slop-design`.

## Credits

Conceptual inspiration only, no copied text or code. See [references/provenance.md](references/provenance.md).

## License

MIT
