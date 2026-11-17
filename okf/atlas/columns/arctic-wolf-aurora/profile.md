---
type: "Platform profile"
title: "Arctic Wolf (Aurora platform and Agentic SOC) profile"
description: "Column profile for Arctic Wolf (Aurora platform and Agentic SOC) in the Security operations (SIEM, XDR) group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "secops"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id arctic-wolf-aurora"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

Arctic Wolf is a managed detection and response vendor. This research covers the Aurora Superintelligence Platform, the Aurora Agentic SOC (the Swarm of Experts agents and AI Trust Engine), Aurora AI including the Aurora Security Assistant, and the Unified Portal controls around them.

Column group: Security operations (SIEM, XDR). Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 2 |
| escalated | 7 |
| not-covered | 30 |
| partial | 7 |

| Verification state | Cells |
| --- | --- |
| contested | 7 |
| verified | 39 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Aurora Agentic SOC | 3p | Agent-led security operations run by Arctic Wolf using the Swarm of Experts, with human analysts overseeing high-impact decisions. |
| Aurora Managed Detection and Response with Active Response | 3p | 24x7 monitoring service with optional response actions through integrations. |
| Aurora Superintelligence Platform | 3p | Arctic Wolf's data and AI platform that feeds its security operations services. |
| Arctic Wolf Unified Portal | 3p | Customer web portal for tickets, investigations, dashboards, Data Explorer and organisation settings. |
| Aurora Security Assistant | 3p | Customer-facing generative AI assistant in the Unified Portal for questions about tickets, risks and assets. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | not-covered | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | escalated | contested | no |
| [A2A](c4-4.md) | Identity | not-covered | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | not-covered | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | partial | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | partial | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | partial | verified | yes |
| [Inference](c2-2.md) | Runtime | partial | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | not-covered | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | partial | verified | yes |
| [Harness](c2-5.md) | Runtime | not-covered | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | escalated | contested | no |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | escalated | contested | no |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | escalated | contested | no |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | not-covered | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | partial | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | not-covered | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | not-covered | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | not-covered | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | not-covered | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | not-covered | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | partial | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | not-covered | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | escalated | contested | no |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | escalated | contested | no |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | escalated | contested | no |

Sources are in the [source registry](sources.md).
