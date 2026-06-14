# Fable-Like-Skill

A Claude Code skill that ports the **prompt-tunable behavioral patterns** Anthropic published for Claude Fable 5 onto any non-Fable model (e.g. Opus 4.8).

It does **not** raise model capability. It changes how that capability is spent — fewer wasted loops, fewer fabricated "done" claims, cleaner diffs, more reliable self-checking. The "character" of Fable, not its weights.

**Provenance:** distilled from Anthropic's official Claude Fable 5 migration guidance (the prompt-tunable "behavioral shifts" section). No leaked or third-party prompts.

## Install (Claude Code, system-wide)

Copy the skill into your global skills directory so it loads in every project:

```sh
mkdir -p ~/.claude/skills/fable-like-skill
cp Fable-Like-Skill.md ~/.claude/skills/fable-like-skill/SKILL.md
```

Claude Code activates it automatically on coding, review, debugging, testing, and multi-step agentic tasks (description-driven).

## The ten principles

1. Act when you have enough information
2. Don't over-engineer; don't tidy uninvited
3. Ground every progress claim in tool output
4. Respect the boundary between assessment and action
5. Lead with the outcome
6. Verify with fresh context
7. Finding bugs: cover first, filter later
8. Delegate when the work fans out
9. Memory discipline
10. Persist to done or to a real blocker

See [`Fable-Like-Skill.md`](./Fable-Like-Skill.md) for the full text.

## Pairs well with

- `/code-review` → fixes → `/verify`
- `/simplify`
