---
type: "Platform profile"
title: "Idira (CyberArk) Secure AI Agents profile"
description: "Column profile for Idira (CyberArk) Secure AI Agents in the Identity, access and secrets group."
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
    locator: "platforms, id idira-cyberark"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-08T00:00:00+10:00"
---

Palo Alto Networks identity security platform built on CyberArk (acquisition completed 11 February 2026), researched for Secure AI Agents (Managed AI agents, Identity Broker, MCP server inventory, AI agent access policies), the Discovery and Context AI agents inventory, Secure Infrastructure Access ZSP database access, Secrets Manager SaaS with Secure Workload Access, and the open-source Agent Guard.

Column group: Identity, access and secrets. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 7 |
| not-covered | 25 |
| out-of-scope | 14 |

| Verification state | Cells |
| --- | --- |
| verified | 46 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| CyberArk Agent Guard | 3p | Apache-2.0 toolset for agent secrets retrieval from external secret providers and an MCP proxy for traceability of agent MCP communications. |
| Idira Discovery and Context AI agents inventory | 3p | Discovers AI agents through AWS Bedrock, AWS AgentCore and Azure scanners or an external API and raises risks such as unmanaged agent and missing owner. |
| Idira Secrets Manager SaaS with Secure Workload Access | 3p | Secrets management (formerly Conjur Cloud) with SPIFFE workload identities, extended in August 2026 to AI agents on Google Gemini Enterprise Agent Platform. |
| Idira Secure AI Agents | 3p | Registers AI agents and MCP servers, issues agent OAuth 2.1 credentials and routes MCP traffic through the Identity Broker under deny-by-default access policies with audit. |
| Idira Secure Infrastructure Access (SIA) and SIA MCP server | 3p | Zero standing privilege access to PostgreSQL and SQL Server databases using ephemeral users, exposed to managed AI agents through the SIA MCP server. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | covered | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | not-covered | verified | yes |
| [A2A](c4-4.md) | Identity | not-covered | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | not-covered | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | not-covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | covered | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | out-of-scope | verified | yes |
| [Inference](c2-2.md) | Runtime | out-of-scope | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | out-of-scope | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | out-of-scope | verified | yes |
| [Harness](c2-5.md) | Runtime | out-of-scope | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | out-of-scope | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | not-covered | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | out-of-scope | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | out-of-scope | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | out-of-scope | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | covered | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | covered | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | covered | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | out-of-scope | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | not-covered | verified | yes |

Sources are in the [source registry](sources.md).
