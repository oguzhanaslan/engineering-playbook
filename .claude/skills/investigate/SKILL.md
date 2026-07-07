---
name: investigate
description: Use when tracing data flow, debugging behavior, finding where data comes from, identifying APIs, services, components, execution flow, and evidence.
---

# Investigate

Root-cause analysis and data-flow tracing. Never speculate — cite evidence (file, log, code path).

- State symptom vs expected.
- Trace the data: source → owning service → API → component → render; map the execution flow.
- Form hypotheses; confirm the root cause with evidence before concluding.
- Fix the root cause; add a regression test; note blast radius.
