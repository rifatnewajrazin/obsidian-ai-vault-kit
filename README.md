# Obsidian AI Vault Kit

A starter rulebook for running an AI assistant (Claude Code, Codex, Gemini, anything that reads a markdown file) inside an Obsidian vault without it making a mess.

I built this after watching an AI quietly rename files, invent facts about me, and ship changes I never asked for. The fix was not a smarter model. It was a short set of written rules the AI has to read before it touches anything. This kit is that set, cleaned up so you can drop it into your own vault.

## What you get

| File | What it does |
| --- | --- |
| `CLAUDE.md` | The master rules file. Hard rules, session routine, folder map, note format. Put it at your vault root. |
| `docs/working-with-ai.md` | How the AI should collaborate: when to ask, when to act, how to log work, how to plan features. |
| `docs/maintenance-playbook.md` | The checklist to run before saving a note, plus what is safe to do alone and what needs your approval. |
| `docs/writing-style.md` | A plain-voice style guide, including the list of AI writing habits to ban. |
| `docs/skills-router.md` | A single page that tells the AI which skill or reference to use for which job. |
| `templates/` | Note frontmatter, a per-folder rules file, and a work log template. |
| `skills/vault-rules/SKILL.md` | A Claude Code skill that makes the AI read the rules before any job. |

## Install

1. Copy `CLAUDE.md` into the root of your vault.
2. Copy `docs/` into `Guidelines/` (or wherever you keep reference notes).
3. Open `CLAUDE.md` and fill in the parts marked `YOUR VALUE`: your name, your folders, your own hard rules.
4. Optional: install the skill so Claude Code checks the rules on its own.

```bash
mkdir -p ~/.claude/skills
cp -r skills/vault-rules ~/.claude/skills/
```

5. Optional: add this line to `~/.claude/CLAUDE.md` so it applies in every project, not just the vault:

```
Before any task, read the vault rules at <path to your vault>/CLAUDE.md.
```

## How it works

The rules are layered on purpose.

1. Your current request always wins.
2. Then the root `CLAUDE.md` and the folder rules file.
3. Then the docs in this kit.
4. Then any skills or outside references.

Every folder can carry its own small `CLAUDE.md` (see `templates/folder-CLAUDE.md`). The root file points to it, so the AI reads the local rules for the folder it is about to write into.

## The five ideas that matter most

- **Only change what was asked.** "Fix these three bugs" does not include "and I also redesigned the header."
- **Draft, show, wait.** Nothing goes live (push, deploy, publish, send) until you say yes. A yes for one change is not a yes for the next.
- **Ask, do not guess.** When something is truly unclear, ask with two to four real options and a recommendation.
- **Never invent facts about you.** Missing detail becomes `TBD` and a question.
- **Never store secrets.** Write down where a secret lives, not the secret.

## Make it yours

This is my setup with my life taken out. Change the folder map, the note types and the hard rules to match how you work. If a rule does not earn its place, delete it. A short rulebook the AI actually follows beats a long one it skims.

## Contributing

Issues and pull requests are welcome. Keep the voice plain, skip em dashes, and keep examples generic. See `CONTRIBUTING.md`.

## Credit

Written by [Rifat Newaj Razin](https://github.com/rifatnewajrazin). MIT licensed.
