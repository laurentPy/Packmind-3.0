---
id: ADR-SP-001
title: Secrets Never Committed to Git
type: security-privacy
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["security-privacy"]
enforcement: {"strategy": "scan", "tool": "Trivy", "severity": "error"}
---
## 1  Context
Historical secret leaks required mass rotations.

## 2  Decision
CI will block any commit that contains potential secrets; use Vault for runtime injection.
