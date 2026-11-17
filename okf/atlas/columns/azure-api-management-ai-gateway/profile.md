---
type: "Platform profile"
title: "Azure API Management AI Gateway profile"
description: "Column profile for Azure API Management AI Gateway in the AI and MCP gateways group."
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
    locator: "platforms, id azure-api-management-ai-gateway"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

Microsoft's AI gateway capabilities in Azure API Management (LLM APIs, remote MCP servers, A2A agent APIs), the AI Gateway tier in public preview, and the Agent 365 integration, with Azure API Center as the registry.

Column group: AI and MCP gateways. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 11 |
| escalated | 4 |
| not-covered | 17 |
| out-of-scope | 5 |
| partial | 9 |

| Verification state | Cells |
| --- | --- |
| agent-checked | 42 |
| contested | 4 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Microsoft Agent 365 integration (preview) | 3p | Discovers gateway MCP servers, blocks servers or tools and adds Defender and Purview tool threat protection. |
| AI Gateway tier (preview) | 3p | Dedicated AI Gateway resource for models and MCP servers with policy cards, runtime keys and OpenTelemetry metrics, in East US 2 and Sweden Central. |
| Azure API Center | 3p | Registry of APIs, MCP servers and other assets with metadata and a discovery portal. |
| Azure API Management AI gateway capabilities | 3p | Policies for LLM token limits, content safety, semantic caching and routing, plus MCP server and A2A agent API governance, on classic and v2 tiers. |

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
| [Agent Provisioning](c1-4.md) | Authorisation | not-covered | agent-checked | yes |
| [Agent Orchestration](c2-1.md) | Runtime | out-of-scope | agent-checked | yes |
| [Inference](c2-2.md) | Runtime | covered | agent-checked | yes |
| [Execution Environment](c2-3.md) | Runtime | out-of-scope | agent-checked | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | out-of-scope | agent-checked | yes |
| [Harness](c2-5.md) | Runtime | escalated | contested | no |
| [Agent Persistent Memory](c2-6.md) | Runtime | out-of-scope | agent-checked | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | partial | agent-checked | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | covered | agent-checked | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | covered | agent-checked | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | partial | agent-checked | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | covered | agent-checked | yes |
| [HITL](c5-1.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | partial | agent-checked | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | covered | agent-checked | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | covered | agent-checked | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | partial | agent-checked | yes |
| [Posture & Reporting](c6-3.md) | Governance | escalated | contested | no |
| [Policy Management](c6-4.md) | Governance | not-covered | agent-checked | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | partial | agent-checked | yes |
| [Ownership & Accountability](c6-6.md) | Governance | covered | agent-checked | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | agent-checked | yes |
| [Change & Release Governance](c6-8.md) | Governance | partial | agent-checked | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | agent-checked | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | not-covered | agent-checked | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | partial | agent-checked | yes |
| [Third-Party Governance](c6-12.md) | Governance | escalated | contested | no |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | escalated | contested | no |

Sources are in the [source registry](sources.md).
