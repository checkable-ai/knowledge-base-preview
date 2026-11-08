---
type: "Platform profile"
title: "Microsoft PyRIT profile"
description: "Column profile for Microsoft PyRIT in the Red teaming and testing group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "red-team"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id pyrit"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-08T00:00:00+10:00"
---

Microsoft's open-source Python Risk Identification Tool for generative AI red teaming (docs version 1.1.0), including the CoPyRIT GUI and its use inside the Microsoft Foundry AI Red Teaming Agent.

Column group: Red teaming and testing. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 1 |
| not-covered | 6 |
| out-of-scope | 39 |

| Verification state | Cells |
| --- | --- |
| verified | 46 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| CoPyRIT GUI | 3p | Web interface for PyRIT for interactive attacks, history and export, deployable to Azure Container Apps. |
| Microsoft Foundry AI Red Teaming Agent | 3p | Foundry service that uses PyRIT attack strategies with Foundry risk and safety evaluators to scan models and Foundry agents. |
| PyRIT | 3p | MIT-licensed Python framework and scanner for automated and human-led red teaming of generative AI systems. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | out-of-scope | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | out-of-scope | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | out-of-scope | verified | yes |
| [A2A](c4-4.md) | Identity | out-of-scope | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | out-of-scope | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | out-of-scope | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | out-of-scope | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | out-of-scope | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | out-of-scope | verified | yes |
| [Inference](c2-2.md) | Runtime | out-of-scope | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | out-of-scope | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | out-of-scope | verified | yes |
| [Harness](c2-5.md) | Runtime | out-of-scope | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | out-of-scope | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | not-covered | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | out-of-scope | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | out-of-scope | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | out-of-scope | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | out-of-scope | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | not-covered | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | out-of-scope | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | out-of-scope | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | out-of-scope | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | covered | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | out-of-scope | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | out-of-scope | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | out-of-scope | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | out-of-scope | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | out-of-scope | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | out-of-scope | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | out-of-scope | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | out-of-scope | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | out-of-scope | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | out-of-scope | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | not-covered | verified | yes |

Sources are in the [source registry](sources.md).
