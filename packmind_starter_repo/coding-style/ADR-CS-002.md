---
id: ADR-CS-002
title: Enforce Prettier for JavaScript/TypeScript
type: coding-style
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["coding-style"]
enforcement: {"strategy": "lint", "tool": "Prettier", "severity": "error"}
---
## 1  Context
Frontend reviews often stall on inconsistent formatting rules across packages.

## 2  Decision
All JS/TS code **must** be formatted by Prettier with the shared config; CI will fail if code is not formatted.
