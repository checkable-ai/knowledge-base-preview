---
type: "Platform profile"
title: "Microsoft Security Copilot profile"
description: "Column profile for Microsoft Security Copilot in the Security operations (SIEM, XDR) group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "approved"
verification: "not applicable"
tags:
  - "secops"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id microsoft-security-copilot"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

Microsoft Security Copilot, the generative AI security assistant and agents (including the Phishing and Security Alert Triage agents in Defender, and Entra, Intune and Purview agents) billed in Security Compute Units, with its roles, plugins, data privacy settings and audit log. Core's microsoft-sentinel entry does not cover it.

Column group: Security operations (SIEM, XDR). Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 12 |
| escalated | 9 |
| not-covered | 15 |
| out-of-scope | 1 |
| partial | 9 |

| Verification state | Cells |
| --- | --- |
| contested | 9 |
| verified | 37 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Security Copilot agents | 3p | Microsoft-built, partner-built and custom agents, including the Phishing Triage and Security Alert Triage agents in Microsoft Defender. |
| Microsoft Security Copilot platform | 3p | Standalone portal and embedded experiences with chat, promptbooks, plugins and owner settings, billed in Security Compute Units. |
| Security Copilot plugins and connectors | 3p | Microsoft and non-Microsoft plugins, custom plugins and the Logic Apps and Copilot Studio connectors. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | partial | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | partial | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | covered | verified | yes |
| [A2A](c4-4.md) | Identity | not-covered | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | out-of-scope | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | covered | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | partial | verified | yes |
| [Inference](c2-2.md) | Runtime | covered | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | escalated | contested | no |
| [Agent In-Session Memory](c2-4.md) | Runtime | covered | verified | yes |
| [Harness](c2-5.md) | Runtime | covered | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | covered | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | partial | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | escalated | contested | no |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | partial | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | partial | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | covered | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | partial | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | covered | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | escalated | contested | no |
| [Connectivity](c5-5.md) | Observability & Explainability | escalated | contested | no |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | partial | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | escalated | contested | no |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | escalated | contested | no |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | not-covered | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | partial | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | escalated | contested | no |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | not-covered | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | covered | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | escalated | contested | no |
| [Third-Party Governance](c6-12.md) | Governance | escalated | contested | no |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | covered | verified | yes |

Sources are in the [source registry](sources.md).
