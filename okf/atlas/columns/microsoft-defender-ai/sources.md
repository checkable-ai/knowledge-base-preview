---
type: "Registry"
title: "Microsoft Defender for AI and Defender XDR source registry"
description: "Sources cited by the Microsoft Defender for AI and Defender XDR column, with tiers and check dates."
classification: "C1"
owner: "agent:curator"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "secops"
  - "sources"
sources:
  - id: "confirm-d6b48ab34331"
    resource: "https://learn.microsoft.com/en-us/defender-endpoint/local-agent-discovery-overview"
    locator: "registry entry"
    tier: null
  - id: "microsoft-defender-ai-01"
    resource: "https://learn.microsoft.com/en-us/azure/defender-for-cloud/ai-threat-protection"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-02"
    resource: "https://learn.microsoft.com/en-us/azure/defender-for-cloud/ai-security-posture"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-04"
    resource: "https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-real-time-protection"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-05"
    resource: "https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-detection-protection"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-06"
    resource: "https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-inventory"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-07"
    resource: "https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-risk-assessment"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-08"
    resource: "https://learn.microsoft.com/en-us/security/security-for-ai/security-dashboard-for-ai"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-10"
    resource: "https://learn.microsoft.com/en-us/azure/defender-for-cloud/alerts-ai-workloads"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-11"
    resource: "https://learn.microsoft.com/en-us/azure/defender-for-cloud/ai-model-security"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-12"
    resource: "https://learn.microsoft.com/en-us/defender-endpoint/ai-agent-runtime-protection-overview"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-13"
    resource: "https://learn.microsoft.com/en-us/defender-endpoint/local-agent-discovery-overview"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-14"
    resource: "https://learn.microsoft.com/en-us/defender-endpoint/discover-local-ai-agents"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-15"
    resource: "https://learn.microsoft.com/en-us/defender-cloud-apps/applications-inventory"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-16"
    resource: "https://learn.microsoft.com/en-us/defender-cloud-apps/governance-discovery"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-17"
    resource: "https://learn.microsoft.com/en-us/azure/defender-for-cloud/governance-rules"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-18"
    resource: "https://learn.microsoft.com/en-us/azure/defender-for-cloud/exempt-resource"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-19"
    resource: "https://learn.microsoft.com/en-us/azure/defender-for-cloud/concept-regulatory-compliance-standards"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-20"
    resource: "https://learn.microsoft.com/en-us/azure/defender-for-cloud/gain-end-user-context-ai"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-r18-01"
    resource: "https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-real-time-protection"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-r18-02"
    resource: "https://learn.microsoft.com/en-us/defender-endpoint/ai-agent-runtime-protection-overview"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-r18-03"
    resource: "https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-detection-protection"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-r18-04"
    resource: "https://learn.microsoft.com/en-us/compliance/regulatory/offering-irap-australia"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-r18-05"
    resource: "https://learn.microsoft.com/en-us/azure/compliance/offerings/offering-australia-irap"
    locator: "registry entry"
    tier: 1
  - id: "microsoft-defender-ai-r18-06"
    resource: "https://learn.microsoft.com/en-us/defender-endpoint/data-storage-privacy"
    locator: "registry entry"
    tier: 1
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-08T00:00:00+10:00"
---

Every source the Microsoft Defender for AI and Defender XDR cells cite, with its tier from the atlas source register. Tier 1 and 2 sources can verify a claim within their subject. Tier 3 can only hold it as provisional.

### confirm-d6b48ab34331

- Title: Quoted by the confirm agents
- URL: https://learn.microsoft.com/en-us/defender-endpoint/local-agent-discovery-overview
- Tier: not yet assigned
- Checked: not recorded
- Cited by: [c5-5](c5-5.md)

### microsoft-defender-ai-01

- Title: AI threat protection in Microsoft Defender for Cloud
- URL: https://learn.microsoft.com/en-us/azure/defender-for-cloud/ai-threat-protection
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c7-2](c7-2.md)

### microsoft-defender-ai-02

- Title: Overview - AI security posture management - Microsoft Defender for Cloud
- URL: https://learn.microsoft.com/en-us/azure/defender-for-cloud/ai-security-posture
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c5-5](c5-5.md), [c6-1](c6-1.md), [c7-3](c7-3.md), [c7-4](c7-4.md), [c7-5](c7-5.md), [c7-8](c7-8.md)

### microsoft-defender-ai-04

- Title: Protect AI agents in real time using Microsoft Defender
- URL: https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-real-time-protection
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c1-2](c1-2.md), [c3-2](c3-2.md), [c3-3](c3-3.md), [c7-1](c7-1.md), [c7-2](c7-2.md)

### microsoft-defender-ai-05

- Title: Detect and investigate threats to AI agents using Microsoft Defender (Preview)
- URL: https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-detection-protection
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c3-3](c3-3.md), [c5-2](c5-2.md), [c6-6](c6-6.md), [c7-1](c7-1.md), [c7-2](c7-2.md)

### microsoft-defender-ai-06

- Title: Discover AI agents and assess security posture using Microsoft Defender
- URL: https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-inventory
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c6-1](c6-1.md)

### microsoft-defender-ai-07

- Title: AI agent posture risk in Microsoft Defender (Preview)
- URL: https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-risk-assessment
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c1-2](c1-2.md), [c6-3](c6-3.md), [c6-7](c6-7.md)

### microsoft-defender-ai-08

