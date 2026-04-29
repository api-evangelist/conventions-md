# CONVENTIONS.md (conventions-md)

CONVENTIONS.md is a Markdown convention popularized by AI pair programming tools such as aider and adopted by AI coding agents like Cursor, Cline, and Claude Code. It documents project-specific coding standards, library preferences, naming conventions, architecture decisions, and development practices in plain natural language so both human developers and AI assistants share the same expectations. The file is loaded into the model context to steer code generation toward project conventions.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/conventions-md/refs/heads/main/apis.yml)

## Type

- **x-type:** standard

## Tags:

 - AI Coding, Aider, Best Practices, Coding Standards, Conventions, Developer Workflow, Documentation, Markdown, Project Configuration

## Timestamps

- **Created:** 2025-01-01
- **Modified:** 2026-04-28

## APIs

### CONVENTIONS.md Format

The CONVENTIONS.md format is a free-form Markdown file describing the coding rules an AI coding agent should follow inside a repository. The file is loaded into the chat context, typically in read-only mode, and may be referenced via /read CONVENTIONS.md, the --read CLI flag, or a persistent read entry in .aider.conf.yml. Common content includes preferred libraries, language and version targets, type system rules, lint and format expectations, error handling style, and architectural patterns the project favors.

**Human URL:** [https://aider.chat/docs/usage/conventions.html](https://aider.chat/docs/usage/conventions.html)

#### Tags:

 - AI Coding, Convention, Markdown, Project Configuration

#### Properties

- [Documentation](https://aider.chat/docs/usage/conventions.html)
- [Documentation](https://aider.chat/docs/config/aider_conf.html)
- [Repository](https://github.com/Aider-AI/aider)

#### Features

- Plain Markdown bullet list of project rules
- Loaded into AI agent context per session or via config
- Supports prompt caching when marked read-only
- Composable alongside CLAUDE.md, .cursor/rules, and copilot-instructions
- No required schema, allowing each project to define what matters

#### Use Cases

- Steering AI agents toward preferred libraries and frameworks
- Documenting type hint, naming, and lint requirements
- Capturing architecture decisions for AI assisted refactors
- Aligning human and AI contributors on a single source of conventions
- Reducing rework caused by AI generated code that misses team norms

### AI Coding Conventions Ecosystem

CONVENTIONS.md sits alongside several closely related AI coding conventions. CLAUDE.md is used by Claude Code for repository memory. .cursor/rules and .cursorrules are used by Cursor. .github/copilot-instructions.md is used by GitHub Copilot. Each follows a similar pattern: a Markdown or text file describing repository-specific rules that gets injected into the AI assistant prompt context. CONVENTIONS.md is the most tool-agnostic option and is widely adopted across multiple AI coding agents.

**Human URL:** [https://docs.anthropic.com/en/docs/claude-code/memory](https://docs.anthropic.com/en/docs/claude-code/memory)

#### Tags:

 - AI Coding, Comparison, Conventions

#### Properties

- [Documentation](https://docs.anthropic.com/en/docs/claude-code/memory)
- [Documentation](https://docs.cursor.com/context/rules-for-ai)
- [Documentation](https://docs.github.com/en/copilot/customizing-copilot/adding-repository-custom-instructions-for-github-copilot)
- [Documentation](https://aider.chat/docs/usage/conventions.html)

#### Features

- Tool-agnostic file naming compared to CLAUDE.md or .cursorrules
- Often committed to repo root for visibility to humans and AI
- Frequently referenced by other agent files such as CLAUDE.md
- Composable with .editorconfig, .prettierrc, and lint configurations

#### Use Cases

- Sharing one set of rules across aider, Cursor, Cline, and Claude Code
- Consolidating coding standards for human and AI contributors
- Documenting cross-cutting concerns separate from tool-specific config

## Common Properties

- [Documentation](https://aider.chat/docs/usage/conventions.html)
- [Documentation](https://docs.anthropic.com/en/docs/claude-code/memory)
- [Documentation](https://docs.cursor.com/context/rules-for-ai)
- [Documentation](https://docs.github.com/en/copilot/customizing-copilot/adding-repository-custom-instructions-for-github-copilot)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
