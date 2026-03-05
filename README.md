## Socratic Coding Coach

This repo includes skills — prompts and workflows you can use with any LLM or AI coding assistant — to strengthen your own programming practice while working with AI and agents. The goal is to prevent skill atrophy: making decisions, writing tests, and understanding the code, with the model guiding you instead of writing the solution for you.

| Domain | Skill | What it does |
|--------|-------|--------------|
| coding | [**Socratic Coach**](skills/coding/SKILL.md) | General-purpose coach: asks questions, points out gaps, ties your design back to SOLID, DRY, testability. Workflow: **outline → tests → code until green.** |
| system-design | [**Architecture**](skills/system-design/SKILL.md) | Guides architecture decisions by asking about requirements, trade-offs, and scaling. Workflow: **requirements → estimation → design → deep dives.** |
| react | [**Composition**](skills/react/SKILL.md) | Helps you reason through component design, state placement, and prop flow without writing components for you. |
| testing | [**Test Design**](skills/testing/SKILL.md) | Guides you through what to test, edge cases, and test structure without writing tests for you. |
| debugging | [**Root Cause**](skills/debugging/SKILL.md) | Helps you systematically isolate bugs by asking about symptoms, hypotheses, and what you've ruled out. |
| refactoring | [**Code Smells**](skills/refactoring/SKILL.md) | Points out code smells and asks why they're problematic — without refactoring for you. |
| databases | [**Data Modeling**](skills/databases/SKILL.md) | Guides schema design, normalization, and query patterns via questions about your domain. |
| api-design | [**REST Contracts**](skills/api-design/SKILL.md) | Helps you reason through endpoints, resources, versioning, and error handling. |
| typescript | [**Type Design**](skills/typescript/SKILL.md) | Asks about type narrowing, generics, and when to use interfaces vs types. |
| performance | [**Bottlenecks**](skills/performance/SKILL.md) | Guides you through profiling and optimization by asking what you've measured. |
| git | [**Commit Strategy**](skills/git/SKILL.md) | Helps you think through branching, commit granularity, and history hygiene. |
| code-review | [**Giving Feedback**](skills/code-review/SKILL.md) | Coaches you on giving constructive code review feedback — framing, tone, actionability. |
| algorithms | [**Problem Solving**](skills/algorithms/SKILL.md) | Guides algorithm design with questions about patterns, complexity, and edge cases. |

**How to use:** Open a skill file, copy the prompt block into a new chat with your preferred assistant (Cursor, Claude, ChatGPT, etc.), then describe your problem. The assistant will respond with questions and hints instead of code.
