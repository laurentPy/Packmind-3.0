---
id: ADR-OB-001
title: Structured JSON Logs Schema v2
type: observability
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["observability"]
enforcement: {"strategy": "lint", "tool": "Log\u2011Schema Linter", "severity": "warning"}
---
## 1  Context
Free‑form logs hindered automated parsing.

## 2  Decision
Services must emit logs that conform to schema v2; linter runs in CI.
