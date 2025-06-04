---
id: ADR-DR-001
title: Blue‑Green Deployments via Argo CD
type: deployment-release
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["deployment-release"]
enforcement: {"strategy": "policy", "tool": "Argo\u00a0CD", "severity": "warning"}
---
## 1  Context
Downtime during in‑place deploys impacted SLAs.

## 2  Decision
Deploy pipelines must implement blue‑green strategy through Argo CD rollout step.
