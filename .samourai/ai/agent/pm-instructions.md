---
id: PM-INSTRUCTIONS
status: Active
created: 2026-04-30
summary: "Repository-specific PM agent configuration for Samourai DevKit"
---

# PM Agent Instructions — Samourai DevKit

## Tracker Configuration

### Platform
- **Primary**: GitHub Issues
- **Repository**: `simodev25/samourai-devkit`
- **Work item prefix**: `GH`

### Labels
- `change`: marks an issue as a deliverable change
- `bug`: bug fix
- `enhancement`: feature or improvement
- `documentation`: documentation-only change
- `blocked`: work is blocked on external input

### Status Mapping
| Tracker Status | Lifecycle Phase |
|----------------|-----------------|
| Open | Not started |
| In Progress | clarify_scope through delivery |
| In Review | review_fix through pr_creation |
| Closed | Delivered and merged |

## Branch Conventions
- Format: `<type>/<workItemRef>/<slug>`
- Types: `feat`, `fix`, `refactor`, `docs`, `chore`, `test`
- Base branch: `main`

## Quality Gates
- Build: N/A (no build step for this repo)
- Tests: `./scripts/.tests/test-install-samourai.sh` (when applicable)
- Lint: N/A
- Manual verification: install script dry-run on test project

## Delivery Preferences
- One ticket per conversation
- Spec-driven workflow (always write spec before plan)
- Commits: Conventional Commits format
- PR: always create PR, never merge automatically
