---
name: testing
description: Apply testing engineering standards to relevant files and reviews.
applyTo: "**/*.{test.ts,spec.ts,cs}"
---
Tests should be deterministic, readable, isolated, and tied to requirements. Include boundary/negative cases, and avoid brittle sleeps or unverified mocks.
