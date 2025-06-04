---
id: ADR-DS-001
title: Use Postgres 16 with Flyway Migrations
type: data-modeling
status: active
scope: global
created: 2025-06-04
review: 2026-06-04
owner: @laurent.py
tags: ["data-modeling"]
enforcement: {"strategy": "migration-lint", "tool": "Flyway", "severity": "error"}
---
## 1  Context
Multiple DB engines increased operational complexity.

## 2  Decision
All relational data must live in Postgres 16; Flyway migration scripts manage schema evolution.
