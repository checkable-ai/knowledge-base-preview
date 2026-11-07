# Checkable AI knowledge base: preview

This repository is a preview of the Checkable AI knowledge base. The knowledge base records what AI platforms and tools document about security controls: who approves an agent's actions, where its data goes, how its activity is logged, and dozens more. Our free [AI Stack Check](https://checkableai.com/stack-check/) runs on it.

What you see here is the lighter version. It holds a slice of our October 2026 research: 27 platforms and tools, from model makers and coding agents to cloud AI platforms, identity, security and governance tools, each checked against the same 44 controls. The full knowledge base is larger, newer and stays private.

You don't need to be technical to use it. Every record is a plain text page you can read on GitHub.

## What is in here

| Folder | What it holds |
| --- | --- |
| `okf/atlas/columns/` | One folder per platform. Each has a profile, a list of its sources and one page per control |
| `okf/atlas/controls/` | One page per control: what it means, and how every platform in this preview answers it |
| `okf/atlas/AGENTS.md` and `okf/atlas/rules/` | The rules an AI agent follows when it reads these pages, and how the pages are made |
| `okf/atlas/retrieval-index.json` | One line of facts per page (verdict, state, sources), so a program can search without reading every page |
| `web/atlas-sample.json` and `app/` | The data file and browser code behind our Ask the Atlas questionnaire, which routes a question to the right records and checks every citation |
| `examples/` | A simulated freshness pull request: what happens when a vendor page changes |
| `docs/` | A diagram of how the research loop runs |

The pages follow Open Knowledge Format v0.2 (credited in [NOTICE](NOTICE)), so people and agents read the same files.

## What the preview holds back

For Anthropic (the Claude platform and Claude Code) and OpenAI, this preview keeps the verdict for every control, its state and its dates. It holds back the vendor quotes, source links, gaps, conditions and configuration steps. Those are the findings buyers ask us about most, and the detail stays in the private knowledge base that the full stack review uses. Every other platform here shows its records in full.

## How to read one record

Open [`okf/atlas/columns/wiz/c6-1.md`](okf/atlas/columns/wiz/c6-1.md). It answers one question: does Wiz keep an inventory of the AI in your estate (control c6-1, Asset Registries and Inventory)?

The block at the top, between the two `---` lines, is the record's label. Three lines matter most:

- `verdict: "supported"` is the short answer. Other values are `partial`, `not-addressed` and `unresolved`.
- `verification: "verified"` means an evaluator agent found a passage on the vendor's own page that backs the verdict. `unverified` means the research has not had that check yet.
- `checked_on: "2026-10-09"` is the day the vendor's pages were read. Products change, so the date matters.

The page below the label reads top to bottom:

1. **Answer.** What Wiz documents: an AI inventory of models, agents, services, MCP servers, tools and identities, plus an AI bill of materials. It also says the inventory is discovered, not registered.
2. **Products.** Which Wiz products the answer covers.
3. **Gaps.** What the sources leave open. Here, tool schemas are not described as part of the inventory.
4. **Options.** A next step: export the inventory through the Wiz API and reconcile it against an approved register.
5. **Evidence.** The evaluator's verdict for each source, the exact passage it quoted, and whether that quote passed the check.
6. **Sources.** The pages behind the record and how much each one can be trusted (tier 1 is the vendor's own documentation).

A not-addressed record also says what kind of gap it is. `gap_kind` tells you whether the control is outside what the product is for or a real gap in it.

## Why you can trust it

- **Vendor sources only.** Every record rests on the vendor's public pages, with the exact part of the page it relies on. No vendor pays to be listed or can change a finding.
- **Receipts.** An evaluator agent fetches the cited page, stores a copy, finds the passage and quotes it. Then plain code confirms the quote really is on that stored copy. The result is the Evidence table, and you can open the source and check it yourself.
- **Review.** Records with no evaluator run yet were researched with cited sources and accepted by our reviewer for this research set. Each record says which of the two it is, in `eligibility_basis`.
- **Honest limits.** A verdict says what a vendor documents. It is not a test of your tenant, licence or settings, and missing documentation is not proof that a feature is missing.

## What this preview is not

- It is not current. The research dates from October 2026 and vendor products change. The [AI Stack Check](https://checkableai.com/stack-check/) uses our newest checked findings.
- It is not the whole knowledge base. The full one covers far more platforms and more controls, with a person reviewing the findings, and it stays private.
- It is not advice about any vendor's product.

## Where to go next

- Run the free [AI Stack Check](https://checkableai.com/stack-check/) on the tools you use. It runs in your browser.
- For a person to review your stack against the full knowledge base, [make an enquiry](https://checkableai.com/enquire/).

## Licence

MIT, see [LICENSE](LICENSE). Quoted vendor documentation stays under its publishers' terms, see [NOTICE](NOTICE). To report a security problem, see [SECURITY.md](SECURITY.md).
