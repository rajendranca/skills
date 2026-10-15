# Concept-only diagram — replace with verified app facts
This is an **illustrative workflow**, NOT a representation of Stratifi, Equity Markets or Prime Services integrations.

```mermaid
flowchart LR
  Request[Business Intake] --> Triage{Triage outcome}
  Triage -->|Small scoped change| Backlog[Existing Pod Backlog]
  Triage -->|High uncertainty| Discovery[Discovery and Impact]
  Triage -->|Operational event| Incident[Incident Process]
  Discovery --> Design[Architecture Review]
  Design --> Plan[Delivery Manager and Pod Planning]
  Plan --> QA[Chief QA Lead: Test Strategy and Gates]
  QA --> Change[Approved Change / Release Governance]
```

Unknown: actual organizational authority, pod routing, tool integrations, exception procedures.
