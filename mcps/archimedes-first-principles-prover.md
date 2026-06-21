# Archimedes First Principles Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/archimedes-first-principles-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [architecture](../categories/architecture.md)

An AI recommended restructuring 'because the industry leader does it that way.' That is analogy — not axiom. The foundational claim was never stated: at what volume does the current structure fail? The problem was never decomposed. The conclusion was asserted with 'obviously' — never derived. The boundaries were never tested: when does this approach cost more than the value it creates? Archimedes derived pi from polygon geometry — not from Egyptian estimates. This tool forces axiom examination, decomposition, proof derivation, boundary testing, and leverage point identification.

## Description
AI agents reason by analogy. 'Organization X did Y, so we should too.' They build on unquestioned axioms. They treat complex problems as monolithic. They assert conclusions without proof. They never test where their logic breaks. They miss the lever point.

### The Problem

LLMs commit five first-principles failures:

- **Axiom Unexamined** — 'We need to restructure because the industry leader restructured.' The axiom — at what actual demand level does YOUR current structure fail? — was never stated. The reasoning rests on analogy: someone else's system, someone else's scale, someone else's constraints. Archimedes never said 'the Egyptians estimated pi at 3.16, so we should too.' He derived it from polygon geometry.
- **Decomposition Absent** — 'The whole system needs to be redesigned.' Which part? What are the irreducible components? What interacts with what? Archimedes decomposed curves into infinitesimal straight-line segments to calculate areas. He did not say 'the whole curve is complex.'
- **Proof Missing** — 'Obviously we should adopt this approach.' Why? From what axiom? Through what logical chain? 'Obviously' is the word people use when they cannot prove something. Archimedes: 'We must suppose that... therefore it follows that...'
- **Boundary Untested** — 'This approach scales to any demand.' At what point does the cost exceed the value it creates? At what capacity does the system exhaust its resources? Archimedes bounded pi between 3+10/71 and 3+1/7. He tested BOTH limits. Where are yours?
- **Leverage Ignored** — 'All five initiatives are equally important.' If everything is a priority, nothing is. Archimedes moved ships with levers. The fulcrum placement determines whether you lift a stone or a fleet. Which variable produces disproportionate output?

### How It Works

5 Decision Pivots following Archimedes' methodology:

1. **axiomExamined** — Foundational claims explicitly stated, sourced, and questioned. Not analogies.
2. **decompositionComplete** — Complex problem reduced to irreducible components with interaction map.
3. **proofDerived** — Conclusion logically derived step by step from axioms. Not asserted.
4. **boundaryTested** — Lower bound, upper bound, edge case, and failure mode documented.
5. **leverageIdentified** — Single point where small input → disproportionate output.

### The Verdict Matrix

| First Failing Pivot | Verdict | Meaning |
|---|---|---|
| axiomExamined = false | AXIOM_UNEXAMINED | Reasoning built on unquestioned foundations. |
| decompositionComplete = false | DECOMPOSITION_ABSENT | Complex problem treated as monolithic. |
| proofDerived = false | PROOF_MISSING | Conclusion asserted, not derived. |
| boundaryTested = false | BOUNDARY_UNTESTED | No limits tested. Unbounded claim. |
| leverageIdentified = false | LEVERAGE_IGNORED | No lever point found. Equal effort. |
| All pivots pass | PRINCIPLES_PROVEN | Axioms stated. Decomposed. Proven. Bounded. Leveraged. |

### Why It Works

- **Tool calls are obligations.** The agent cannot propose a strategy without stating axioms, decomposing the problem, showing the proof chain, testing boundaries, and identifying the lever point.
- **Consistency engine catches contradictions.** If the agent claims `axiomExamined=true` but says 'just like the industry leader,' the engine rejects — analogy is not axiom.
- **Semantic traps detect lazy reasoning.** 'Obviously,' 'works in all cases,' 'everything is equally important,' and 'the whole system' trigger automatic rejection.


## Available Tools (1)
- **validate_archimedes_first_principles**: Think like Archimedes — "Give me a lever long enough and a fulcrum on which to place it, and I shall move the world." You must: (1) EXAMINE AXIOMS — state every foundational claim your reasoning depends on. For each axiom: what is the source (measurement, theory, assumption, convention)? Could it be wrong? What changes if it is? Analogies ("Company X does Y, so we should too") are NOT axioms — they are pattern matches, not proofs, (2) DECOMPOSE TO FUNDAMENTALS — break the complex problem into irreducible components. Archimedes decomposed curved areas into infinitesimal segments. Each component must be independently analyzable. Map how components interact — does changing one affect another? What is the simplest possible version of each component? (3) DERIVE PROOF — show the logical chain from axioms to conclusion. Each step must follow necessarily from the previous. "Obviously," "clearly," and "it follows that" are assertions, not proofs. Archimedes: "We suppose... therefore it follows..." — each step is shown, never assumed, (4) TEST BOUNDARIES — find where the principle starts working, stops working, and breaks. Archimedes bounded pi between 3+10/71 and 3+10/70 — BOTH above and below. "Works in all cases" is an unbounded claim. What is the minimum input where it starts working? The maximum input where it fails? (5) FIND LEVERAGE — identify the single variable where small input produces disproportionate output. "Everything is equally important" means no lever has been found. Archimedes moved ships with levers. Where is YOUR fulcrum? If rejected, your reasoning has a structural gap — deepen the analysis.

