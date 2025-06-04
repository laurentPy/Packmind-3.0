---
id: ADR-OB-002
title: Prometheus Metrics Prefix with service_
type: observability
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["observability"]
enforcement: {"strategy": "lint", "tool": "Prometheus Rules Linter", "severity": "warning"}
---
## 1  Context
Metric name collisions and unclear ownership in dashboards.

## 2  Decision
All custom metrics must prefix `service_`; linter validates prometheus rules.
