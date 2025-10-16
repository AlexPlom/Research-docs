# Spec Kit

GitHub Spec Kit is an open-source toolkit for **Spec-Driven Development** (SDD): you capture the product outcome as a living specification and let AI agents execute against that spec. Instead of ad-hoc prompting, Spec Kit keeps your agents focused on the agreed scenario, so the code and documentation that ship are aligned with the plan.

## Installation
- Install the `specify` CLI once via `uv` (recommended):  
  ```bash
  uv tool install specify-cli --from git+https://github.com/github/spec-kit.git
  ```
- Run ad-hoc without installing:  
  ```bash
  uvx --from git+https://github.com/github/spec-kit.git specify init <project-name>
  ```
- Upgrade when new releases drop:  
  ```bash
  uv tool install specify-cli --force --from git+https://github.com/github/spec-kit.git
  ```
> The CLI expects `uv` to be available; install it from [https://docs.astral.sh/uv/](https://docs.astral.sh/uv/) if you have not already.

## Core Commands
- `/speckit.constitution` — codify project principles that every agent run must respect.
- `/speckit.specify` — capture the product scenario, user goals, and success criteria.
- `/speckit.plan` — translate the spec into architecture choices, dependencies, and risk notes.
- `/speckit.tasks` — generate an ordered task graph (with parallel markers) that the implementer will follow.
- `/speckit.implement` — drive the AI agent through the tasks, issuing real CLI calls, tests, and code edits.
- `specify init|check` — bootstrap or validate a local Spec Kit workspace directly from the CLI.

## How It Works
1. **Specify** the outcome, not the technology. The spec becomes the single source of truth.
2. **Plan** the solution: decide frameworks, integrations, and entry points before touching code.
3. **Task** it out: Spec Kit materialises the plan into actionable, dependency-aware checklists.
4. **Implement** with your preferred AI pair (Copilot Workspace, Claude Code, Gemini CLI, etc.). The agent executes tasks, runs tests, and keeps artifacts in sync with the spec.

The loop is iterative: refine specs or plans, regenerate tasks, and re-run `/speckit.implement` until the feature meets acceptance criteria. Because the spec drives every step, drift between requirements and implementation is caught early.

## Useful Videos
- [Will GitHub Spec Kit Replace Prompting? Full Deep Dive](https://www.youtube.com/watch?v=YUo5xKoAEuI)
- [GitHub Spec Kit First Look](https://www.youtube.com/watch?v=xgnIBh25a5A)
- [The ONLY guide you'll need for GitHub Spec Kit](https://www.youtube.com/watch?v=a9eR1xsfvHg)
- [Using GitHub Spec Kit with your EXISTING PROJECTS](https://www.youtube.com/watch?v=SGHIQTsPzuY)
- [GitHub Spec Kit DOES WHAT Under The Hood?](https://www.youtube.com/watch?v=o6SYjY1Bkzo)