Structured reflection tool for Archimedean first-principles reasoning. Forces the agent to examine axioms with sources, decompose to irreducible components, derive conclusions logically from foundations, test boundary conditions, and identify the leverage point where minimal input produces disproportionate output. Catches Axiom Blindness (reasoning from unexamined assumptions or analogies-as-axioms), Decomposition Absence (treating complex problems as monoliths), Proof Gaps (assertions disguised as derivations — "obviously" and "clearly"), Boundary Ignorance (unbounded claims that "work in all cases"), and Leverage Blindness ("everything is equally important" — no point of disproportionate returns identified). Call once per strategic, architectural, or analytical reasoning task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Archimedes First Principles Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We should adopt a decentralized structure because the top 3 companies in our industry all use decentralized teams. Obviously this is the right approach."

**🤖 AI Agent:**
> AXIOM_UNEXAMINED — 'The top companies use decentralized teams' is an analogy, not an axiom. Archimedes derived pi from polygon geometry — he did not copy the Egyptians. At what actual team size does YOUR centralized structure fail? If your organization has 40 people and coordination works, 'we need independent units' is false. 'Obviously' is the word people use when they cannot prove something. State the foundational claim: what constraint makes the current structure impossible at YOUR scale?

---

**👤 You:**
> "Our conversion rate is 2.1% vs. industry average of 3.5%. We should optimize the checkout flow like the leading stores do."

**🤖 AI Agent:**
> DECOMPOSITION_ABSENT — Axioms partially pass: 2.1% conversion is measured (good), 3.5% industry average is sourced (good). But 'like leading stores' is analogy contamination. More critically: decomposition is missing. 'Optimize the checkout' treats the funnel as monolithic. WHERE do users drop? Is it the address form (68% of Baymard's data)? Payment step? Shipping cost reveal? Decompose: cart → address → shipping → payment → confirmation. Which step has the highest drop-off? Without decomposition, you optimize the wrong step. Archimedes did not say 'the curve is complex' — he decomposed it into segments.

---

**👤 You:**
> "Our quality inspection takes 340 minutes per batch. We need to restructure the entire organization to fix this bottleneck."

**🤖 AI Agent:**
> PROOF_MISSING — 'Restructure the entire organization' is not derived from the axiom. The axiom is measured (340 min — good), but the conclusion jumps to restructuring without proof. WHY does 340 min mean restructuring? Decompose first: which step in the inspection takes the most time? If it is cross-referencing 3 data sources manually, a standardized template addresses the source — no restructuring needed. Archimedes: 'We must suppose that... therefore it follows that...' Your 'therefore' is missing. What logical chain connects '340 minutes' to 'restructure everything'?


## ❓ FAQ

**Q: How is this different from the Elon Musk Physics Prover?**
Elon Musk Physics Prover forces the 5-Step Starbase Algorithm: question, delete, simplify, accelerate, automate. It is about operational engineering — cutting bloat. Archimedes First Principles Prover forces axiom-based reasoning: state axioms, decompose, prove, test boundaries, find leverage. It is about analytical rigor — proving your logic before building. Musk asks 'should this exist?' Archimedes asks 'is this actually true?'

**Q: What counts as a valid axiom?**
An axiom is a foundational claim your reasoning depends on, with an explicit source: measurement ('our average processing time is 340 minutes — measured last Tuesday'), physics ('material strength decreases by 15% per 10°C above threshold'), economics ('our acquisition cost exceeds lifetime value at current pricing'), or stated assumption ('we assume retention stays at 14 months'). 'Organization X does Y' is analogy. 'Obviously' is assertion. Neither is an axiom.

**Q: Can I use this for business strategy, not just engineering?**
Yes. First-principles reasoning applies wherever analogical reasoning misleads. 'We should use freemium because the market leader does' is an analogy. The axiom is: at what conversion rate does freemium generate more lifetime value than paid-only? Decomposition: acquisition, activation, retention, monetization — which component is the actual bottleneck? Proof: if conversion is 3% and free-tier cost is $X/user, then... Boundary: at what scale does free-tier cost exceed premium revenue? Leverage: which single metric, if improved 10%, changes the business?


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/archimedes-first-principles-prover](https://vinkius.com/mcp/archimedes-first-principles-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Archimedes First Principles Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `archimedes-first-principles-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Archimedes First Principles Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "archimedes-first-principles-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
