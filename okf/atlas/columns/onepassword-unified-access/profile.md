---
type: "Platform profile"
title: "1Password Unified Access profile"
description: "Column profile for 1Password Unified Access in the Identity, access and secrets group."
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
    locator: "platforms, id onepassword-unified-access"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-08T00:00:00+10:00"
---

1Password's access platform for humans, AI agents and machines, covering Credential Broker, Privileged Access (Apono), SaaS Manager, Device Trust, Enterprise Password Manager and the developer AI integrations as documented in October 2026.

Column group: Identity, access and secrets. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 3 |
| not-covered | 25 |
| out-of-scope | 18 |

| Verification state | Cells |
| --- | --- |
| verified | 46 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| 1Password Credential Broker | 3p | Runtime credential delivery to verified workloads, in public preview for GitHub Actions with AI agent support planned. |
| 1Password developer AI integrations | 3p | Environments MCP server, agent hooks, NVIDIA OpenShell integration, Agentic Autofill and service accounts. |
| 1Password Device Trust | 3p | Endpoint posture checks with AI Insights for AI apps and MCP integrations. |
| 1Password Privileged Access | 3p | Just-in-time access and Agent Privilege Guard for AI agents, built on Apono. |
| 1Password SaaS Manager | 3p | SaaS and shadow AI discovery, app access governance and AI spend tracking. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | not-covered | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | not-covered | verified | yes |
| [A2A](c4-4.md) | Identity | out-of-scope | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | not-covered | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | not-covered | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | out-of-scope | verified | yes |
| [Inference](c2-2.md) | Runtime | out-of-scope | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | not-covered | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | out-of-scope | verified | yes |
| [Harness](c2-5.md) | Runtime | out-of-scope | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | out-of-scope | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | not-covered | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | out-of-scope | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | out-of-scope | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | out-of-scope | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | not-covered | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | out-of-scope | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | not-covered | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | not-covered | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | not-covered | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | out-of-scope | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | out-of-scope | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | not-covered | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | out-of-scope | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | out-of-scope | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | out-of-scope | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | not-covered | verified | yes |

Sources are in the [source registry](sources.md).
