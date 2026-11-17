# UAAOS – MARGDARSHAN

**Universal Autonomous AI Operating System**  
*A model-agnostic master guidance file for responsible AI-assisted software development.*

> **Activation phrase**  
> `UAAOS-MARGDARSHAN: LOAD, VERIFY, REMEMBER AND CONTINUE.`

**Project status:** Early public draft  
**Guidance version:** 1.2  
**Canonical instruction file:** [`AGENTS.md`](./AGENTS.md)

---

## What is MARGDARSHAN?

UAAOS – MARGDARSHAN is a reusable set of operating instructions for AI coding agents. It aims to make AI-assisted development more consistent, careful, recoverable and transparent across projects.

The project is built around one rule: **`AGENTS.md` is the single canonical source of development guidance.** The other files in this repository explain how to use, review and contribute to that master file; they do not create competing copies of its rules.

MARGDARSHAN is designed to encourage an AI agent to:

- inspect an existing project before changing it;
- check installed software and dependencies before installing or updating;
- skip unnecessary tools and upgrades;
- break large work into phases, tasks and small verifiable steps;
- investigate root causes and fix genuine development errors;
- preserve progress and recover safely after interruptions;
- research uncertain technical details from reliable sources;
- protect privacy, secrets and user data;
- test actual functionality instead of claiming success from generated code alone;
- clearly report verified, incomplete, blocked and untested work.

## What this project is — and is not

**It is:** a portable Markdown instruction framework that can guide compatible AI coding agents and can be supplied manually to other AI assistants.

**It is not:** an executable program, an agent, a model, a security sandbox, an automatic backup utility, or a guarantee that every AI product will load or obey the file automatically.

The AI application or agent harness controls instruction discovery, available tools, context limits and permissions. The underlying model alone cannot guarantee those features. See [Compatibility](./COMPATIBILITY.md).

## Quick start

1. Download or clone this repository.
2. Copy `AGENTS.md` into the root of the software project you want the agent to work on.
3. Open that project folder in your AI coding agent.
4. Send the activation message below.
5. Ask the agent to confirm that it actually read the file and identify the next safe task.

```text
UAAOS-MARGDARSHAN: LOAD, VERIFY, REMEMBER AND CONTINUE.

Read the complete AGENTS.md in this project root. Do not claim it was loaded unless you actually read it. Inspect the project, current changes and any existing project-state records. Preserve user work. Report the next incomplete task and continue only within the permissions available to you. If this agent does not automatically discover AGENTS.md, ask me to attach or provide it; do not pretend it was loaded.
```

Detailed instructions: [GETTING_STARTED.md](./GETTING_STARTED.md).

## Design principles

| Principle | Expected behaviour |
|---|---|
| Safety before speed | Protect data and obtain approval for consequential actions. |
| Check before install | Reuse compatible software; skip unnecessary updates and dependencies. |
| Small verified steps | Decompose work and validate each meaningful unit. |
| Recoverable progress | Save checkpoints and inspect state before resuming. |
| Evidence-based research | Prefer official documentation, release notes and reproducible evidence. |
| Real functionality | Do not represent placeholders, mocks or untested code as complete. |
| Privacy by default | Do not send private data to external services without authorization. |
| Honest reporting | Distinguish verified, partially verified, not verified, blocked and failed work. |

## Repository contents

| File or folder | Purpose |
|---|---|
| [`AGENTS.md`](./AGENTS.md) | The one canonical master instruction file. |
| [`GETTING_STARTED.md`](./GETTING_STARTED.md) | Beginner-friendly setup and activation steps. |
| [`COMPATIBILITY.md`](./COMPATIBILITY.md) | Agent-harness support and limitations. |
| [`SECURITY.md`](./SECURITY.md) | Responsible vulnerability reporting guidance. |
| [`PRIVACY.md`](./PRIVACY.md) | Privacy principles and data-handling expectations. |
| [`CONTRIBUTING.md`](./CONTRIBUTING.md) | Suggestions, issue reports and contribution process. |
| [`CODE_OF_CONDUCT.md`](./CODE_OF_CONDUCT.md) | Community participation expectations. |
| [`SUPPORT.md`](./SUPPORT.md) | Where to ask questions and report problems. |
| [`ROADMAP.md`](./ROADMAP.md) | Proposed future improvements; not promises. |
| [`CHANGELOG.md`](./CHANGELOG.md) | Version history. |
| [`.github/`](./.github/) | Issue and pull-request templates. |

## Important limitations

- A Markdown instruction file cannot grant tools or permissions that an agent does not have.
- A prompt cannot replace operating-system access controls, sandboxing, secret management, backups or human approval.
- Recovery cannot guarantee restoration of data that was never saved or backed up.
- Research quality depends on source access, freshness and verification; social posts and videos are leads, not automatic proof.
- Different agent products may require manual attachment or a product-specific setting to load the same file.
- The project does not claim that software built under these instructions will be bug-free or completely secure.

## Security and privacy

Read [SECURITY.md](./SECURITY.md) and [PRIVACY.md](./PRIVACY.md). Never commit passwords, API keys, private keys, tokens, personal information or private project data to a public repository.

## License and reuse

**No open-source license has been selected for this project yet.** The repository is publicly viewable, but public visibility alone does not grant permission to copy, modify, redistribute, sublicense or commercially reuse its contents. Please do not assume an open-source license applies. A license decision must be made by the project owner before reuse permissions are advertised.

## Sources and compatibility references

This project follows publicly documented instruction-file mechanisms where available. Product support can change; consult the vendor documentation linked in [COMPATIBILITY.md](./COMPATIBILITY.md) before relying on automatic loading.

## Contributing

Ideas, bug reports and compatibility feedback are welcome through GitHub Issues. Read [CONTRIBUTING.md](./CONTRIBUTING.md) before proposing changes. Do not submit copied third-party content or secrets.

---

**MARGDARSHAN's promise:** encourage careful engineering, preserve user trust and report only what can be supported by evidence.
