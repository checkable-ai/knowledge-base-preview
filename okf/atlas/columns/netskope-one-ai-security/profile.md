---
type: "Platform profile"
title: "Netskope One AI Security profile"
description: "Column profile for Netskope One AI Security in the AI usage control (SASE, browser, DLP) group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "ai-usage-control"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id netskope-one-ai-security"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-08T00:00:00+10:00"
---

Netskope's AI security suite launched March 2026, covering Agentic Broker for MCP traffic, AI Guardrails, AI Gateway with MCP Gateway, AI Red Teaming and Agent Action Control (beta).

Column group: AI usage control (SASE, browser, DLP). Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 7 |
| not-covered | 20 |
| out-of-scope | 19 |

| Verification state | Cells |
| --- | --- |
| verified | 46 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Netskope Agent Action Control | 3p | Beta policy control over high-impact AI agent actions in connected SaaS apps. |
| Netskope One Agentic Broker | 3p | Inline visibility, DLP and real-time protection policies for MCP client to server traffic, with an MCP server risk catalog. |
| Netskope One AI Gateway | 3p | Self-hosted gateway appliance between agents and LLMs or MCP servers with token auth, rate limits, DLP and guardrails. |
| Netskope One AI Guardrails | 3p | Prompt and response moderation for prompt injection, jailbreaks and harmful content, inline or via an on-demand API. |
| Netskope One AI Red Teaming | 3p | Automated adversarial prompt testing of LLM and REST targets with attack success rate reporting and drift tracking. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | not-covered | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | not-covered | verified | yes |
| [A2A](c4-4.md) | Identity | not-covered | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | out-of-scope | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | not-covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | out-of-scope | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | out-of-scope | verified | yes |
| [Inference](c2-2.md) | Runtime | covered | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | out-of-scope | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | out-of-scope | verified | yes |
| [Harness](c2-5.md) | Runtime | out-of-scope | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | out-of-scope | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | not-covered | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | out-of-scope | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | not-covered | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | out-of-scope | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | not-covered | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | covered | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | not-covered | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | out-of-scope | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | out-of-scope | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | out-of-scope | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | out-of-scope | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | out-of-scope | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | out-of-scope | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | out-of-scope | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | not-covered | verified | yes |

Sources are in the [source registry](sources.md).
