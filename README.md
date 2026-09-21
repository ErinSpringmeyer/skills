# skills

Skills, agents and plugins for Claude, published as a marketplace and as individual downloads.  Built and tested in a private workshop, released here.

## Install

**Claude Code or Cowork** — add the marketplace once, then install what you want:

```
/plugin marketplace add ErinSpringmeyer/skills
/plugin install <plugin-name>@erin-springmeyer
```

**claude.ai** — download a skill zip from the latest [release](https://github.com/ErinSpringmeyer/skills/releases) and upload it in Claude's skills settings.  You can also copy a folder from `skills/` directly.

**Anything else** — a skill is a folder with a `SKILL.md` inside.  Copy the one you want into wherever your agent reads skills from.

## Layout

```
skills/       every released skill, on its own
plugins/      bundles built from those skills
deprecated/   retired items, each with a sunset date
```

Two kinds of plugin: a **collection** groups a domain's skills, such as `productivity` or `finance-ops`; a **bundle** packages the several skills one task needs, such as `job-search`.  `skills/` is the single source, and a plugin's `skills/` folder is written from it at release.

## Conventions

Names are lowercase kebab-case.  Frontmatter uses only Agent Skills spec fields, so the same skill works in Claude Code, Cowork, claude.ai and other agents that read `SKILL.md`.  Versions are semantic, at both the item and the plugin level, and each plugin keeps its own CHANGELOG.

## License

MIT.  See [LICENSE](LICENSE).
