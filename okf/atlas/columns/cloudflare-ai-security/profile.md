---
type: "Platform profile"
title: "Cloudflare AI Gateway and Firewall for AI profile"
description: "Column profile for Cloudflare AI Gateway and Firewall for AI in the AI and MCP gateways group."
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
    locator: "platforms, id cloudflare-ai-security"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-08T00:00:00+10:00"
---

Cloudflare AI Gateway for model traffic, MCP server portals with Access and Gateway (including DLP and shadow MCP detection), and AI Security for Apps (formerly Firewall for AI) on the WAF, as documented at October 2026.

Column group: AI and MCP gateways. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 9 |
| not-covered | 23 |
| out-of-scope | 14 |

| Verification state | Cells |
| --- | --- |
| verified | 46 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Cloudflare AI Gateway | 3p | Proxy between applications and model providers with routing, rate and spend limits, Guardrails, DLP, logging and Access integration. |
| Cloudflare AI Security for Apps (formerly Firewall for AI) | 3p | WAF detections for prompt injection, PII and unsafe topics on LLM endpoints and public MCP servers. |
| Cloudflare Gateway (AI and MCP controls) | 3p | Secure web gateway with DLP, AI prompt protection, shadow IT analytics and MCP traffic detection. |
| Cloudflare MCP server portals | 3p | Single Access-protected endpoint that exposes curated tools from many MCP servers and holds upstream credentials. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | covered | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | covered | verified | yes |
| [A2A](c4-4.md) | Identity | out-of-scope | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | out-of-scope | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | not-covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | not-covered | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | out-of-scope | verified | yes |
| [Inference](c2-2.md) | Runtime | not-covered | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | not-covered | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | out-of-scope | verified | yes |
| [Harness](c2-5.md) | Runtime | covered | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | out-of-scope | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | not-covered | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | out-of-scope | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | not-covered | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | not-covered | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | not-covered | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | not-covered | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | not-covered | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | out-of-scope | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | out-of-scope | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | out-of-scope | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | not-covered | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | out-of-scope | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | covered | verified | yes |

Sources are in the [source registry](sources.md).
