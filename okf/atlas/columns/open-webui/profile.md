---
type: "Platform profile"
title: "Open WebUI profile"
description: "Column profile for Open WebUI in the Self-hosted and hybrid group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "self-hosted"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id open-webui"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

Open WebUI is a self-hosted chat and agent interface for local and API models. This research covers the open source application as documented, plus the enterprise-licensed Terminals orchestrator and the Open Terminal agent workspace.

Column group: Self-hosted and hybrid. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 9 |
| escalated | 9 |
| not-covered | 18 |
| partial | 10 |

| Verification state | Cells |
| --- | --- |
| contested | 9 |
| verified | 37 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Open WebUI | 3p | Self-hosted web application with chat, RBAC, workspace models, knowledge bases (RAG), tools, functions, MCP and audit logging. |
| Open Terminal | 3p | Containerised shell and file API that Open WebUI uses as an agent workspace for code and command execution. |
| Terminals orchestrator | 3p | Enterprise-licensed orchestration layer that provisions an isolated Open Terminal workspace per user under admin policies. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | partial | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | covered | verified | yes |
| [A2A](c4-4.md) | Identity | not-covered | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | covered | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | covered | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | escalated | contested | no |
| [Inference](c2-2.md) | Runtime | escalated | contested | no |
| [Execution Environment](c2-3.md) | Runtime | covered | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | escalated | contested | no |
| [Harness](c2-5.md) | Runtime | covered | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | covered | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | escalated | contested | no |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | escalated | contested | no |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | partial | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | partial | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | partial | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | partial | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | covered | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | not-covered | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | partial | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | partial | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | escalated | contested | no |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | partial | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | escalated | contested | no |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | escalated | contested | no |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | partial | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | partial | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | escalated | contested | no |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | not-covered | verified | yes |

Sources are in the [source registry](sources.md).
