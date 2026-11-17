---
type: "Platform profile"
title: "AuthZed (SpiceDB) profile"
description: "Column profile for AuthZed (SpiceDB) in the Identity, access and secrets group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "identity"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id authzed-spicedb"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

AuthZed's Zanzibar-style fine-grained authorisation platform: open source SpiceDB, AuthZed Cloud, AuthZed Dedicated and SpiceDB Enterprise, plus its AI agent material (SpiceBox, spicedb-dev, Open Agent Primitives and MCP servers).

Column group: Identity, access and secrets. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 17 |
| escalated | 3 |
| not-covered | 18 |
| partial | 8 |

| Verification state | Cells |
| --- | --- |
| contested | 3 |
| verified | 43 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| AuthZed Cloud | 3p | Hosted self-service SpiceDB with audit logging and restricted API access included. |
| AuthZed Dedicated | 3p | Managed SpiceDB on dedicated infrastructure with private networking, multi-region deployments and a management dashboard. |
| SpiceDB Enterprise | 3p | Commercially licensed SpiceDB build for self-hosting that adds audit logging, restricted API access, rate limiting and security embargo. |
| AuthZed MCP servers | 3p | A remote documentation MCP server and a local in-memory SpiceDB development MCP server. |
| Open Agent Primitives (OAP) | 3p | Open source platform for running enterprise AI agents on six named primitives, described in one AuthZed blog post. |
| SpiceBox and spicedb-dev | 3p | Open source tools that enforce SpiceDB permissions on Claude Code agent tool calls (SpiceBox) and teach coding agents to add authorisation to generated code (spicedb-dev). |
| SpiceDB (open source) | 3p | Apache 2.0 permissions database that stores relationships and answers permission checks against a schema. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | partial | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | covered | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | covered | verified | yes |
| [A2A](c4-4.md) | Identity | partial | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | covered | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | covered | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | covered | verified | yes |
| [Inference](c2-2.md) | Runtime | escalated | contested | no |
| [Execution Environment](c2-3.md) | Runtime | covered | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | covered | verified | yes |
| [Harness](c2-5.md) | Runtime | covered | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | covered | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | covered | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | partial | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | covered | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | partial | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | partial | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | escalated | contested | no |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | escalated | contested | no |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | partial | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | partial | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | partial | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | not-covered | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | not-covered | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | not-covered | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | covered | verified | yes |

Sources are in the [source registry](sources.md).
