---
type: "Platform profile"
title: "Microsoft Power Platform (Power Apps and Power Automate) profile"
description: "Column profile for Microsoft Power Platform (Power Apps and Power Automate) in the App builders group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "app-builders"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id microsoft-power-platform"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

Microsoft low-code suite covering Copilot in Power Apps and Power Automate, plus Power Platform admin and governance controls (environments, data policies, managed environments). Copilot Studio and Dynamics agents are researched separately.

Column group: App builders. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 14 |
| escalated | 9 |
| not-covered | 14 |
| partial | 9 |

| Verification state | Cells |
| --- | --- |
| agent-checked | 37 |
| contested | 9 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Power Platform admin and governance controls | 3p | Environments, environment groups, data policies, advanced connector policies, managed environments, inventory and pipelines. |
| Power Apps with Copilot | 3p | Low-code app builder with Copilot and plans that generate apps and data models from natural language. |
| Power Automate with Copilot | 3p | Cloud and desktop flow automation with Copilot that creates and edits flows from prompts. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | agent-checked | yes |
| [Credential Brokerage](c4-2.md) | Identity | not-covered | agent-checked | yes |
| [Delegation (OBO)](c4-3.md) | Identity | covered | agent-checked | yes |
| [A2A](c4-4.md) | Identity | not-covered | agent-checked | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | covered | agent-checked | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | agent-checked | yes |
| [Human Approval](c1-3.md) | Authorisation | covered | agent-checked | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | escalated | contested | no |
| [Agent Orchestration](c2-1.md) | Runtime | covered | agent-checked | yes |
| [Inference](c2-2.md) | Runtime | escalated | contested | no |
| [Execution Environment](c2-3.md) | Runtime | covered | agent-checked | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | not-covered | agent-checked | yes |
| [Harness](c2-5.md) | Runtime | escalated | contested | no |
| [Agent Persistent Memory](c2-6.md) | Runtime | not-covered | agent-checked | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | partial | agent-checked | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | covered | agent-checked | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | covered | agent-checked | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [HITL](c5-1.md) | Observability & Explainability | covered | agent-checked | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | escalated | contested | no |
| [Cost & Yield](c5-3.md) | Observability & Explainability | escalated | contested | no |
| [Infrastructure](c5-4.md) | Observability & Explainability | covered | agent-checked | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | covered | agent-checked | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | escalated | contested | no |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | covered | agent-checked | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | partial | agent-checked | yes |
| [Posture & Reporting](c6-3.md) | Governance | escalated | contested | no |
| [Policy Management](c6-4.md) | Governance | escalated | contested | no |
| [AI Lifecycle Management](c6-5.md) | Governance | partial | agent-checked | yes |
| [Ownership & Accountability](c6-6.md) | Governance | partial | agent-checked | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | agent-checked | yes |
| [Change & Release Governance](c6-8.md) | Governance | covered | agent-checked | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | agent-checked | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | partial | agent-checked | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | escalated | contested | no |
| [Third-Party Governance](c6-12.md) | Governance | partial | agent-checked | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | covered | agent-checked | yes |

Sources are in the [source registry](sources.md).
