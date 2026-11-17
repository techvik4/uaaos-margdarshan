# GitHub Publishing Checklist

Complete this checklist before making the repository public.

## Content review
- [ ] Confirm the project name and description.
- [ ] Review every file for typos and outdated claims.
- [ ] Confirm `AGENTS.md` is the only full master instruction file.
- [ ] Confirm compatibility claims match the documented agent versions and modes.
- [ ] Replace `OWNER/REPOSITORY` in `.github/ISSUE_TEMPLATE/config.yml` with the real repository URL.
- [ ] Inspect files and Git history for secrets, private information and third-party material.
- [ ] Decide whether to add an open-source license. Do not imply an open-source license before selecting one.
- [ ] Decide whether GitHub Discussions should be enabled.
- [ ] Decide whether private vulnerability reporting should be enabled.

## Repository setup
- [ ] Create a GitHub repository named `uaaos-margdarshan`.
- [ ] Keep it private while doing the final review if preferred.
- [ ] Upload all files and folders, preserving the `.github` directory.
- [ ] Set the description from README.md.
- [ ] Add relevant topics such as `ai-agents`, `agents-md`, `developer-tools`, `software-engineering`, `prompt-engineering`.
- [ ] Review the rendered README and issue templates.
- [ ] Only then decide whether to make the repository public.

## Release readiness
- [ ] Create a version tag only after the release content is approved.
- [ ] Publish release notes based on CHANGELOG.md.
- [ ] Do not claim support for an agent/version that has not been tested.
