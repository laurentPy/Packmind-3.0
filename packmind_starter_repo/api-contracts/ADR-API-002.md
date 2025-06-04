---
id: ADR-API-002
title: Adopt JSON:API Spec for Internal HTTP APIs
type: api-contracts
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["api-contracts"]
enforcement: {"strategy": "contract-test", "tool": "Dredd", "severity": "warning"}
---
## 1  Context
Inconsistent response shapes complicate shared tooling.

## 2  Decision
Internal service APIs must conform to JSON:API; Dredd contract tests validate spec adherence.
