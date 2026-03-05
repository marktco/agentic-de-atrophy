# AGENTS.md

Guidelines for AI coding agents working in this repository.

## Repository Overview

This is a **documentation-only repository** containing AI coaching prompts and skills.
It is NOT a code project — there is no build system, test suite, or application code.

**Purpose**: Provide system prompts that turn AI assistants into Socratic coaches who
guide developers to solutions through questions rather than writing code for them.

**Core philosophy**: Help developers grow by making them think, not by solving problems
for them. The workflow is: **outline → tests → code until green**.

---

## Repository Structure

```
socratic-coding-coach/
├── README.md                        # Project overview and skill table
├── AGENTS.md                        # This file (agent guidelines)
├── .gitignore                       # Standard Node.js template
└── skills/                          # All skills organized by category
    ├── foundational/                # Core skills every developer needs
    │   ├── coding/SKILL.md          # General coding coach
    │   ├── problem-decomposition/SKILL.md  # Breaking down complex problems
    │   ├── reading-code/SKILL.md    # Understanding unfamiliar codebases
    │   ├── documentation/SKILL.md   # Writing clear documentation
    │   ├── estimation/SKILL.md      # Task breakdown and estimation
    │   └── algorithms/SKILL.md      # Algorithm design
    │
    ├── design/                      # Architecture and design
    │   ├── system-design/SKILL.md   # System architecture
    │   ├── api-design/SKILL.md      # API design
    │   └── databases/SKILL.md       # Data modeling
    │
    ├── quality/                     # Code quality and maintenance
    │   ├── testing/SKILL.md         # Test design
    │   ├── debugging/SKILL.md       # Root cause analysis
    │   ├── refactoring/SKILL.md     # Code smells and refactoring
    │   ├── code-review/SKILL.md     # Giving feedback
    │   └── performance/SKILL.md     # Performance optimization
    │
    ├── languages/                   # Language and framework specific
    │   ├── react/SKILL.md           # React component composition
    │   └── typescript/SKILL.md      # TypeScript type design
    │
    └── workflow/                    # Process and collaboration
        └── git/SKILL.md             # Git workflow and history
```

---

## Build / Lint / Test Commands

**None.** This repository contains only Markdown documentation.

There is no:
- `package.json` or build system
- Test framework or test files
- Linting configuration
- TypeScript/JavaScript code

To validate changes, manually review Markdown formatting and ensure YAML frontmatter is valid.

---

## File Formats and Structure

### SKILL.md Format

Skills use YAML frontmatter followed by Markdown content:

```yaml
---
name: skill-name-in-kebab-case
description: "One-sentence description of what the skill does."
---
```

After the frontmatter:
1. **Title** — `# Skill Name` (title case)
2. **Purpose section** — Brief explanation of the skill's goal
3. **The Prompt** — The actual system prompt in a fenced code block
4. **How to Use It** — Instructions for users
5. **Tips** — Optional guidance for getting the most out of the skill

### README.md Format

- Brief intro paragraph explaining the repository's purpose
- Table of available skills with links and descriptions
- Usage instructions

---

## Naming Conventions

| Element | Convention | Example |
|---------|------------|---------|
| Skill names | kebab-case | `socratic-coding-coach` |
| Skill files | SKILL.md | `skills/react/SKILL.md` |
| Domain directories | lowercase kebab-case | `system-design/`, `react/` |
| Root documentation | UPPERCASE.md | `README.md`, `AGENTS.md` |
| Section headings | Title case | `## How to Use It` |

---

## Content Guidelines

### Writing Style

- Clear, concise, professional tone
- No unnecessary jargon
- Use bold for emphasis, not ALL CAPS
- Use bullet lists for rules and steps
- Use numbered lists for sequential workflows
- Keep sentences short

### Prompt Writing

When creating or editing coaching prompts:

1. **Be explicit about constraints** — Clearly state what the AI must NOT do
2. **Provide escalation paths** — Include hint ladders for when users are stuck
3. **Reference best practices** — SOLID, DRY, separation of concerns, testability
4. **Define the workflow** — Specify the order of operations (outline → tests → code)
5. **Set the tone** — Encouraging but honest; treat users as capable developers

### Key Principles to Embed in Prompts

- Never write implementation code for the user
- Ask questions instead of giving answers
- Point out problems without providing fixes
- Affirm good reasoning explicitly
- Use the escalating hint ladder when users are stuck:
  1. Question pointing toward the concept
  2. Name the concept or pattern (no code)
  3. Pseudocode outline only
  4. Minimal isolated example (not their exact problem)

---

## Editing Existing Content

When modifying `SKILL.md` or other documentation:

1. **Preserve YAML frontmatter** — Do not break the `---` delimiters
2. **Keep code blocks intact** — Prompts live in fenced code blocks
3. **Maintain the section order** — Purpose → Prompt → Usage → Tips
4. **Update the README table** if skill descriptions change

---

## Adding New Skills

If adding a new skill file:

1. Create `skills/<domain>/SKILL.md` with proper YAML frontmatter
2. Follow the existing skill file structure
3. Add an entry to the README.md skill table
4. Use kebab-case for the `name` field in frontmatter

---

## Git Workflow

- `main` branch contains stable content
- `feature/*` branches for new skills or major changes
- Commit messages should be clear and descriptive
- No CI/CD pipeline — changes are reviewed manually

---

## What NOT to Do

- Do not add code files (`.js`, `.ts`, `.py`, etc.) — this is documentation only
- Do not create build configurations or test setups
- Do not add package management files (`package.json`, `requirements.txt`)
- Do not write implementation code in prompts — that contradicts the Socratic method
- Do not use emojis unless explicitly requested

---

## Quality Checklist

Before committing changes:

- [ ] YAML frontmatter is valid (proper `---` delimiters, quoted strings)
- [ ] Markdown renders correctly (check headings, lists, code blocks)
- [ ] Prompts are in fenced code blocks (triple backticks)
- [ ] Links in README point to correct files
- [ ] Skill descriptions are accurate and concise
- [ ] Writing is clear and free of typos

---

## Reference: The Socratic Method

The core approach this repository promotes:

> Help developers grow by guiding them to solutions through questions, not by
> writing code for them.

**Workflow**: outline → tests → code until green

**Hint Ladder** (escalate only when stuck):
1. Question about the concept
2. Name the pattern
3. Pseudocode only
4. Minimal isolated example

**Best Practices to Reference** (via questions):
- SOLID principles
- DRY (Don't Repeat Yourself)
- Separation of concerns
- Testability
- Naming and clarity
