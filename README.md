# weekly-revision-checklist

An [Agent Skill](https://agentskills.io/specification) that helps an AI
agent build a weekly revision checklist for university students. The agent
asks a few short questions, then outputs a checklist table with topic,
priority, time needed and done columns.

The skill refuses graded homework and assessed work, and redirects to
revision activities instead.

## Folder tree

```
weekly-revision-checklist/
├── SKILL.md              # Metadata plus the agent instructions
├── references/
│   └── REFERENCE.md      # Priority scheme, time estimates, example, edge cases
├── README.md             # This file
└── LICENSE               # MIT license
```

No `scripts/` or `assets/` are included - the skill is pure instructions,
so there is nothing to run.

## Install

Copy the folder into your agent's skills directory, keeping the folder
name identical to the `name` field in SKILL.md. Common locations:

- Claude Code: `~/.claude/skills/weekly-revision-checklist`
- Other agents: wherever the agent discovers skills (check its docs).

## Validate

```bash
pip install skills-ref
skills-ref validate ./weekly-revision-checklist
```

## Customize

Edit the `description` in SKILL.md to change the trigger phrases. Keep the
folder name and the `name` field in sync, or validation will fail.
