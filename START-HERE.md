# Engineering Leadership Copilot v2 — personal-first VS Code installation
**Optimized for a corporate laptop, GitHub Copilot in VS Code, frontier models, Markdown/architecture diagrams, no Git repository required.**

This is a self-contained updated version of the earlier Leadership Workspace Starter. It includes previously recommended engineering/QA/agentic skills plus chief-architect, portfolio-delivery and intake workflows.

## Quick 10-minute setup (no admin rights or scripts required)
1. Verify your corporate Copilot license and approval to use **your chosen frontier models**, custom agents and this approved document content. Do not paste confidential employee/client/control information into unapproved services.
2. Back up existing personal customizations. Open VS Code → Copilot Chat → select **Copilot** harness (if target selector appears) → gear icon / **Chat: Open Customizations**.
3. In the Agents tab select **New Agent (User)**. Paste `personal-copilot/.copilot/agents/portfolio-chief-architect.agent.md`; save. Repeat for `intake-triage-lead.agent.md`, `pod-delivery-governor.agent.md` and `architecture-governance-chair.agent.md`. Optional specialist agents can be added later.
4. In the Skills tab select **New Skill (User)** and create `intake-triage-routing`, `cross-application-impact-assessment`, `pod-delivery-governance`, `portfolio-health-review` and `delegation-and-decision-rights`, pasting each `SKILL.md`. Use the other skills as needed. Name must equal containing folder.
5. For personal always-on instructions, use the contents of `personal-copilot/.copilot/copilot-instructions.md` and create/merge it via the approved personal customization location/UI.
6. Select your preferred approved frontier model from **Copilot Chat's model picker** or select **Auto / Intelligence** if available. No agent YAML fixes a model, so your choice stays flexible.
7. Open `sample-leadership-workspace` via File → Open Folder. No `.git` needed; use the `.template.md` files after reviewing them. Paste only approved, appropriately classified material.
8. Select `portfolio-chief-architect` and try: 'Review this folder, summarize what is *actually documented* about the portfolio, and identify top 5 missing items required to triage a new intake. No changes.'

## Manual file method (Copilot harness)
Place selected agent files at `~/.copilot/agents/`, selected full skill folders at `~/.copilot/skills/`, and personal instructions at `~/.copilot/copilot-instructions.md`. Optionally place `.instructions.md` files at `~/.copilot/instructions/`.
`~` means **your user home directory**. On Windows it is commonly `%USERPROFILE%`, on macOS `$HOME`. Corporate-managed VS Code may have limitations; use the Customizations UI rather than bypassing controls.

After installing, run `/agents` to check agent discovery and `/skills` to check skills. If a file is unrecognized, confirm the **selected harness**, path, name, and Customizations editor or Developer: Open Agent Debug Logs. Reloading VS Code may help but is not the first step.

## Which agent should I select?
| Situation | Select | Why |
|---|---|---|
| Most requests or unclear scope | `portfolio-chief-architect` | Integrated architecture + delivery decision lens |
| New demand/request | `intake-triage-lead` | Fast route decision and stakeholder set |
| Design/ADR | `architecture-governance-chair` | Technical options, cross-app impacts, gates |
| Pod/release blockers | `pod-delivery-governor` | Management by exception and delegation |
| New stakeholders/meetings | `stakeholder-and-delegation-advisor` | Consult/inform/own/approve map |
| Executive update | `executive-portfolio-briefing` | Sharp recommendation and decision requests |
| Quality deep dive | `qa-strategist` | QA assurance questions; not QA signoff |
| Agentic SDLC adoption | `agentic-transformation-lead` | Pilot operating model and governance |
| People feedback | `people-leader` | Private preparation with minimal employee data |

See `WORKFLOWS-AND-PROMPTS.md` for ten ready prompts. See `MIGRATION-FROM-PRIOR-KIT.md` to merge without overwriting the old kit.

## Permissions and data-security posture
- These agent definitions explicitly expose only built-in `read` and `search` tool sets; they **cannot directly edit or execute commands through those tool sets**, assuming the selected harness honors their tool restrictions. Check the tools picker and corporate policy on every new harness.
- To write an approved file, ask for text in chat and paste it after review, or temporarily use a separately reviewed editing agent with an appropriate approval gate. A prompt alone is not a security boundary.
- No MCP servers, downloaded packages, auto-run scripts, CI/CD credentials or GitHub repository access are configured. Third-party/community skills must be reviewed before use.
- A **role map** in the workspace is an example, not actual corporate reporting structure or formal decision authority. Customize it with organization-approved facts before trusting routing recommendations.
- Pod commitments, architecture approvals, production change signoffs and HR decisions stay with authorized people.

## What changed versus v1
The earlier kit mostly helped review engineering documents. This kit adds **the operating system of the chief architect/delivery-owner role**: intake decisions, architecture impact, delegation and stakeholders, pod dependencies, QA oversight, portfolio pulse and agentic SDLC governance.

## References (current VS Code documentation)
- Custom agents: https://code.visualstudio.com/docs/agent-customization/custom-agents
- Personal skills: https://code.visualstudio.com/docs/agent-customization/agent-skills
- Custom instructions: https://code.visualstudio.com/docs/agent-customization/custom-instructions
- Tool sets and permissions: https://code.visualstudio.com/docs/agents/reference/tools-reference
- Model picker and Auto optimization: https://code.visualstudio.com/docs/agent-customization/language-models
