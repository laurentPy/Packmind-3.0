---
id: ADR-DM-001
title: Allow Only MIT or Apache‑2.0 Licensed Dependencies
type: dependency-management
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["dependency-management"]
enforcement: {"strategy": "policy", "tool": "Snyk Licenses", "severity": "error"}
---
## 1  Context
Licensing compliance risk exists with GPL‑licensed transitive dependencies.

## 2  Decision
CI license scan will block merges if a new non‑permitted license is detected.
