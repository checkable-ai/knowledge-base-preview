---
type: "Platform profile"
title: "Google Workspace with Gemini profile"
description: "Column profile for Google Workspace with Gemini in the Enterprise and workplace agents group."
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
    locator: "platforms, id google-workspace-gemini"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

Gemini features built into Google Workspace (Gmail, Docs, Sheets, Drive, Meet, Chat), the Gemini app as a Workspace core service, Workspace Intelligence, Google Workspace Studio flows and the Admin console AI controls. Does not cover the Gemini API or Gemini Enterprise.

Column group: Enterprise and workplace agents. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 8 |
| escalated | 3 |
| not-covered | 17 |
| out-of-scope | 4 |
| partial | 14 |

| Verification state | Cells |
| --- | --- |
| agent-checked | 43 |
| contested | 3 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Admin console AI controls | 1p | Gemini feature toggles, conversation history settings, DLP for Gemini, audit logs, data regions and the AI control center. |
| Gemini app with enterprise data protections | 1p | The Gemini app (web, mobile and Chrome) offered as a Workspace core service on most business and enterprise editions. |
| Gemini in Workspace apps | 1p | Gemini side panel and generative AI features in Gmail, Docs, Sheets, Slides, Drive, Meet and Chat. |
| Workspace Intelligence | 1p | The retrieval layer that gives Gemini context from Gmail, Drive, Calendar and Chat under the user's own permissions. |
| Google Workspace Studio | 1p | No-code agent flows that act on a user's behalf across Workspace apps, with agent identity, access management and DLP controls. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | partial | agent-checked | yes |
| [Credential Brokerage](c4-2.md) | Identity | partial | agent-checked | yes |
| [Delegation (OBO)](c4-3.md) | Identity | covered | agent-checked | yes |
| [A2A](c4-4.md) | Identity | not-covered | agent-checked | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | out-of-scope | agent-checked | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | agent-checked | yes |
| [Human Approval](c1-3.md) | Authorisation | partial | agent-checked | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | partial | agent-checked | yes |
| [Agent Orchestration](c2-1.md) | Runtime | partial | agent-checked | yes |
| [Inference](c2-2.md) | Runtime | partial | agent-checked | yes |
| [Execution Environment](c2-3.md) | Runtime | out-of-scope | agent-checked | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | covered | agent-checked | yes |
| [Harness](c2-5.md) | Runtime | escalated | contested | no |
| [Agent Persistent Memory](c2-6.md) | Runtime | covered | agent-checked | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | partial | agent-checked | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | partial | agent-checked | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | covered | agent-checked | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [HITL](c5-1.md) | Observability & Explainability | partial | agent-checked | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | partial | agent-checked | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | out-of-scope | agent-checked | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | partial | agent-checked | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | out-of-scope | agent-checked | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | covered | agent-checked | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | partial | agent-checked | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | agent-checked | yes |
| [Posture & Reporting](c6-3.md) | Governance | escalated | contested | no |
| [Policy Management](c6-4.md) | Governance | not-covered | agent-checked | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | agent-checked | yes |
| [Ownership & Accountability](c6-6.md) | Governance | escalated | contested | no |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | agent-checked | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | agent-checked | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | agent-checked | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | covered | agent-checked | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | agent-checked | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | agent-checked | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | covered | agent-checked | yes |

Sources are in the [source registry](sources.md).
