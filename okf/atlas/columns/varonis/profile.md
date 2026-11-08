---
type: "Platform profile"
title: "Varonis Atlas AI Security profile"
description: "Column profile for Varonis Atlas AI Security in the Data security for AI group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "data-security"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id varonis"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-08T00:00:00+10:00"
---

Varonis Atlas AI TRiSM platform (built on the AllTrue.ai acquisition announced February 2026) plus Varonis Data Security Platform coverage of Microsoft 365 Copilot, ChatGPT Enterprise and Salesforce Agentforce.

Column group: Data security for AI. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 10 |
| not-covered | 23 |
| out-of-scope | 13 |

| Verification state | Cells |
| --- | --- |
| verified | 46 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Varonis for Agentforce | 3p | Agentforce agent catalogue, access right-sizing and activity monitoring. |
| Varonis Atlas | 3p | AI inventory, AI-SPM, pen testing, runtime guardrails gateway, activity monitoring, AIDR, compliance and AI TPRM. |
| Varonis for ChatGPT Enterprise | 3p | Classification and monitoring of ChatGPT Enterprise prompts, uploads and admin changes through the Compliance API. |
| Varonis for Microsoft 365 Copilot | 3p | Copilot prompt monitoring, sensitive data exposure reduction, labelling and UBA alerts. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | not-covered | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | not-covered | verified | yes |
| [A2A](c4-4.md) | Identity | out-of-scope | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | out-of-scope | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | not-covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | not-covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | not-covered | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | out-of-scope | verified | yes |
| [Inference](c2-2.md) | Runtime | out-of-scope | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | out-of-scope | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | out-of-scope | verified | yes |
| [Harness](c2-5.md) | Runtime | out-of-scope | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | out-of-scope | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | not-covered | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | out-of-scope | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | not-covered | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | out-of-scope | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | out-of-scope | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | covered | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | covered | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | covered | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | covered | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | covered | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | not-covered | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | out-of-scope | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | not-covered | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | not-covered | verified | yes |

Sources are in the [source registry](sources.md).
