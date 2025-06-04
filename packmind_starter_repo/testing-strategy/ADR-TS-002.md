---
id: ADR-TS-002
title: Mutation Score ≥ 60 %
type: testing-strategy
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["testing-strategy"]
enforcement: {"strategy": "test", "tool": "Stryker", "severity": "warning"}
---
## 1  Context
High coverage did not guarantee assertion quality, evidenced by surviving mutants.

## 2  Decision
Mutation tests must achieve at least 60 % kill rate before merge.
