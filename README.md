# ani-skills

A small, growing collection of [agent skills](https://docs.claude.com/en/docs/claude-code/skills) — self-contained instruction modules that teach Claude Code (and compatible agents) how to do a specific kind of work well.

Each skill is a folder with a `SKILL.md` file: YAML frontmatter (`name` + `description` that tells the agent *when* to reach for it) followed by the instructions themselves. Drop one into your agent's skills directory and it becomes available on demand.

## Skills

| Skill | What it does |
|-------|--------------|
| [`find-unknowns`](skills/find-unknowns) | Maps the unknowns in an idea, feature, or plan before they get expensive — a blind-spot pass, a known/unknown quadrant map, and a decision-changing interview. Reach for it to de-risk a decision, stress-test a pivot, or answer "what am I missing?" |

More to come.

## Install

Skills live in `~/.claude/skills/` for Claude Code. You can either symlink (recommended — you get updates with a `git pull`) or copy.

**Symlink a single skill:**

```bash
git clone https://github.com/anianroid/ani-skills.git
ln -s "$PWD/ani-skills/skills/find-unknowns" ~/.claude/skills/find-unknowns
```

**Or copy it:**

```bash
cp -r ani-skills/skills/find-unknowns ~/.claude/skills/
```

Then invoke it in Claude Code with `/find-unknowns`, or just describe the task and let the agent pick it up from the `description`.

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
