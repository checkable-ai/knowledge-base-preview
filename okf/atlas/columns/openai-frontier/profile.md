---
type: "Platform profile"
title: "OpenAI Frontier profile"
description: "Column profile for OpenAI Frontier in the Enterprise and workplace agents group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "enterprise-agents"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id openai-frontier"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

OpenAI's enterprise platform to build, deploy and manage AI agents (AI coworkers) with shared business context, agent identity and permissions and an agent execution environment. Covers the Frontier platform only, not the OpenAI APIs.

Column group: Enterprise and workplace agents. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 3 |
| escalated | 3 |
| not-covered | 35 |
| partial | 5 |

| Verification state | Cells |
| --- | --- |
| agent-checked | 43 |
| contested | 3 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Enterprise Frontier Program | 1p | Forward deployed engineers who work with the customer to design architectures, operationalise governance and run agents in production. |
| OpenAI Frontier | 1p | Enterprise agent platform with Business Context, Agent Execution, evaluation and optimisation loops, and agent identity and access management, available to a limited set of customers. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | partial | agent-checked | yes |
| [Credential Brokerage](c4-2.md) | Identity | not-covered | agent-checked | yes |
| [Delegation (OBO)](c4-3.md) | Identity | not-covered | agent-checked | yes |
| [A2A](c4-4.md) | Identity | not-covered | agent-checked | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | not-covered | agent-checked | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | agent-checked | yes |
| [Human Approval](c1-3.md) | Authorisation | not-covered | agent-checked | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | escalated | contested | no |
| [Agent Orchestration](c2-1.md) | Runtime | escalated | contested | no |
| [Inference](c2-2.md) | Runtime | not-covered | agent-checked | yes |
| [Execution Environment](c2-3.md) | Runtime | partial | agent-checked | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | not-covered | agent-checked | yes |
| [Harness](c2-5.md) | Runtime | covered | agent-checked | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | covered | agent-checked | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | not-covered | agent-checked | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | partial | agent-checked | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [HITL](c5-1.md) | Observability & Explainability | escalated | contested | no |
| [Behavioural](c5-2.md) | Observability & Explainability | partial | agent-checked | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | not-covered | agent-checked | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | agent-checked | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | agent-checked | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | agent-checked | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | agent-checked | yes |
| [Ownership & Accountability](c6-6.md) | Governance | not-covered | agent-checked | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | agent-checked | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | agent-checked | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | agent-checked | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | not-covered | agent-checked | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | agent-checked | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | agent-checked | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | partial | agent-checked | yes |

Sources are in the [source registry](sources.md).
