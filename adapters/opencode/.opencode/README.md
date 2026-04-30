# OpenCode Kit V1.1 - Tooling

## Layout

- Config: `.opencode/opencode.jsonc`
- Agents: `.opencode/agent/*.md`
- Commandes: `.opencode/command/*.md`
- Skills: `.opencode/skills/<skill>/SKILL.md`
- Skills projet générés: `.opencode/skills/project/<skill>/SKILL.md`

## Agents V1

- `bootstrapper`
- `pm`
- `spec-writer`
- `test-plan-writer`
- `plan-writer`
- `coder`
- `reviewer`
- `runner`
- `fixer`
- `doc-syncer`
- `committer`
- `pr-manager`

## Agents complémentaires 

- `architect`
- `code-reviewer`
- `designer`
- `editor`
- `external-researcher`
- `image-generator`
- `image-reviewer`
- `review-feedback-applier`
- `tdd-orchestrator`
- `toolsmith`

## Commandes V1

- `/bootstrap`
- `/plan-change`
- `/write-spec`
- `/write-test-plan`
- `/write-plan`
- `/run-plan`
- `/tdd`
- `/review`
- `/check`
- `/check-fix`
- `/sync-docs`
- `/commit`
- `/pr`
- `/git-workflow`

## Extension V1.1

- `/generate-project-skills`
- `/test-api-e2e`

## Skills V1

- `brainstorming`
- `writing-plans`
- `test-driven-development`
- `systematic-debugging`
- `requesting-code-review`
- `receiving-code-review`
- `verification-before-completion`
- `dispatching-parallel-agents`
- `finishing-a-development-branch`
- `agent-orchestration`
- `git-workflow-orchestrator`
- `tdd-orchestrator`

## Artefacts installés

Le core Samourai est installé sous `.samourai/core/`. L’adapter OpenCode est
installé sous `.opencode/`.

- `.opencode/agent/*.md`
- `.opencode/command/*.md`
- `.opencode/skills/*/SKILL.md`
- `.samourai/core/governance/conventions/*`
- `.samourai/core/governance/lifecycle/*`
- `.samourai/core/governance/policies/*`
- `.samourai/core/templates/*`
- `.samourai/core/decisions/*`

`AGENTS.md` n’est pas fourni comme fichier statique. Il est généré par `/bootstrap`
dans le projet cible.

## Conventions

- Nommage en `kebab-case`
- Une commande = un fichier
- Un agent = un fichier
- Un skill = un dossier avec `SKILL.md`
