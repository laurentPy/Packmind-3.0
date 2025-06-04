---
id: ADR-API-001
title: Expose OpenAPI 3 Spec & Semantic Versioning
type: api-contracts
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["api-contracts"]
enforcement: {"strategy": "contract-test", "tool": "Spectral", "severity": "error"}
---
## 1  Context
Breaking API changes surfaced late, causing downstream client failures.

## 2  Decision
Every public API must ship an OpenAPI 3 spec and follow semver; Spectral rules validate breaking changes.
