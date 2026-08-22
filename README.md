# CONVENTIONS.md (conventions-md)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
