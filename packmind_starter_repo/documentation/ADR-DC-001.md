---
id: ADR-DC-001
title: Every Public Module Requires TechDocs Page
type: documentation
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["documentation"]
enforcement: {"strategy": "check", "tool": "Doc\u2011Link Checker", "severity": "warning"}
---
## 1  Context
Engineers struggle to find module usage examples.

## 2  Decision
Merge blocked if TechDocs link missing; checker verifies presence.
