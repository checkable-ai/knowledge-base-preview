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
  at: "2026-11-08T00:00:00+10:00"
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
`tags`, `sources` and `generated`. An answer page adds an `atlas` block: platform, control, group, verdict, whether
agents may retrieve the page and why, the check date and the file it was drawn from.

The verdict is one of `covered`, `partial`, `not-covered`, `out-of-scope` or `escalated`. A `not-covered` answer also
carries a `gap_kind`: `out-of-scope` when the control is outside what the product is for, and `in-scope-gap` when the
control belongs to the product and nothing is documented. `review: approved` means the owner approved the verdict
shown on the page.

`retrieval-index.json` lists every page with its path, platform, group, control, verdict, gap kind, verification,
retrieval status, sources, chunk names and SHA-256, so a program can filter and fetch without parsing YAML.

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

An answer whose text holds a money figure, an email address, a phone number or a network address is left out whole,
so the tree holds no personal or client data. Quoted vendor text is never reworded, because rewording a quote changes
the evidence. Every link in the tree is the registered address of one of the listed sources.
