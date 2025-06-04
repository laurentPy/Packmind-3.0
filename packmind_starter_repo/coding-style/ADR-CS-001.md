---
id: ADR-CS-001
title: Enforce Google Java Style
type: coding-style
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["coding-style"]
enforcement: {"strategy": "lint", "tool": "Spotless", "severity": "error"}
---
## 1  Context
Developers spend significant time debating whitespace and brace placement.

## 2  Decision
All Java code **must** follow Google Java Style; Spotless will auto‑format on commit and fail CI if violations remain.
