# Engineering Leadership + Agentic SDLC Copilot Starter Kit

This is a **self-contained starter kit**, not a security-certified or tested production plugin. It uses first-party VS Code/GitHub Copilot customization conventions.

## Install in an existing VS Code project
1. Back up/commit changes. Unzip this archive.
2. Copy the `.github` folder into your repo **merging**, not overwriting existing instructions. Review every file before committing.
3. Open that repository in an updated VS Code with GitHub Copilot access. Select Agent in Copilot Chat.
4. Select a named agent from the agent picker (e.g. `architecture-challenger`), then request a review.
5. In Copilot Chat type `/skills` to inspect discovered skills; or open the Agent Customizations interface. Skills are loaded when relevant based on metadata.
6. Start read-only. Only authorize writes/terminal commands after reviewing the plan and organizational policy.

## Install personally across repositories
Copy selected `.github/agents/*.agent.md` to `~/.copilot/agents/` and selected `.github/skills/<name>/` folders to `~/.copilot/skills/`. Keep repo-specific instructions inside the repo. Exact supported paths may differ between Copilot harnesses; review VS Code's Custom Agents page.

## Try these prompts
- Select `architecture-challenger`: 'Review this application's inbound and outbound integration architecture. Cite specific files and write a tradeoff-based ADR.'
- Select `qa-strategist`: 'Propose a risk-based quality strategy for the next release; identify uncovered negative paths and evidence requirements.'
- Select `dev-lead`: 'Assess technical debt, prioritizing measurable risks and changes achievable in two sprints.'
- Select `agentic-sdlc-designer`: 'Design a governed pilot for agent-generated PRs with human review and reproducible evaluations.'
- Select `delivery-advisor`: 'Challenge this plan; distinguish assumptions, commitments and critical-path dependencies.'
- Select `people-leader`: 'Help me prepare an anonymized coaching conversation about missed ownership commitments.'

## Optional Spec Kit integration (separate from core kit)
Install `uv` and `uv tool install specify-cli`, verify `specify version`, then in a **throwaway test repo** initialize `specify init . --integration copilot`. For an existing repo follow the Spec Kit existing-project adoption instructions first; its initializer can modify workspace customizations. Do not run it blindly over an existing `.github` tree. Consider version pinning for team rollout.

## Governance
- Pilot with anonymized/synthetic data and a read-only architecture review first.
- Define tool permissions, data access boundaries, command approvals, branch protections, mandatory CI and human PR approval.
- No production deploy or autonomous secrets access.
- Maintain a reviewed allowlist of third-party skills and a changelog of revisions.
- Run baseline evaluations before expanding autonomous tasks.

## Evaluation scorecard
For 10–20 tasks, record category, complexity, baseline effort, Copilot effort, active human minutes, review defects, test results, change failure/rollback, cost and reviewer acceptance. Compare similar tasks and avoid measuring success by generated LOC.

## Sources
- https://code.visualstudio.com/docs/agent-customization/custom-agents
- https://code.visualstudio.com/docs/agent-customization/agent-skills
- https://code.visualstudio.com/docs/agent-customization/custom-instructions
- https://github.com/github/awesome-copilot
- https://github.com/github/spec-kit
- https://github.com/obra/superpowers
- https://github.com/microsoft/skills
