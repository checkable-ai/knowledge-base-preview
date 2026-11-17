---
type: "Platform profile"
title: "Portkey (now Prisma AIRS AI Gateway) profile"
description: "Column profile for Portkey (now Prisma AIRS AI Gateway) in the AI and MCP gateways group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "ai-gateways"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id portkey"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

Portkey's hosted AI gateway and control plane (LLM routing, MCP gateway, agent gateway, guardrails, observability, prompt management) and its MIT-licensed open source gateway that teams host themselves, from portkey.ai pages and its GitHub.

Column group: AI and MCP gateways. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 10 |
| escalated | 13 |
| not-covered | 12 |
| out-of-scope | 2 |
| partial | 9 |

| Verification state | Cells |
| --- | --- |
| agent-checked | 33 |
| contested | 13 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Portkey Agent Gateway | 3p | Registry and proxy giving access control and logging for A2A agent servers. |
| Portkey Enterprise hybrid deployment | 3p | Gateway and data plane in the customer environment with a Portkey-managed control plane. |
| Portkey hosted gateway and control plane | 3p | Managed AI gateway with Dev, Pro and Enterprise plans covering routing, guardrails, observability, prompts and org administration. |
| Portkey MCP Gateway | 3p | Proxy with authentication, access control, guardrails, rate limits and logging for MCP servers. |
| Portkey open source AI Gateway | 3p | MIT-licensed gateway run locally or self-hosted for routing, retries, fallbacks and basic guardrails. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | agent-checked | yes |
| [Credential Brokerage](c4-2.md) | Identity | covered | agent-checked | yes |
| [Delegation (OBO)](c4-3.md) | Identity | covered | agent-checked | yes |
| [A2A](c4-4.md) | Identity | covered | agent-checked | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | out-of-scope | agent-checked | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | agent-checked | yes |
| [Human Approval](c1-3.md) | Authorisation | not-covered | agent-checked | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | escalated | contested | no |
| [Agent Orchestration](c2-1.md) | Runtime | escalated | contested | no |
| [Inference](c2-2.md) | Runtime | covered | agent-checked | yes |
| [Execution Environment](c2-3.md) | Runtime | out-of-scope | agent-checked | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | escalated | contested | no |
| [Harness](c2-5.md) | Runtime | escalated | contested | no |
| [Agent Persistent Memory](c2-6.md) | Runtime | escalated | contested | no |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | escalated | contested | no |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | covered | agent-checked | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | covered | agent-checked | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | partial | agent-checked | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | escalated | contested | no |
| [HITL](c5-1.md) | Observability & Explainability | partial | agent-checked | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | escalated | contested | no |
| [Cost & Yield](c5-3.md) | Observability & Explainability | partial | agent-checked | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | partial | agent-checked | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | partial | agent-checked | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | escalated | contested | no |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | escalated | contested | no |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | escalated | contested | no |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | escalated | contested | no |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | covered | agent-checked | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | partial | agent-checked | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | agent-checked | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | agent-checked | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | agent-checked | yes |
| [Ownership & Accountability](c6-6.md) | Governance | not-covered | agent-checked | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | agent-checked | yes |
| [Change & Release Governance](c6-8.md) | Governance | partial | agent-checked | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | escalated | contested | no |
| [Data Lifecycle Governance](c6-10.md) | Governance | covered | agent-checked | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | agent-checked | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | agent-checked | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | covered | agent-checked | yes |

Sources are in the [source registry](sources.md).
