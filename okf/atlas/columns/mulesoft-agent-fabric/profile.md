---
type: "Platform profile"
title: "MuleSoft Agent Fabric and Omni Gateway profile"
description: "Column profile for MuleSoft Agent Fabric and Omni Gateway in the AI and MCP gateways group."
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
    locator: "platforms, id mulesoft-agent-fabric"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-08T00:00:00+10:00"
---

MuleSoft's (Salesforce) Agent Fabric (Agent Registry and provider scanners, Agent Broker, Agent Visualizer, rogue agent detection and kill switch, external vault credentials) and Omni Gateway (Model Proxy, MCP, A2A and LLM policies), with the MCP Bridge, MCP and A2A connectors and Australia Cloud hosting. The Salesforce Agentforce column (salesforce) also holds earlier MuleSoft Agent Fabric findings for c3-4, c4-4, c5-5, c6-1 and c7-9.

Column group: AI and MCP gateways. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 10 |
| not-covered | 31 |
| out-of-scope | 5 |

| Verification state | Cells |
| --- | --- |
| verified | 46 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| MuleSoft AI Chain, Inference and Vectors connectors | 3p | Mule connectors for agent, chat, RAG and tool operations, model inference across many providers and external vector stores. |
| MuleSoft Agent Broker and agent networks | 3p | Agent network projects that route work across A2A agents and tools, defined in agent-network.yaml and Agent Script broker files. |
| MuleSoft MCP Bridge, MCP Connector, A2A Bridge and A2A Connector | 3p | Routes for exposing APIs and Mule apps as MCP servers or clients and joining agents to an A2A network. |
| MuleSoft Model Proxy | 3p | Omni Gateway endpoint for multiple LLM providers with model and semantic routing, fallback, semantic caching and model wallets. |
| MuleSoft Omni Gateway | 3p | API, agent and MCP gateway (formerly Flex Gateway) in managed, connected and local modes, with MCP, A2A and LLM policies. |
| MuleSoft Agent Registry and provider scanners | 3p | Exchange catalogue of agents, MCP servers, APIs, model proxies and gateways, populated by scheduled or on-demand provider scans. |
| MuleSoft rogue agent detection, kill switch and external vaults | 3p | Model proxy policies that flag risky agent behaviour and block quarantined agents, plus zero-copy credentials from AWS, Azure and HashiCorp vaults. |
| MuleSoft Agent Visualizer | 3p | Map of agents, brokers, MCP servers and LLMs with live request flows and latency, throughput and error metrics. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | not-covered | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | covered | verified | yes |
| [A2A](c4-4.md) | Identity | covered | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | out-of-scope | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | not-covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | not-covered | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | not-covered | verified | yes |
| [Inference](c2-2.md) | Runtime | not-covered | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | not-covered | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | not-covered | verified | yes |
| [Harness](c2-5.md) | Runtime | not-covered | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | not-covered | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | not-covered | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | not-covered | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | covered | verified | yes |
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
| [AI Discovery](c7-9.md) | Agentic MLSecOps | covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | covered | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | not-covered | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | out-of-scope | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | out-of-scope | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | not-covered | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | covered | verified | yes |

Sources are in the [source registry](sources.md).
