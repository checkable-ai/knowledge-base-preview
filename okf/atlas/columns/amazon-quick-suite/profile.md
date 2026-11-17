---
type: "Platform profile"
title: "Amazon Quick Suite (Amazon Quick) profile"
description: "Column profile for Amazon Quick Suite (Amazon Quick) in the Enterprise and workplace agents group."
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
    locator: "platforms, id amazon-quick-suite"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

Amazon Web Services' Amazon Quick (previously Amazon Quick Suite), an agentic workplace assistant covering chat and custom agents, Spaces and knowledge bases (Quick Index), Quick Flows, Quick Automate, Quick Sight dashboards, Quick Desktop, extensions, MCP and other connectors, and the account admin, identity, audit and security controls.

Column group: Enterprise and workplace agents. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 16 |
| escalated | 7 |
| not-covered | 11 |
| out-of-scope | 2 |
| partial | 10 |

| Verification state | Cells |
| --- | --- |
| agent-checked | 39 |
| contested | 7 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Quick Flows and Quick Automate | 3p | Personal and team flows plus enterprise process automations with agents, code actions and human-in-the-loop tasks. |
| Quick chat, agents and Spaces | 3p | Chat assistant with system and custom agents, Spaces, knowledge bases and Research, grounded in connected content. |
| Quick connectors, MCP and extensions | 3p | Action connectors from OpenAPI and MCP servers, Agent Registry integration and extensions for Office, Slack, Teams and browsers. |
| Quick Desktop | 3p | Desktop app with system tools, local code execution sandbox, memory and per-operation permissions. |
| Quick Sight and Q in Quick | 3p | Dashboards, analytics and generative BI with row and column level security. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | agent-checked | yes |
| [Credential Brokerage](c4-2.md) | Identity | partial | agent-checked | yes |
| [Delegation (OBO)](c4-3.md) | Identity | covered | agent-checked | yes |
| [A2A](c4-4.md) | Identity | escalated | contested | no |
| [Agent Local Scopes](c1-1.md) | Authorisation | covered | agent-checked | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | agent-checked | yes |
| [Human Approval](c1-3.md) | Authorisation | escalated | contested | no |
| [Agent Provisioning](c1-4.md) | Authorisation | covered | agent-checked | yes |
| [Agent Orchestration](c2-1.md) | Runtime | covered | agent-checked | yes |
| [Inference](c2-2.md) | Runtime | partial | agent-checked | yes |
| [Execution Environment](c2-3.md) | Runtime | covered | agent-checked | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | covered | agent-checked | yes |
| [Harness](c2-5.md) | Runtime | covered | agent-checked | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | covered | agent-checked | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | covered | agent-checked | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | covered | agent-checked | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | escalated | contested | no |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [HITL](c5-1.md) | Observability & Explainability | covered | agent-checked | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | partial | agent-checked | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | partial | agent-checked | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | covered | agent-checked | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | out-of-scope | agent-checked | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | out-of-scope | agent-checked | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | escalated | contested | no |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | partial | agent-checked | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | escalated | contested | no |
| [Posture & Reporting](c6-3.md) | Governance | partial | agent-checked | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | agent-checked | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | partial | agent-checked | yes |
| [Ownership & Accountability](c6-6.md) | Governance | covered | agent-checked | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | agent-checked | yes |
| [Change & Release Governance](c6-8.md) | Governance | partial | agent-checked | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | escalated | contested | no |
| [Data Lifecycle Governance](c6-10.md) | Governance | covered | agent-checked | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | agent-checked | yes |
| [Third-Party Governance](c6-12.md) | Governance | escalated | contested | no |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | covered | agent-checked | yes |

Sources are in the [source registry](sources.md).
