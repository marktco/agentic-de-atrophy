## Socratic Coding Coach

This repo includes skills — prompts and workflows you can use with any LLM or AI coding assistant — to strengthen your own programming practice while working with AI and agents. The goal is to prevent skill atrophy: making decisions, writing tests, and understanding the code, with the model guiding you instead of writing the solution for you.

### Foundational Skills

| Skill | What it does |
|-------|--------------|
| [**Socratic Coach**](skills/foundational/coding/SKILL.md) | General-purpose coach: asks questions, points out gaps, ties your design back to SOLID, DRY, testability. Workflow: **outline → tests → code until green.** |
| [**Problem Decomposition**](skills/foundational/problem-decomposition/SKILL.md) | Helps you break down complex problems into manageable pieces by asking about boundaries, dependencies, and the smallest useful piece. |
| [**Reading Code**](skills/foundational/reading-code/SKILL.md) | Guides you through understanding unfamiliar codebases by asking about entry points, patterns, and data flow. |
| [**Documentation**](skills/foundational/documentation/SKILL.md) | Helps you write clear docs by asking about your audience, their goals, and what they need to succeed. |
| [**Estimation**](skills/foundational/estimation/SKILL.md) | Guides task breakdown and estimation by asking about unknowns, dependencies, and past experience. |
| [**Algorithms**](skills/foundational/algorithms/SKILL.md) | Guides algorithm design with questions about patterns, complexity, and edge cases. |

### Design Skills

| Skill | What it does |
|-------|--------------|
| [**System Design**](skills/design/system-design/SKILL.md) | Guides architecture decisions by asking about requirements, trade-offs, and scaling. |
| [**API Design**](skills/design/api-design/SKILL.md) | Helps you reason through endpoints, resources, versioning, and error handling. |
| [**Data Modeling**](skills/design/databases/SKILL.md) | Guides schema design, normalization, and query patterns via questions about your domain. |

### Quality Skills

| Skill | What it does |
|-------|--------------|
| [**Test Design**](skills/quality/testing/SKILL.md) | Guides you through what to test, edge cases, and test structure without writing tests for you. |
| [**Debugging**](skills/quality/debugging/SKILL.md) | Helps you systematically isolate bugs by asking about symptoms, hypotheses, and what you've ruled out. |
| [**Refactoring**](skills/quality/refactoring/SKILL.md) | Points out code smells and asks why they're problematic — without refactoring for you. |
| [**Code Review**](skills/quality/code-review/SKILL.md) | Coaches you on giving constructive code review feedback — framing, tone, actionability. |
| [**Performance**](skills/quality/performance/SKILL.md) | Guides you through profiling and optimization by asking what you've measured. |

### Language & Framework Skills

| Skill | What it does |
|-------|--------------|
| [**React**](skills/languages/react/SKILL.md) | Helps you reason through component design, state placement, and prop flow. |
| [**TypeScript**](skills/languages/typescript/SKILL.md) | Asks about type narrowing, generics, and when to use interfaces vs types. |

### Workflow Skills

| Skill | What it does |
|-------|--------------|
| [**Git**](skills/workflow/git/SKILL.md) | Helps you think through branching, commit granularity, and history hygiene. |

---

**How to use:** Open a skill file, copy the prompt block into a new chat with your preferred assistant (Cursor, Claude, ChatGPT, etc.), then describe your problem. The assistant will respond with questions and hints instead of code.
