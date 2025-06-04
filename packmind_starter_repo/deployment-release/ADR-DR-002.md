---
id: ADR-DR-002
title: Manual Approval Required for Production Releases
type: deployment-release
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["deployment-release"]
enforcement: {"strategy": "policy", "tool": "Argo\u00a0CD", "severity": "error"}
---
## 1  Context
Automated production pushes introduced unreviewed hotfix bugs.

## 2  Decision
Argo CD syncs to prod require manual sign‑off from the on‑call engineer.
