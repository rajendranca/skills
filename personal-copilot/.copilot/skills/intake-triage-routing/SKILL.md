---
name: intake-triage-routing
description: 'Use for every new idea, project request, urgent ask, enhancement or intake; determine whether triage or deeper discovery is needed.'
---

# Demand intake decisioning
1. Translate request into business outcome and classify as: operational incident/escalation; BAU change; bounded enhancement; new project/program; cross-platform modernization; regulatory/compliance/security-driven request. If unclear label tentative.
2. Evaluate: criticality/time-sensitivity (external vs asserted), impacted application(s), scope clarity, integrations/data/security changes, production/customer/market risk, dependencies, cost/capacity/effort uncertainty, required funding/governance. Use qualitative low/medium/high with reasons, not fake scores.
3. Route:
   - **Operational escalation**: time-sensitive production/control event → operational incident/security process; notify relevant on-call and stakeholders *as a recommendation*, don't send.
   - **Quick triage**: bounded, known owner, limited blast radius, established pattern and acceptable uncertainty → clarify and route to existing backlog.
   - **Focused discovery**: ambiguous business need, cross-app/API/data/NFR impact, capacity unknown or novel architecture → BA-led discovery and technical impact assessment.
   - **Formal project intake**: material funding, multi-pod work, external commitment, strategic change → sponsor, delivery manager and governance path after discovery.
4. Name **proposed roles**: sponsor/business owner; BA; impacted application/pod lead; senior manager; delivery manager; chief QA lead; architecture owner; security, infra, data, operations, vendors only if impact justifies. Validate actual assignment.
5. Deliver: one-paragraph understanding, recommended route + confidence, key rationale, stakeholder table (engage / why / when), 3–6 unknowns, proposed first gate, 3 next actions with provisional owners. Clearly separate triage decision from priority or delivery commitment.

If the opened workspace contains `01-intake/intake-record.template.md`, use it as an optional reference. Otherwise give a Markdown triage summary in chat.
