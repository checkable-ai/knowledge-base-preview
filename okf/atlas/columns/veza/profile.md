---
type: "Platform profile"
title: "Veza profile"
description: "Column profile for Veza in the Identity, access and secrets group."
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
    locator: "platforms, id veza"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

Veza's identity security and governance platform, built on the Access Graph, covering AI Agent Security, NHI Security, Access Agents, Access Requests, Access Reviews and Lifecycle Management. Veza is now part of ServiceNow and is described as the agent identity control plane for ServiceNow AI Control Tower.

Column group: Identity, access and secrets. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 6 |
| escalated | 8 |
| not-covered | 27 |
| partial | 5 |

| Verification state | Cells |
| --- | --- |
| agent-checked | 38 |
| contested | 8 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Veza Access Agents (Access AI) | 3p | Natural language agents inside Veza that search the graph, explain reviews and policies, and classify non-human identities. |
| Veza Access Graph and Access Intelligence | 3p | Graph of identities, resources and permissions across cloud, SaaS and data systems, with search, risks, rules and alerts. |
| Veza AI Agent Security | 3p | Discovery and governance of AI agents, models, tools and MCP servers across named agent platforms, with access path analysis and ownership. |
| Veza Access Requests, Access Reviews and Lifecycle Management | 3p | Identity governance workflows for access approval, certification campaigns and joiner, mover and leaver automation. |
| Veza NHI Security | 3p | Discovery of service accounts, API keys, tokens and certificates, with ownership, rotation tracking and remediation. |
| Veza from ServiceNow | 3p | Veza following the ServiceNow acquisition completed on 2 March 2026, positioned as the enterprise agent identity control plane within ServiceNow AI Control Tower. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | partial | agent-checked | yes |
| [Credential Brokerage](c4-2.md) | Identity | not-covered | agent-checked | yes |
| [Delegation (OBO)](c4-3.md) | Identity | not-covered | agent-checked | yes |
| [A2A](c4-4.md) | Identity | not-covered | agent-checked | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | escalated | contested | no |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | agent-checked | yes |
| [Human Approval](c1-3.md) | Authorisation | not-covered | agent-checked | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | not-covered | agent-checked | yes |
| [Agent Orchestration](c2-1.md) | Runtime | escalated | contested | no |
| [Inference](c2-2.md) | Runtime | escalated | contested | no |
| [Execution Environment](c2-3.md) | Runtime | escalated | contested | no |
| [Agent In-Session Memory](c2-4.md) | Runtime | escalated | contested | no |
| [Harness](c2-5.md) | Runtime | escalated | contested | no |
| [Agent Persistent Memory](c2-6.md) | Runtime | escalated | contested | no |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | not-covered | agent-checked | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [HITL](c5-1.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | covered | agent-checked | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | covered | agent-checked | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | covered | agent-checked | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | agent-checked | yes |
| [Posture & Reporting](c6-3.md) | Governance | partial | agent-checked | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | agent-checked | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | agent-checked | yes |
| [Ownership & Accountability](c6-6.md) | Governance | covered | agent-checked | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | agent-checked | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | agent-checked | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | escalated | contested | no |
| [Data Lifecycle Governance](c6-10.md) | Governance | not-covered | agent-checked | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | partial | agent-checked | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | agent-checked | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | covered | agent-checked | yes |

Sources are in the [source registry](sources.md).
