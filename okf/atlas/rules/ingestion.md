---
type: "Guide"
title: "Rules for the pages in this tree"
description: "How the pages in this tree are made, which pages agents may retrieve, and what is left out."
classification: "C1"
owner: "human:owner"
status: "stable"
review: "pending"
verification: "not applicable"
tags:
  - "rules"
sources: []
generated:
  by: "process:offerings-atlas-ingest"
  at: "2026-11-18T00:00:00+10:00"
---

These rules govern every page in this tree. The tree is generated, so a page is never edited by hand. A rerun on the
same records and the same date writes the same pages.

## Where the facts come from

Each page is drawn from the vendor's own public documentation. The sources a page relies on are listed on the page,
each with its trust tier. Tier 1 is the vendor's own documentation and tier 2 is a vendor blog or a standards body.

## Type mapping

| Record | Page | Type |
| --- | --- | --- |
| One answer, a platform against a control | `columns/<platform>/<control>.md` | Platform capability |
| A platform | `columns/<platform>/profile.md` | Platform profile |
| The sources a platform cites | `columns/<platform>/sources.md` | Registry |
| A control | `controls/<control>.md` | Control |
| This file and the agent guide | `rules/ingestion.md`, `AGENTS.md` | Guide |

## Front matter

Every page carries `type`, `title`, `description`, `classification`, `owner`, `status`, `review`, `verification`,
`tags`, `sources` and `generated`. `owner` names who is accountable for the page, and it is the same on every answer
page: the owner of Checkable AI. Who checked a record is in its `review`, `verification` and eligibility basis. An answer page adds an `atlas` block: platform, control, group, verdict, whether
agents may retrieve the page and why, the check date and the file it was drawn from.

An answer page also carries its limits as data, beside the verdict. `conditions_apply: true` marks an answer that is
covered with conditions: a plan, a preview, a region, an add-on or a hosting route decides whether the control is
there for a given customer. `condition_kinds` and `hard_kinds` name the kinds of condition, `plans`,
`plans_excluded`, `hosting_routes` and `hosting` give the plans and hosting routes the conditions name, and
`condition_sentences` lists each condition with its own kinds and values. `missing_kinds` and `missing_sentences` do
the same for what the documentation leaves out. A value of `not-stated` means the page makes the control depend on a
plan or a route without naming one.

The verdict is one of `covered`, `partial`, `not-covered`, `out-of-scope` or `escalated`. A `not-covered` answer also
carries a `gap_kind`: `out-of-scope` when the control is outside what the product is for, and `in-scope-gap` when the
control belongs to the product and nothing is documented. `review: approved` means a person at Checkable AI accepted
the verdict shown on the page, and its `verification` is `verified`. `review: pending` means the agents checked the
verdict as the page states (an evaluator that found the quoted passage on the vendor's page, or two model families that
agreed) and no person has accepted it yet, so its `verification` is `agent-checked`. A `not-covered` or `out-of-scope`
verdict often has no passage to quote: there the documentation was read and two model families agreed it does not
document the control. An `escalated` verdict is one the agents did not agree on (`verification: "contested"`), so a
person settles it.

`retrieval-index.json` lists every page with its path, platform, group, control, verdict, gap kind, verification,
review state, retrieval status, sources, chunk names and SHA-256, so a program can filter and fetch without parsing YAML.

## Tags

An answer page carries four tags, in order: the column group, the control category, the verdict and the verification
state. Profiles and registries carry the group, and controls carry the category.

## Chunks

An answer page opens with one orientation paragraph, then six sections, each preceded by a `chunk` comment so a
retriever can split and cite them: answer, products, gaps, options, evidence and sources. No chunk is longer than 600
words.

## Retrieval

An answer page is open to agents on the edition date when its verdict was confirmed by two model families, a quote
check passed on a `covered` or `partial` verdict, the page is classed C1, and its recheck date is still ahead. The
index marks these pages `agent_eligible` and gives the date to which each one holds. Every other page stays open to
people to read, shows its state, and gives the reason it is not marked for agents.

## What is left out

An answer whose text holds an email address, a phone number, a network address or a money figure is left out whole,
so the tree holds no personal or client data. Three kinds are not personal or client data and stay: a vendor's
published list price, a role mailbox on the vendor's own domain, and a private or documentation network address used
as an example. Quoted vendor text is never reworded, because rewording a quote changes
the evidence. Every link in the tree is the registered address of one of the listed sources.
