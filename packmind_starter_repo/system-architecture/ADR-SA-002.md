---
id: ADR-SA-002
title: No UI → Core Domain Direct Calls
type: system-architecture
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["system-architecture"]
enforcement: {"strategy": "policy", "tool": "Sonargraph", "severity": "error"}
---
## 1  Context
UI layers bypassing the API layer created tight coupling.

## 2  Decision
UI modules may only call through the API gateway; Sonargraph checks enforce the dependency graph.
