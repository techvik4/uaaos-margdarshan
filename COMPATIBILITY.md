# Agent Compatibility and File Loading

**Last reviewed:** 17 November 2026

## The key distinction

UAAOS – MARGDARSHAN is model-agnostic as written guidance, but automatic loading is controlled by the agent application or harness—not simply by which underlying AI model is selected.

The project keeps one canonical file: `AGENTS.md`. Some products recognize it natively; others use a different default filename or require the user to attach/read the file manually.

## Current documented support

| Agent or harness | Documented instruction mechanism | Recommended use of this project |
|---|---|---|
| OpenAI Codex | `AGENTS.md` | Place the master file in the repository root and verify the active instruction chain. |
| Cursor | `AGENTS.md` is supported as a simple project instruction format; `.cursor/rules/*.mdc` is another native option. | Use root `AGENTS.md`; verify the active workspace. |
| GitHub Copilot coding agent | `AGENTS.md` is supported, alongside Copilot-specific instruction mechanisms. | Use root `AGENTS.md` and verify the selected Copilot workflow. |
| VS Code agent workflows | Support depends on the selected harness; the current reference lists `AGENTS.md` for Codex and Copilot and native formats for other agents. | Check which harness is selected, then verify discovery. |
| Claude Code | Native persistent project instructions use `CLAUDE.md`. | Keep `AGENTS.md` canonical; attach it or ask Claude Code to read it at the beginning of a session. |
| Gemini CLI | Default context file is `GEMINI.md`; context filenames can be configured. | Keep `AGENTS.md` canonical; either configure it as a context filename or supply it manually. |
| Other tools and chat models | Varies by product and version. | Attach/open the file and use the activation message; verify actual reading. |

This table is not a guarantee for every version, plan, operating system, IDE integration or agent mode. Check vendor documentation before adopting a workflow.

## Official references

- [OpenAI Codex: Custom instructions with AGENTS.md](https://learn.chatgpt.com/docs/agent-configuration/agents-md)
- [VS Code: Custom instructions reference](https://code.visualstudio.com/docs/agents/reference/custom-instructions-reference)
- [Cursor: Rules and AGENTS.md](https://cursor.com/docs/rules)
- [GitHub Copilot: Customization cheat sheet](https://docs.github.com/en/copilot/reference/customization-cheat-sheet)
- [GitHub: Copilot coding agent supports AGENTS.md](https://github.blog/changelog/2025-08-28-copilot-coding-agent-now-supports-agents-md-custom-instructions/)
- [Claude: CLAUDE.md project context](https://support.claude.com/en/articles/14553240-give-claude-context-claude-md-and-better-prompts)
- [Gemini CLI: Provide context with GEMINI.md](https://google-gemini.github.io/gemini-cli/docs/cli/gemini-md.html)

## One-file policy

1. `AGENTS.md` is the canonical master guidance file.
2. Do not maintain separate full copies for different models.
3. If a product requires another filename, first consider manual attachment or an explicit read instruction.
4. If automatic discovery is essential, a minimal native loader may be used only as a deliberate compatibility adapter. It must point to the canonical `AGENTS.md`, must not contain a competing rule set and must be tested. The current repository does not include such duplicate adapters.
5. Never claim automatic compatibility unless it has been tested in the exact agent, version and mode.

## Verification checklist

- [ ] The agent is running in the intended project root.
- [ ] The agent identifies the exact `AGENTS.md` path.
- [ ] The agent can summarize key rules from the file.
- [ ] The agent discloses context-size or discovery limitations.
- [ ] The agent's tools and permissions are understood.
- [ ] The agent does not claim a permission or capability it does not have.
