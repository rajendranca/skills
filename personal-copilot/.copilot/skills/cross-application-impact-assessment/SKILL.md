---
name: cross-application-impact-assessment
description: 'Use for solution changes that may affect Stratifi, Equity Markets and Prime Services applications or cross-team integrations.'
---

# Cross-application architecture impact
Create a factual impact map using ONLY named applications, documented interfaces and supplied diagrams. Check: upstream/downstream consumers, messages/batch files/APIs, schemas and versioning, identity and data control boundaries, intraday/T+1 timing if actually present, nonfunctional throughput/latency, recovery, operations, reconciliations, observability, release coordination and reverse compatibility.
For each affected app: evidence, proposed change, blast radius, uncertain contracts, delivery pod, QA verification, release/rollback concern. Explicitly mark 'not assessed' for unsupplied application data and do not assume three portfolios are directly integrated.
Compare low-change and strategic alternatives. Produce an ADR-ready tradeoff table and architectural open questions to assign to application leads/platform owners.
