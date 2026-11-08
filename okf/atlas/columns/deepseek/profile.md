---
type: "Platform profile"
title: "DeepSeek profile"
description: "Column profile for DeepSeek in the Frontier AI providers group."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "frontier-ai"
  - "profile"
sources:
  - id: "atlas-catalogue"
    resource: "data/catalog.json"
    locator: "platforms, id deepseek"
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-08T00:00:00+10:00"
---

Chinese model lab (Hangzhou DeepSeek Artificial Intelligence Co., Ltd.). This research covers the DeepSeek API (deepseek-flash and deepseek-v4-pro), DeepSeek Harness and the open-weight V4 models. Its privacy policy says personal data is collected, processed and stored in the People's Republic of China, and the Open Platform terms are governed by PRC law. Australian PSPF Direction 001-2025 (Home Affairs, 4 February 2025) requires non-corporate Commonwealth entities to identify and remove all DeepSeek products, applications and web services and prevent their access, use or installation on government systems and devices, with exemptions limited to national security and regulatory functions. Open-source models deployed locally on a government system with mitigations fall outside the direction.

Column group: Frontier AI providers. Facts are agent-run. Cells listed as eligible are the only ones agents may retrieve.

## Verdicts and states

| Verdict | Cells |
| --- | --- |
| covered | 3 |
| not-covered | 40 |
| out-of-scope | 1 |
| partial | 2 |

| Verification state | Cells |
| --- | --- |
| verified | 46 |

## Products

| Product | Party | Description |
| --- | --- | --- |
| DeepSeek API (Open Platform) | 1p | Hosted OpenAI and Anthropic compatible API for DeepSeek models. |
| DeepSeek Harness (dsh) | 1p | MIT-licensed developer-preview agent harness with web UI and CLI that runs on the user's host. |
| DeepSeek open-weight models (self-hosted) | 3p | MIT-licensed V4 weights on Hugging Face run on customer or third-party infrastructure. |

## Cells

| Control | Category | Verdict | State | Agent-eligible |
| --- | --- | --- | --- | --- |
| [Agent ID](c4-1.md) | Identity | not-covered | verified | yes |
| [Credential Brokerage](c4-2.md) | Identity | not-covered | verified | yes |
| [Delegation (OBO)](c4-3.md) | Identity | not-covered | verified | yes |
| [A2A](c4-4.md) | Identity | not-covered | verified | yes |
| [Agent Local Scopes](c1-1.md) | Authorisation | partial | verified | yes |
| [Agent Remote Scopes](c1-2.md) | Authorisation | not-covered | verified | yes |
| [Human Approval](c1-3.md) | Authorisation | covered | verified | yes |
| [Agent Provisioning](c1-4.md) | Authorisation | not-covered | verified | yes |
| [Agent Orchestration](c2-1.md) | Runtime | covered | verified | yes |
| [Inference](c2-2.md) | Runtime | not-covered | verified | yes |
| [Execution Environment](c2-3.md) | Runtime | not-covered | verified | yes |
| [Agent In-Session Memory](c2-4.md) | Runtime | not-covered | verified | yes |
| [Harness](c2-5.md) | Runtime | covered | verified | yes |
| [Agent Persistent Memory](c2-6.md) | Runtime | not-covered | verified | yes |
| [Execution Containment & Kill Switch](c2-7.md) | Runtime | partial | verified | yes |
| [Model Gateway](c3-1.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Tool Gateway](c3-2.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [Data Gateway](c3-3.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [A2A Gateway](c3-4.md) | Mediation / Policy Enforcement | not-covered | verified | yes |
| [HITL](c5-1.md) | Observability & Explainability | not-covered | verified | yes |
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
| [Data & Feature Stores](c7-8.md) | Agentic MLSecOps | out-of-scope | verified | yes |
| [AI Discovery](c7-9.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Automated AI Pen-Testing](c7-10.md) | Agentic MLSecOps | not-covered | verified | yes |
| [Asset Registries & Inventory](c6-1.md) | Governance | not-covered | verified | yes |
| [Registration & Approval Workflows](c6-2.md) | Governance | not-covered | verified | yes |
| [Posture & Reporting](c6-3.md) | Governance | not-covered | verified | yes |
| [Policy Management](c6-4.md) | Governance | not-covered | verified | yes |
| [AI Lifecycle Management](c6-5.md) | Governance | not-covered | verified | yes |
| [Ownership & Accountability](c6-6.md) | Governance | not-covered | verified | yes |
| [Risk Assessment & Classification](c6-7.md) | Governance | not-covered | verified | yes |
| [Change & Release Governance](c6-8.md) | Governance | not-covered | verified | yes |
| [Exceptions & Risk Acceptance](c6-9.md) | Governance | not-covered | verified | yes |
| [Data Lifecycle Governance](c6-10.md) | Governance | not-covered | verified | yes |
| [Assurance & Compliance Evidence](c6-11.md) | Governance | not-covered | verified | yes |
| [Third-Party Governance](c6-12.md) | Governance | not-covered | verified | yes |
| [Independent Assurance & Authorisation](c6-13.md) | Governance | not-covered | verified | yes |

Sources are in the [source registry](sources.md).
