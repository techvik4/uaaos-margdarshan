# Security Policy

## Scope

This repository contains natural-language development guidance. It is not a security product, sandbox, secrets manager or automated vulnerability scanner.

## Reporting a vulnerability

Please do not publish exploit details, credentials, private data or an unpatched vulnerability in a public issue.

If GitHub's **Private vulnerability reporting** is enabled for this repository, use the repository's **Security** tab to report the issue privately. If private reporting is unavailable, open a minimal public issue asking for a private contact route without including exploit details.

## Security expectations for users

- Review `AGENTS.md` before using it in a sensitive or production repository.
- Keep API keys, tokens, passwords, private keys and `.env` files out of Git.
- Do not let an AI agent execute downloaded scripts or dependencies blindly.
- Use operating-system permissions, sandboxing and secret managers; Markdown instructions are not a security boundary.
- Review commands before allowing destructive actions.
- Do not send private source code, logs, datasets or personal data to an external model or service without authorization.
- Require human approval for production deployment, publication, purchases and irreversible operations.

## Response

Reports will be reviewed as project capacity allows. No response-time or remediation-time guarantee is made. Please include the affected version, impact and reproducible steps where safe to share.
