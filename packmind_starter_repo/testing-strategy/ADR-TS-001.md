---
id: ADR-TS-001
title: Maintain 90 % Line Coverage on Critical Services
type: testing-strategy
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["testing-strategy"]
enforcement: {"strategy": "test", "tool": "Jest", "severity": "error"}
---
## 1  Context
Recent outages stemmed from untested edge cases in core services.

## 2  Decision
PRs decreasing coverage below 90 % will fail the pipeline.
