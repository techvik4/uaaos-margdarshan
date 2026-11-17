# Privacy Principles

UAAOS – MARGDARSHAN is a Markdown guidance project. This repository does not itself run an agent, collect project telemetry or receive the files an AI agent works on.

When using the guidance with an AI tool, the tool provider's data handling, retention, training, logging and account settings still apply. This file cannot override those policies.

## Recommended practices

1. Treat source code, logs, prompts, datasets, credentials and personal information as private by default.
2. Send only the minimum information required to an external AI service.
3. Obtain authorization before uploading private files or logs to an external service.
4. Remove credentials and personal data from bug reports and screenshots.
5. Use `.gitignore` and secret scanning to prevent accidental commits.
6. Store project backups in access-controlled locations.
7. Define retention and deletion rules for project data.
8. Verify which tools, MCP servers, extensions and integrations can read or transmit project files.
9. Do not assume that a model's privacy setting is the same as the application's retention or logging policy.

## Repository privacy

Before publishing a project, inspect the full Git history and current files for secrets, private customer information, licensed content and confidential material. Deleting a secret from the latest commit may not remove it from Git history; rotate exposed credentials immediately.
