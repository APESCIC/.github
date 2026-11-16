# Agent instructions for APESCIC/.github

Cursor's user rules and skills set how work is done here (branches, issues, pull requests, merge, release, deploy, ship gate, decisions and safety). This file describes this repository and fills the named slots below. If anything here disagrees with them, Cursor's rules win and this file is corrected in the same milestone.

Cursor/agent layout standard: https://github.com/apescic-director/Cursor/blob/bmurphy/cursor-agent-standard-81b0/docs/cursor-agent-standards.md

The owner is Bambie Murphy. Write UK English (organisation, behaviour, colour, licence) in docs, issues and pull requests. Never print, paste or commit secrets.

## About the app

This is the public GitHub organisation profile repository for Association of Protecting Exotic Species CIC (APES CIC). It holds the organisation `README.md` and the signed-out org profile in `profile/README.md`. There is no application code and no deployable app.

- Repository: `APESCIC/.github`. Work only in this repository.

## Stack and architecture

- Markdown only: root `README.md` (organisation home) and `profile/README.md` (GitHub organisation profile).
- No PHP, Node, Composer, database or build step.

## Local development and preview

| Item | Value |
| --- | --- |
| Clone | `C:\Users\BambieMurphy\Documents\GitHub\.github` |
| Herd site | None |
| Preview URL | None (organisation profile Markdown; skip the live preview gate) |
| Preview command | None |
| HMR port | None |
| Env file | None |
| Database | None |
| Mail | None |

No local web stack. Preview changes by reading the Markdown and, after merge, on the organisation page on GitHub.

## Tests and checks

| Check | Command |
| --- | --- |
| Tests | None |
| Lint / format | None (Markdown copy review) |
| CI workflows | None |

## Workflow slots

Shipping follows Cursor's `github-milestone-completion` and `ship-gate` skills where a versioned product ships; this repository is not versioned. This repo fills these slots:

| Slot | Value |
| --- | --- |
| Milestone branch pattern | `bmurphy/<slug>` (or the issue branch named in the plan) |
| Version files | None |
| Release tooling | None: merging the pull request is the final step |
| Area labels | None |
| Issue title prefix | `[Type] Short title` |

Development is tracked only in GitHub issues, sub-issues and milestones — never Linear. Secrets live only in APES Vault (Bitwarden); never commit them.

## Deploy and health

| Item | Value |
| --- | --- |
| Target | Not deployed (GitHub serves the organisation profile from this repository) |
| Cloudron app ID | None |
| Domain | None (visible on https://github.com/APESCIC) |
| Deploy command | None |
| Deploys | Not deployed; merge to `main` updates the organisation profile |
| Auto-deploy couplings | none |
| Health URL | None |
| Version field | None |
| Secrets live in | APES Vault (never commit secrets) |

## Decisions and gotchas

- 2026-11-16: Added root `AGENTS.md` and `.cursorignore` to align with the APES Cursor/agent standard (thin profile repo; no `.cursor/` tree required).
- Gotcha: changing `profile/README.md` is what GitHub shows on the organisation profile; the root `README.md` is the repository landing page for `APESCIC/.github` itself.

## Where to find things

- Organisation landing copy: [README.md](README.md)
- GitHub organisation profile: [profile/README.md](profile/README.md)
- Org Cursor/agent standard: https://github.com/apescic-director/Cursor/blob/bmurphy/cursor-agent-standard-81b0/docs/cursor-agent-standards.md
