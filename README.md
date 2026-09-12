# ani-skills

A small, growing collection of [agent skills](https://docs.claude.com/en/docs/claude-code/skills) — self-contained instruction modules that teach Claude Code (and compatible agents) how to do a specific kind of work well.

Each skill is a folder with a `SKILL.md` file: YAML frontmatter (`name` + `description` that tells the agent *when* to reach for it) followed by the instructions themselves. Drop one into your agent's skills directory and it becomes available on demand.

## Skills

| Skill | What it does |
|-------|--------------|
| [`find-unknowns`](skills/find-unknowns) | Maps the unknowns in an idea, feature, or plan before they get expensive — a blind-spot pass, a known/unknown quadrant map, and a decision-changing interview. Reach for it to de-risk a decision, stress-test a pivot, or answer "what am I missing?" |
| [`thought-partner`](skills/thought-partner) | Pre-build thought partner. Inherits `find-unknowns` and Garry Tan's gstack office-hours: maps blind spots, asks the hard questions one at a time, forces a wedge and alternatives, then hands you a go / no-go / spike brief. No code until the brief is approved. |
| [`deep-write`](skills/deep-write) | Turns a raw thought dump into a publish-ready essay plus an X thread and a LinkedIn post, with deep research at every stage. Ships with a retunable house voice, output templates, and a self-evolving profile layer that each user grows from empty. |
| [`product-psychology`](skills/product-psychology) | Applies the [Growth.Design](https://growth.design/psychology) / Benson catalog (106 biases and UX principles across information, meaning, time, and memory) when designing a product surface. Diagnose the bucket, pick a few principles, pass an ethics floor, then stop. |
| [`product-psychology-audit`](skills/product-psychology-audit) | Reviews a live flow against the same catalog. Walks information → meaning → time → memory and reports principle, evidence, risk, fix, severity. Pair it with `product-psychology` (sibling folder required). |

More to come.

## Install

Skills live in `~/.claude/skills/` for Claude Code. You can either symlink (recommended — you get updates with a `git pull`) or copy.

**Symlink a single skill:**

```bash
git clone https://github.com/anianroid/ani-skills.git
ln -s "$PWD/ani-skills/skills/find-unknowns" ~/.claude/skills/find-unknowns
ln -s "$PWD/ani-skills/skills/thought-partner" ~/.claude/skills/thought-partner
ln -s "$PWD/ani-skills/skills/product-psychology" ~/.claude/skills/product-psychology
ln -s "$PWD/ani-skills/skills/product-psychology-audit" ~/.claude/skills/product-psychology-audit
```

**Or copy it:**

```bash
cp -r ani-skills/skills/find-unknowns ~/.claude/skills/
cp -r ani-skills/skills/thought-partner ~/.claude/skills/
cp -r ani-skills/skills/product-psychology ~/.claude/skills/
cp -r ani-skills/skills/product-psychology-audit ~/.claude/skills/
```

`product-psychology-audit` expects `product-psychology` as a sibling folder.

Then invoke it in Claude Code with `/find-unknowns`, `/thought-partner`, `/product-psychology`, or `/product-psychology-audit`, or just describe the task and let the agent pick it up from the `description`.

> Skills also work at the project level (`.claude/skills/`) and inside plugins. See the [Claude Code skills docs](https://docs.claude.com/en/docs/claude-code/skills) for the full loading model.

## Adding a skill

1. Create a folder under `skills/<your-skill-name>/`.
2. Add a `SKILL.md` with frontmatter:

   ```markdown
   ---
   name: your-skill-name
   description: One or two sentences on what it does AND when the agent should use it — the "when" is what makes it fire at the right time.
   ---

   # Your Skill

   The instructions...
   ```

3. Keep it self-contained. Supporting files (references, scripts, templates) can live alongside `SKILL.md` in the same folder.
4. Add a row to the table above and open a PR.

## License

[MIT](LICENSE) — use it, fork it, remix it.

## Credits

- `find-unknowns` is based on ["A Field Guide to Fable: Finding Your Unknowns"](https://x.com/trq212) by [@trq212](https://x.com/trq212).
- `thought-partner` inherits `find-unknowns` and the forcing-question / premise / alternatives methodology from [gstack](https://github.com/garrytan/gstack) by [Garry Tan](https://github.com/garrytan) (MIT).
- `product-psychology` and `product-psychology-audit` are based on [106 Cognitive Biases & Principles That Affect Your UX](https://growth.design/psychology) by [Growth.Design](https://growth.design), organized around [Buster Benson](https://busterbenson.com)'s four-bucket Cognitive Bias Codex.
