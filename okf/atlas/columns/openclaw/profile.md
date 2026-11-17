---
type: "Platform profile"
title: "OpenClaw profile"
description: "Column profile for OpenClaw in the Agent frameworks group."
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
    locator: "platforms, id openclaw"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

The open source (MIT) OpenClaw personal agent Gateway and runtime from the OpenClaw Foundation, with its sandboxing, tool policy, exec approvals, memory, A2A channel, Policy plugin, ClawHub skills and plugin registry, and the pre-1.0 OpenClaw Enterprise control plane.

Column group: Agent frameworks. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 16 |
| escalated | 4 |
| not-covered | 10 |
| partial | 16 |

| Verification state | Cells |
| --- | --- |
| contested | 4 |
| verified | 42 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| ClawHub | 3p | Public registry of skills and plugins with security audits, moderation and install tooling. |
| OpenClaw Enterprise | 3p | Pre-1.0 open source control plane for multi-tenant persistent agents, intended for internal pilots. |
| OpenClaw Gateway and agent runtime | 3p | Self-hosted Gateway that runs agents, channels, tools, sandboxes, memory and the operator control plane. |
| OpenClaw Policy plugin and security audit | 3p | Conformance checks, attestation and the openclaw security audit command. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | partial | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | partial | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | covered | verified | yes |
| [A2A](c4-4.md) | Identity | covered | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | covered | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | covered | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | covered | verified | yes |
| [Inference](c2-2.md) | Runtime | covered | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | covered | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | covered | verified | yes |
| [Harness](c2-5.md) | Runtime | covered | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | covered | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | covered | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | partial | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | covered | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | escalated | contested | no |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | partial | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | covered | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | partial | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | covered | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | not-covered | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | partial | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | escalated | contested | no |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | partial | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | partial | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | escalated | contested | no |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | partial | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | escalated | contested | no |
| [Posture & Reporting](c6-3.md) | Governance | partial | verified | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | partial | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | partial | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | partial | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | partial | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | partial | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | partial | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | not-covered | verified | yes |

Sources are in the [source registry](sources.md).
