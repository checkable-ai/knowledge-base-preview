---
type: "Platform profile"
title: "Lovable profile"
description: "Column profile for Lovable in the App builders group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "approved"
verification: "not applicable"
tags:
  - "app-builders"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id lovable"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

Lovable's AI app builder and its Pro, Business and Enterprise workspace plans, covering the build agent and chat, Lovable Cloud backend, connectors and MCP, the Lovable API and MCP server, security scanning, workspace admin, identity, audit and trust material.

Column group: App builders. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 13 |
| escalated | 11 |
| not-covered | 12 |
| partial | 10 |

| Verification state | Cells |
| --- | --- |
| contested | 11 |
| verified | 35 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Lovable app builder | 3p | Prompt-driven agent (Chat, Plan and Build modes) that generates, edits and deploys full-stack web apps with a built-in backend or Supabase. |
| Lovable connectors, MCP and API | 3p | Connector gateway, chat connectors (MCP), Lovable MCP server, workspace API keys and OAuth clients. |
| Lovable security scanning and Trust center | 3p | Quick and Deep scans, Security center, Wiz and Aikido connectors and the per-app Trust center. |
| Lovable Business and Enterprise workspaces | 3p | Paid workspace plans adding SSO, groups, security centre, policies, audit logs, SCIM and regional controls. |

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
| [Agent Provisioning](c1-4.md) | Authorisation | escalated | contested | no |
| [Agent Orchestration](c2-1.md) | Runtime | covered | verified | yes |
| [Inference](c2-2.md) | Runtime | covered | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | not-covered | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | partial | verified | yes |
| [Harness](c2-5.md) | Runtime | covered | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | covered | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | partial | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | partial | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | partial | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | covered | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | escalated | contested | no |
| [Cost & Yield](c5-3.md) | Observability & Explainability | partial | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | covered | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | not-covered | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | partial | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | not-covered | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | escalated | contested | no |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | escalated | contested | no |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | partial | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | not-covered | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | partial | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | escalated | contested | no |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | escalated | contested | no |
| [Ownership & Accountability](c6-6.md) | Governance | escalated | contested | no |
| [Risk Assessment & Classification](c6-7.md) | Governance | escalated | contested | no |
| [Change & Release Governance](c6-8.md) | Governance | partial | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | escalated | contested | no |
| [Data Lifecycle Governance](c6-10.md) | Governance | covered | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | escalated | contested | no |
| [Third-Party Governance](c6-12.md) | Governance | escalated | contested | no |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | covered | verified | yes |

Sources are in the [source registry](sources.md).
