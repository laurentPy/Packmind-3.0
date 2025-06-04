---
id: ADR-SP-002
title: Mandatory TLS 1.3 for All Traffic
type: security-privacy
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["security-privacy"]
enforcement: {"strategy": "policy", "tool": "OPA Gatekeeper", "severity": "error"}
---
## 1  Context
Older TLS versions expose downgrade and cipher vulnerabilities.

## 2  Decision
Ingress controllers must enforce TLS 1.3 only; Gatekeeper policies validate configuration.
