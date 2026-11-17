---
type: "Platform profile"
title: "Firecrawl profile"
description: "Column profile for Firecrawl in the Agent web access group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "agent-web-access"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id firecrawl"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

Firecrawl's web search, scrape, crawl, map, Agent and Interact API with its hosted and open source MCP server, the self-hostable AGPL repository, and the Enterprise security controls (zero data retention, key and IP restrictions, Threat Protection and SIEM audit logging).

Column group: Agent web access. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 2 |
| escalated | 9 |
| not-covered | 25 |
| out-of-scope | 2 |
| partial | 8 |

| Verification state | Cells |
| --- | --- |
| agent-checked | 37 |
| contested | 9 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Firecrawl Cloud API | 3p | Hosted scrape, crawl, map, search, Agent and Interact API with dashboard, teams and API keys. |
| Firecrawl Enterprise controls | 3p | Zero data retention, PII redaction, key and IP restrictions, Threat Protection, SIEM audit logging, SSO and SCIM. |
| Firecrawl MCP server | 3p | Hosted and open source MCP server that exposes Firecrawl tools to agent clients with keyless, OAuth or API key access. |
| Firecrawl open source | 3p | AGPL-3.0 self-hostable core with Docker Compose, without Agent, Browser, Interact or enterprise controls. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | agent-checked | yes |
| [Credential Brokerage](c4-2.md) | Identity | partial | agent-checked | yes |
| [Delegation (OBO)](c4-3.md) | Identity | not-covered | agent-checked | yes |
| [A2A](c4-4.md) | Identity | not-covered | agent-checked | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | out-of-scope | agent-checked | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | agent-checked | yes |
| [Human Approval](c1-3.md) | Authorisation | escalated | contested | no |
| [Agent Provisioning](c1-4.md) | Authorisation | escalated | contested | no |
| [Agent Orchestration](c2-1.md) | Runtime | partial | agent-checked | yes |
| [Inference](c2-2.md) | Runtime | partial | agent-checked | yes |
| [Execution Environment](c2-3.md) | Runtime | partial | agent-checked | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | partial | agent-checked | yes |
| [Harness](c2-5.md) | Runtime | escalated | contested | no |
| [Agent Persistent Memory](c2-6.md) | Runtime | escalated | contested | no |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | partial | agent-checked | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | escalated | contested | no |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | escalated | contested | no |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | agent-checked | yes |
| [HITL](c5-1.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | partial | agent-checked | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | not-covered | agent-checked | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | escalated | contested | no |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | out-of-scope | agent-checked | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | partial | agent-checked | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | escalated | contested | no |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | agent-checked | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | not-covered | agent-checked | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | agent-checked | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | agent-checked | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | agent-checked | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | agent-checked | yes |
| [Ownership & Accountability](c6-6.md) | Governance | not-covered | agent-checked | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | agent-checked | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | agent-checked | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | agent-checked | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | covered | agent-checked | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | agent-checked | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | agent-checked | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | escalated | contested | no |

Sources are in the [source registry](sources.md).
