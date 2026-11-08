---
type: "Platform profile"
title: "Wiz profile"
description: "Column profile for Wiz in the AI security group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "ai-security"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id wiz"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-08T00:00:00+10:00"
---

Cloud security platform, a Google company since March 2026, researched for its AI security offerings: the AI Application Protection Platform (AI-APP) with AI-SPM and AI inventory, Wiz Defend with the Runtime Sensor, the Sensor for Developer Workstations, Wiz Code, Wiz Workflows and the Blue, Green and Red agents, from public wiz.io pages because docs.wiz.io requires a login.

Column group: AI security. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 9 |
| not-covered | 29 |
| out-of-scope | 8 |

| Verification state | Cells |
| --- | --- |
| verified | 46 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Wiz AI Application Protection Platform (AI-APP) | 3p | Graph-based AI security platform launched in 2026 that combines AI-SPM visibility, cross-layer risk analysis and runtime threat detection for AI applications. |
| Wiz AI Security Posture Management (AI-SPM) | 3p | Agentless AI discovery, AI inventory and AI-BOM, agent, tool and MCP mapping, AI security rules, AI attack paths and DSPM for AI. |
| Wiz Code | 3p | Code security with rule-based and AI SAST, IDE and coding agent plugins, skills and git-boundary hooks, and the Unified Policy Engine. |
| Wiz Defend | 3p | Cloud detection and response combining Runtime Sensor signals, cloud and SaaS logs and agentless context, with Blue Agent investigation and Wiz Workflows response. |
| Wiz Red Agent | 3p | Generally available AI-driven continuous external penetration testing of custom applications and APIs. |
| Wiz Runtime Sensor | 3p | eBPF workload sensor for Linux and Windows VMs, Kubernetes and serverless containers that detects, blocks and captures forensics for runtime threats, including on AI workloads. |
| Wiz Workflows | 3p | Automation that chains triggers, conditions, approvals, notifications, Wiz AI Agents and remediation actions into multi-step security processes. |
| Wiz Sensor for Developer Workstations | 3p | Private Preview sensor for Windows and macOS developer machines that inventories packages, secrets, IDE extensions, AI coding agents, skills, MCP servers and models and detects supply chain attacks. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | not-covered | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | not-covered | verified | yes |
| [A2A](c4-4.md) | Identity | not-covered | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | not-covered | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | not-covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | not-covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | not-covered | verified | yes |
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
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | out-of-scope | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | covered | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | out-of-scope | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | not-covered | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | covered | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | covered | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | not-covered | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | covered | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | covered | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | not-covered | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | covered | verified | yes |

Sources are in the [source registry](sources.md).
