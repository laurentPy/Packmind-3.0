---
id: ADR-DM-002
title: Pin Dependencies to Minor Versions
type: dependency-management
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["dependency-management"]
enforcement: {"strategy": "lint", "tool": "Renovate", "severity": "warning"}
---
## 1  Context
Unpinned versions caused unpredictable builds after upstream patch releases.

## 2  Decision
All dependency versions **must** be pinned to the minor version (e.g., 1.5.x) and auto‑bumped by Renovate PRs.
