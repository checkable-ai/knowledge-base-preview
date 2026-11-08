---
type: "Platform profile"
title: "LiteLLM profile"
description: "Column profile for LiteLLM in the Agent frameworks group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "agent-frameworks"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id litellm"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-08T00:00:00+10:00"
---

LiteLLM is an open-source, self-hosted AI gateway (proxy) from BerriAI that fronts model providers, MCP servers and A2A agents. This research covers the open-source proxy and the features gated behind a LiteLLM Enterprise licence, as documented on docs.litellm.ai.

Column group: Agent frameworks. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 12 |
| not-covered | 30 |
| out-of-scope | 4 |

| Verification state | Cells |
| --- | --- |
| verified | 46 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| LiteLLM Agent Gateway (A2A) | 3p | Registry and proxy for A2A agents with key and team access control, per-session iteration and budget caps and a kill switch webhook. |
| LiteLLM Enterprise | 3p | Licence-gated features on the same self-hosted proxy, including SSO, JWT auth, RBAC, audit logs, secret managers, key rotation and per key or team guardrails. |
| LiteLLM MCP Gateway | 3p | MCP server registry and proxy with per key, team and organisation tool permissions, OAuth and OBO auth, and MCP guardrails. |
| LiteLLM Proxy (AI Gateway) | 3p | Open-source OpenAI-compatible gateway with virtual keys, budgets, rate limits, routing, fallbacks, guardrails and logging callbacks. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | covered | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | covered | verified | yes |
| [A2A](c4-4.md) | Identity | covered | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | not-covered | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | not-covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | covered | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | not-covered | verified | yes |
| [Inference](c2-2.md) | Runtime | covered | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | out-of-scope | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | not-covered | verified | yes |
| [Harness](c2-5.md) | Runtime | covered | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | not-covered | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | not-covered | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | not-covered | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | not-covered | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | covered | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | not-covered | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | not-covered | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | not-covered | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | covered | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | not-covered | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | out-of-scope | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | not-covered | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | covered | verified | yes |

Sources are in the [source registry](sources.md).
