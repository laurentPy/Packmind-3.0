---
id: ADR-SA-001
title: Microservices Aligned with Bounded Contexts
type: system-architecture
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["system-architecture"]
enforcement: {"strategy": "policy", "tool": "ArchUnit", "severity": "warning"}
---
## 1  Context
Random service splits created chatty dependencies and unclear ownership.

## 2  Decision
Service boundaries must map to domain bounded contexts; ArchUnit rules detect cross‑context calls.
