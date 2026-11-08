---
type: "Platform profile"
title: "Google Antigravity and Gemini Code Assist profile"
description: "Column profile for Google Antigravity and Gemini Code Assist in the Coding agents group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "coding-agents"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id google-antigravity"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-08T00:00:00+10:00"
---

Google's agentic development platform (Antigravity 2.0, Antigravity CLI, Antigravity for IDEs and the Antigravity SDK) as deployed through Gemini Enterprise AI developer tools, plus the Gemini Code Assist Standard and Enterprise editions now in sunset.

Column group: Coding agents. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 11 |
| not-covered | 31 |
| out-of-scope | 3 |
| partial | 1 |

| Verification state | Cells |
| --- | --- |
| verified | 46 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| Antigravity 2.0 | 1p | Desktop command centre that runs multiple local agents in parallel across projects and workspaces. |
| Antigravity CLI | 1p | Terminal coding agent with permissions, sandbox, subagents, hooks and a headless mode, replacing Gemini CLI. |
| Gemini Code Assist Standard and Enterprise | 1p | Earlier coding assistant editions managed through Google Cloud, closed to new purchases from 9 October 2026. |
| Gemini Enterprise AI developer tools | 1p | Gemini Enterprise admin settings, IAM roles, quotas, metrics and logging that govern Antigravity for licensed users. |
| Antigravity for IDEs | 1p | Agent extensions for VS Code, Visual Studio, JetBrains, Zed and Xcode, plus the standalone Antigravity IDE (not supported for enterprise). |
| Antigravity SDK | 1p | Python toolkit for building custom agents on the Antigravity harness with a declarative policy engine. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | not-covered | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | covered | verified | yes |
| [A2A](c4-4.md) | Identity | not-covered | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | covered | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | not-covered | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | covered | verified | yes |
| [Inference](c2-2.md) | Runtime | covered | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | covered | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | not-covered | verified | yes |
| [Harness](c2-5.md) | Runtime | covered | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | covered | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | covered | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | covered | verified | yes |
| [Behavioural](c5-2.md) | Observability & Explainability | not-covered | verified | yes |
| [Cost & Yield](c5-3.md) | Observability & Explainability | not-covered | verified | yes |
| [Infrastructure](c5-4.md) | Observability & Explainability | not-covered | verified | yes |
| [Connectivity](c5-5.md) | Observability & Explainability | not-covered | verified | yes |
| [Administrative Audit](c7-1.md) | Agentic MLSecOps | not-covered | verified | yes |
| [SOC Telemetry](c7-2.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Model Assurance](c7-3.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Runtime Assurance](c7-4.md) | Agentic MLSecOps | not-covered | verified | yes |
| [First-Party Tool Assurance](c7-5.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Third-Party Tool Assurance](c7-6.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | not-covered | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | not-covered | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | not-covered | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | out-of-scope | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | out-of-scope | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | partial | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | not-covered | verified | yes |

Sources are in the [source registry](sources.md).
