---
id: ADR-DS-002
title: Snake_case Plural Table Names
type: data-modeling
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["data-modeling"]
enforcement: {"strategy": "lint", "tool": "SqlFluff", "severity": "warning"}
---
## 1  Context
Inconsistent table naming slowed onboarding and automated code‑gen.

## 2  Decision
Tables must use lower‑snake plural names (e.g., `user_accounts`); SqlFluff enforces naming.
