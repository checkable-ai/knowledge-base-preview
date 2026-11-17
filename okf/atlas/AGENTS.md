---
type: "Guide"
title: "Agent guide to the offerings atlas tree"
description: "How agents read this tree, and why they never write to it."
classification: "C1"
owner: "human:owner"
status: "draft"
review: "pending"
verification: "not applicable"
tags:
  - "rules"
sources: []
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

This tree is generated. Never edit it. Change the atlas store and rerun the ingest, under the [ingestion rules](rules/ingestion.md).

## Reading

1. Load `retrieval-index.json` and keep only entries marked `agent_eligible`.
   Each entry names its basis: `agent-verified` (an evaluator checked it) or `agent-confirmed` (two model families confirmed it, with a quote check on covered and partial). Say which when you quote it.
2. Retrieve, index or summarise only the pages left in that list. Every other page is for people to read.
3. Quote a cell with its verdict, its state, its gaps and its sources. A positive answer alone drops qualifiers.
4. Read the limits with the verdict. A cell page whose `atlas` block says `conditions_apply: true` is covered with conditions: a plan, preview, region, add-on or hosting route decides whether the control is there for a given customer. `condition_sentences` lists each condition with its kinds, the plans it names and the hosting routes it names, and `missing_sentences` does the same for what the documentation leaves out. Quote the sentences that apply with the verdict.

## What the states mean

| State | Meaning |
| --- | --- |
| verified | The agents checked the verdict and a person at Checkable AI accepted it (`review: approved`). For `covered` and `partial` the check is a quoted passage on the vendor's page or two model families agreeing. For `not-covered` and `out-of-scope` there is often no passage to quote: the vendor's documentation was read and two model families agreed it does not document the control, as at `checked_on` |
| agent-checked | Checked by the agents in the same way, and no person has accepted it yet (`review: pending`) |
| provisional | Supported by a tier 3 source only, expires after 30 days |
| contested | Evaluators or sources disagree |
| stale | Was verified, recheck date passed |

## What this tree never holds

Business decisions, prices or offerings. A cell page marked `review: approved` carries a person's acceptance of its current verdict, never a business decision. One marked `review: pending` has been checked by the agents, as its state says, and waits for that person.