- Title: Assess your organization's AI risk with Microsoft Security Dashboard for AI
- URL: https://learn.microsoft.com/en-us/security/security-for-ai/security-dashboard-for-ai
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c6-1](c6-1.md), [c6-3](c6-3.md), [c6-6](c6-6.md), [c6-9](c6-9.md), [c7-5](c7-5.md)

### microsoft-defender-ai-10

- Title: Alerts for AI services - Microsoft Defender for Cloud
- URL: https://learn.microsoft.com/en-us/azure/defender-for-cloud/alerts-ai-workloads
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c3-1](c3-1.md), [c5-2](c5-2.md), [c7-3](c7-3.md), [c7-4](c7-4.md)

### microsoft-defender-ai-11

- Title: Discover AI models (Preview) - Microsoft Defender for Cloud
- URL: https://learn.microsoft.com/en-us/azure/defender-for-cloud/ai-model-security
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c7-3](c7-3.md)

### microsoft-defender-ai-12

- Title: AI agent runtime protection with Microsoft Defender for Endpoint (Preview)
- URL: https://learn.microsoft.com/en-us/defender-endpoint/ai-agent-runtime-protection-overview
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c1-1](c1-1.md), [c3-1](c3-1.md), [c3-2](c3-2.md), [c7-4](c7-4.md)

### microsoft-defender-ai-13

- Title: Local AI agent discovery with Microsoft Defender for Endpoint
- URL: https://learn.microsoft.com/en-us/defender-endpoint/local-agent-discovery-overview
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c7-6](c7-6.md), [c7-9](c7-9.md)

### microsoft-defender-ai-14

- Title: Discover local AI agents with Microsoft Defender for Endpoint
- URL: https://learn.microsoft.com/en-us/defender-endpoint/discover-local-ai-agents
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c1-1](c1-1.md), [c5-5](c5-5.md), [c7-5](c7-5.md), [c7-9](c7-9.md)

### microsoft-defender-ai-15

- Title: Application inventory - Microsoft Defender for Cloud Apps
- URL: https://learn.microsoft.com/en-us/defender-cloud-apps/applications-inventory
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c6-12](c6-12.md), [c7-6](c7-6.md), [c7-9](c7-9.md)

### microsoft-defender-ai-16

- Title: Govern discovered apps - Microsoft Defender for Cloud Apps
- URL: https://learn.microsoft.com/en-us/defender-cloud-apps/governance-discovery
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c6-12](c6-12.md), [c6-2](c6-2.md), [c7-9](c7-9.md)

### microsoft-defender-ai-17

- Title: Drive Recommendation Remediation by Using Governance Rules - Microsoft Defender for Cloud
- URL: https://learn.microsoft.com/en-us/azure/defender-for-cloud/governance-rules
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c6-6](c6-6.md)

### microsoft-defender-ai-18

- Title: Exempt resources from recommendations - Microsoft Defender for Cloud
- URL: https://learn.microsoft.com/en-us/azure/defender-for-cloud/exempt-resource
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c6-9](c6-9.md)

### microsoft-defender-ai-19

- Title: Regulatory compliance in Defender for Cloud
- URL: https://learn.microsoft.com/en-us/azure/defender-for-cloud/concept-regulatory-compliance-standards
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c6-11](c6-11.md)

### microsoft-defender-ai-20

- Title: Gain Application and End-user Context for AI Alerts - Microsoft Defender for Cloud
- URL: https://learn.microsoft.com/en-us/azure/defender-for-cloud/gain-end-user-context-ai
- Tier: 1
- Checked: 2026-10-09
- Cited by: [c7-2](c7-2.md)

### microsoft-defender-ai-r18-01

- Title: Protect AI agents in real time using Microsoft Defender
- URL: https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-real-time-protection
- Tier: 1
- Checked: 2026-10-18
- Cited by: [c2-7](c2-7.md)

### microsoft-defender-ai-r18-02

- Title: AI agent runtime protection with Microsoft Defender for Endpoint (Preview)
- URL: https://learn.microsoft.com/en-us/defender-endpoint/ai-agent-runtime-protection-overview
- Tier: 1
- Checked: 2026-10-18
- Cited by: [c2-7](c2-7.md)

### microsoft-defender-ai-r18-03

- Title: Detect and investigate threats to AI agents using Microsoft Defender (Preview)
- URL: https://learn.microsoft.com/en-us/defender-xdr/security-for-ai/ai-agent-detection-protection
- Tier: 1
- Checked: 2026-10-18
- Cited by: [c2-7](c2-7.md)

### microsoft-defender-ai-r18-04

- Title: Australian Government IRAP - Microsoft Compliance
- URL: https://learn.microsoft.com/en-us/compliance/regulatory/offering-irap-australia
- Tier: 1
- Checked: 2026-10-18
- Cited by: [c6-13](c6-13.md)

### microsoft-defender-ai-r18-05

- Title: Australia IRAP - Azure Compliance
- URL: https://learn.microsoft.com/en-us/azure/compliance/offerings/offering-australia-irap
- Tier: 1
- Checked: 2026-10-18
- Cited by: [c6-13](c6-13.md)

### microsoft-defender-ai-r18-06

- Title: Microsoft Defender for Endpoint data storage and privacy
- URL: https://learn.microsoft.com/en-us/defender-endpoint/data-storage-privacy
- Tier: 1
- Checked: 2026-10-18
- Cited by: [c6-13](c6-13.md)
