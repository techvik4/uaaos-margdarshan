# Getting Started

This guide explains how to use UAAOS – MARGDARSHAN with an AI coding agent.

## 1. Download the master file

Download [`AGENTS.md`](./AGENTS.md) from this repository. It is the only canonical set of master development instructions.

## 2. Add it to your software project

Place `AGENTS.md` in the root folder of the software project the agent will work on. For example:

```text
MySoftwareProject/
├── AGENTS.md
├── README.md
├── src/
├── tests/
└── ...
```

Do not overwrite an existing `AGENTS.md` without reviewing it first. If one already exists, compare and merge the instructions carefully while preserving project-specific requirements.

## 3. Open the correct folder

Open the project root in the coding application. An agent launched from another folder may not discover the intended project instructions.

## 4. Activate MARGDARSHAN

Send this message:

```text
UAAOS-MARGDARSHAN: LOAD, VERIFY, REMEMBER AND CONTINUE.

Read the complete AGENTS.md in this project root. Do not claim it was loaded unless you actually read it. Inspect the existing project, current changes, requirements and recovery records. Preserve user work. Tell me whether the file was actually loaded, what project state you can see, and what the next safe incomplete task is. Continue autonomously only within the permissions available to you. Ask before destructive, paid, system-wide, publishing or privacy-impacting actions.
```

## 5. Verify that it loaded

Ask the agent:

```text
Show me the exact path of the MARGDARSHAN instruction file you read, summarize its main safety and recovery rules, and list any instruction-loading limitations. Do not claim a file was loaded if you did not read it.
```

A useful response should identify the correct path, summarize actual rules and disclose any limitation. A simple “done” is not proof.

## 6. Start or resume work

For a new project, ask the agent to inspect the repository and prepare a phased plan before making changes. For an existing project, ask it to inspect the current files, version-control status and last verified checkpoint before continuing.

## Agent-specific notes

- **Codex, Cursor and supported GitHub Copilot agent workflows:** current documentation describes support for `AGENTS.md` in relevant workflows. Confirm the selected harness and workspace root.
- **Claude Code:** its native persistent project instructions use `CLAUDE.md`. To keep one canonical master file, provide `AGENTS.md` as context or explicitly ask Claude Code to read it at session start. Do not create a duplicate master file unless you deliberately choose a small pointer/loader later.
- **Gemini CLI:** its default context file is `GEMINI.md`. It supports configurable context filenames; an experienced user can configure `AGENTS.md` as a context filename. Otherwise, provide the file as context and verify it was loaded.
- **Other agents and chat-based models:** attach or open `AGENTS.md`, paste the activation message and verify that the assistant actually read it.

See [COMPATIBILITY.md](./COMPATIBILITY.md) for official documentation links and caveats.

## Important

The activation phrase is a reminder, not a technical enforcement mechanism. The agent's application controls automatic file loading, tools, memory, context limits and permissions. Never rely on a text instruction as the only protection against data loss or unsafe commands.
