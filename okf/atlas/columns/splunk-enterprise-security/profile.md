---
type: "Platform profile"
title: "Splunk Enterprise Security profile"
description: "Column profile for Splunk Enterprise Security in the Security operations (SIEM, XDR) group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "secops"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id splunk-enterprise-security"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-08T00:00:00+10:00"
---

Cisco's Splunk SIEM (ES 8.7, Essentials and Premier editions) with Splunk SOAR, UEBA, Splunk Security Content, its AI agents and Security AI Assistant, the Splunk MCP Server ES tools, and the Observability Cloud AI Agent Monitoring and AI Security Monitoring features that feed agent telemetry into Splunk.

Column group: Security operations (SIEM, XDR). Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 6 |
| not-covered | 26 |
| out-of-scope | 14 |

| Verification state | Cells |
| --- | --- |
| verified | 46 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Splunk AI Agent Monitoring and AI Security Monitoring | 3p | Observability Cloud features for agent performance, tokens, cost, quality and Cisco AI Defense risk, scheduled for deprecation in favour of Splunk Agent Observability. |
| ES AI agents and Security AI Assistant | 3p | Triage agent, AI SOC Analyst, Detection Builder, Automation Builder and Connector Builder agents, and the Security AI Assistant running on Model Runtime. |
| Splunk Security Content (ESCU) | 3p | Splunk-maintained detections and analytic stories, including Cisco AI Defense alert and Ollama detections. |
| Splunk Enterprise Security | 3p | SIEM with findings, risk-based alerting, UEBA and audit dashboards, sold as Essentials and Premier editions. |
| Splunk MCP Server app (ES tools) | 3p | MCP server app that exposes read-only ES investigation, finding and AI analysis tools to external AI clients under Splunk RBAC. |
| Splunk SOAR | 3p | Playbook automation for ES, including Prompt blocks that pause a playbook for a human response. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | not-covered | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | covered | verified | yes |
| [A2A](c4-4.md) | Identity | not-covered | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | not-covered | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | not-covered | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | not-covered | verified | yes |
| [Inference](c2-2.md) | Runtime | not-covered | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | not-covered | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | out-of-scope | verified | yes |
| [Harness](c2-5.md) | Runtime | not-covered | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | out-of-scope | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | not-covered | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | out-of-scope | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | covered | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | not-covered | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | covered | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | not-covered | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | not-covered | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | out-of-scope | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | out-of-scope | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | not-covered | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | out-of-scope | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | out-of-scope | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | not-covered | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | out-of-scope | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | covered | verified | yes |

Sources are in the [source registry](sources.md).
