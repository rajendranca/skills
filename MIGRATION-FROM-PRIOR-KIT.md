# Upgrade from the previous Leadership Workspace Starter

## What is preserved
All prior personal agents/skills and the optional earlier development-oriented team repository configuration remain in this v2 package. Existing agents are scoped to `read` and `search` tool sets for advisory operation. Most older secondary agents are hidden from the picker using `user-invocable: false` to reduce clutter; they remain as files and can be made visible by changing this setting to `true`.

## What's new
- Chief-architect persona and role-specific permanent context.
- New intake triage and stakeholder routing agent/skills.
- Multi-pod governance, portfolio reporting, delegation, architecture governance and leadership briefing agents/skills.
- Example-only Markdown workspace for intake, architecture, delivery/QA, stakeholder routing and agentic SDLC pilot.
- Read/search-only tool configuration for primary personal agents; frontier-model selection remains in the VS Code UI.

## How to upgrade safely
1. Back up current `~/.copilot/` personal customizations and any workspace `.github` customizations.
2. Diff the new `personal-copilot/.copilot/copilot-instructions.md` against your existing personal file; merge rather than overwrite confidential corporate rules.
3. Merge `agents/`, `skills/` and `instructions/` after reviewing modified agent frontmatter. Do not overwrite organization-managed files.
4. Open the sample workspace as a plain folder and confirm agents/skills discover correctly.
5. Skip the `optional-team-repo-kit` unless you explicitly want repo-scoped engineering coding standards; it is retained as a reference, not automatically deployed.

## Different agent hosts
Select the **Copilot** harness/target in VS Code's Chat Customizations UI. Local, Copilot and other harnesses can have different supported storage paths. The `.copilot` personal folder in this kit targets Copilot harness behavior.
