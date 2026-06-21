# Product Discovery Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/product-discovery-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Block engineering waste. This gatekeeper demands hard data, behavioral segments, and proven willingness-to-pay before a single line of code is written.

## Description
Building software based on assumptions or shallow market feedback is the number one cause of startup failure. Product Discovery Prover acts as a structured validation gate, requiring product managers and AI agents to prove problem existence, isolate behavioral customer segments, and verify purchase intent before committing engineering hours to an MVP.

### The Problem It Solves

Many product initiatives fail due to five common discovery mistakes:

- **Solutions seeking problems** — Coding features based on personal intuition without empirical data proving a real problem exists.
- **Vague segments** — Targets defined by demographics instead of specific behavioral indicators.
- **Competitor blindness** — Claiming "no competition exists" instead of analyzing existing workflows, spreadsheets, and manual workarounds.
- **False purchase signals** — Confusing polite compliments with concrete willingness-to-pay signals.
- **MVP bloat** — Building a miniature version of the final software platform instead of a rapid experiment designed to test a core hypothesis.

### Key Benefits

- **Enforces evidence-based validation** — Requires hard data (search volume, support logs, waitlist conversions) before approving product requirements.
- **Behavioral segmentation** — Forces teams to target specific user behaviors rather than broad, unactionable demographics.
- **Verifies real purchase intent** — Distinguishes between vanity feedback ("I love this idea") and actual commitment (pre-orders, budget allocation).
- **Scopes testable experiments** — Elevates MVPs from unstructured code builds into rapid, testable experiments with defined metrics.
- **Prevents wasted engineering** — Acts as a hard gate against building software that nobody wants, saving months of development cycles.


## Available Tools
- **validate_product_discovery**: You must: (1) PROBLEM EVIDENCE — cite specific evidence the problem exists AT SCALE. User interviews (30+ where THEY raise the pain), search volume, forum posts, support tickets, existing spend on workarounds. "I think people need this" is not evidence, (2) SEGMENT — define the customer by BEHAVIOR, not demographics. Current tool, rejected alternatives, workflow friction, scale of operations, (3) COMPETITORS — test every competitor's product for real tasks for at least 1 week. Document strengths, gaps, switching costs, and lock-in. "No competition" is a red flag, (4) PURCHASE INTENT — show evidence of MONEY commitment, not interest. Pre-orders, LOIs, pilot agreements, current workaround spending. Compliments ≠ data, (5) MVP SCOPE — state the core hypothesis, the minimum experiment to test it, success metric with threshold, and timeline (1-4 weeks). If it takes more than 4 weeks, it is not minimum. If rejected, your product thinking has a blind spot. Fix it before building.

Structured reflection tool for product discovery validation — forces evidence-based problem validation, behavioral segmentation, hands-on competitor testing, purchase intent verification, and hypothesis-driven MVP scoping before any "build it" recommendation. Based on Lean Startup (Ries 2011), Jobs-to-be-Done (Christensen 2016), and The Mom Test (Fitzpatrick 2013). Catches Solution-Seeking-Problem (building a technology then searching for someone who needs it — "We built an AI that generates color palettes from text descriptions." Cool technology. Now: who has this problem? Designers? They already have Coolors, Adobe Color, and trained color intuition. Non-designers? They use templates with pre-made palettes. Developers? They copy colors from designs they admire. 47 customer discovery interviews: 0 interviewees described color palette generation as a pain point they would pay to solve. The technology is impressive. The problem does not exist at scale. Start with the pain — not the technology. Evidence of pain: "I spend 3 hours every project choosing colors and my clients always reject them" — THAT would be worth exploring), Segment Vague (describing the customer by demographics instead of behavior — "Our target market is small businesses." There are 33 million small businesses in the US alone. A bakery in rural Iowa and a fintech startup in Manhattan are both "small businesses." They have nothing in common. Behavioral segmentation: "Solo accountants who use spreadsheets for time tracking, have tried and abandoned FreshBooks within 30 days, and bill fewer than 20 clients per month at hourly rates." Now you know: their current tool (spreadsheets), their rejected alternative (FreshBooks), their scale (< 20 clients), their pricing model (hourly), and their pain (manual tracking). This segment can be found, reached, and converted — "small businesses" cannot), Competitor Blind (listing competitors without testing their product — "Competitor A has a clunky UI." Have you used it? For how long? "Competitor B lacks integrations." Which integrations? Did you check their API docs? Sign up for every competitor. Use them for real tasks for at least 1 week. Document: what they do well (because customers stay for a reason), what they do poorly (the gap your product must fill), switching cost (what a customer loses by leaving them), and lock-in mechanisms (data export, contract terms, integrations that break). If switching cost exceeds your value advantage, you cannot win the customer), Interest ≠ Intent (confusing compliments with purchase commitments — The Mom Test (Fitzpatrick 2013): "That's a great idea!" = politeness, not validation. "Would you use this?" = hypothetical, not commitment. "When can I buy it?" = intent signal. Proof of purchase intent (strongest → weakest): (1) Pre-orders with payment: they paid before the product exists. (2) Letters of Intent (LOI): signed commitment to purchase at launch. (3) Pilot agreements: they allocated time and resources to test. (4) Current spending on workarounds: they already pay for an inferior solution. (5) "I would definitely use this": worthless without money attached. "10,000 people on the waitlist" means nothing. "47 people pre-ordered at $99 with a credit card" means everything), and MVP Bloat (scoping a "minimum" product that takes 6 months to build — "Our MVP needs user authentication, payment processing, real-time collaboration, mobile apps for iOS and Android, and an admin dashboard." That is not an MVP — that is a product. An MVP is the MINIMUM experiment to test the CORE hypothesis. Hypothesis: "Solo accountants will pay $29/month for automated time tracking." MVP: a Google Form that asks 50 accountants to log their time for 1 week using your proposed format, then measures: did they complete it? Was it faster? Would they pay? Timeline: 1 week. Cost: $0. If 70%+ complete and 40%+ say "yes, I would pay" — THEN build the product. If not — pivot the hypothesis, not the code. An MVP is an experiment, not a product). Call once per product idea, feature hypothesis, or market entry decision


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Product Discovery Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Let's build an AI assistant for lawyers. It will help them read contracts faster. The market is huge and lawyers will love it."

**🤖 AI Agent:**
> Verdict: SOLUTION_SEEKING_PROBLEM. Stop. You have zero data. 'The market is huge' is not evidence — it is a guess. Before writing code: how do lawyers review contracts today? How many hours per week? What does a missed clause cost them? Bring numbers or do not proceed.

---

**👤 You:**
> "Idea: AI contract tool. Problem: solo lawyers spend 10+ hours/week reviewing standard vendor agreements. Keyword 'contract review tool' has 1.2K searches/month. Segment: solo corporate lawyers in boutique firms who use Word. Alternatives: Manual reading, paralegals, enterprise tools. Will pay: 8 lawyers pre-ordered at $99/month on our landing page. MVP: PDF upload + OpenAI prompt producing a 3-bullet summary. Tested in 2 weeks."

**🤖 AI Agent:**
> Verdict: DISCOVERY_PROVEN. Right. Problem quantified at 10+ hours/week. Search demand confirmed at 1.2K/month. Segment is behavioral — not 'lawyers' but 'solo corporate lawyers in boutique firms using Word.' Competitors mapped. 8 pre-orders at $99/month — that is real money. MVP scoped as a 2-week experiment, not a platform. Ship it.

---

**👤 You:**
> "Idea: AI contract summarizer. Problem: corporate lawyers spend 10+ hours/week. Segment: lawyers who use Microsoft Word. Competitors: Manual reading. Will pay: 20 people signed up to our waitlist saying 'it sounds like a great tool'. MVP: landing page, upload portal, settings dashboard, API integration, and analytics."

**🤖 AI Agent:**
> Verdict: NO_PURCHASE_INTENT. Three failures. First — 'lawyers who use Word' is a tool preference, not a behavioral segment. Second — 'it sounds great' is a compliment, not a commitment. Money is data. Where are the credit cards? Third — your MVP has 5 features. That is not an MVP, that is a product. Strip it to one testable hypothesis.


## ❓ FAQ

**Q: Why does the tool reject demographic segments?**
Because demographics are useless for product design. 'Millennials' is a marketing category, not a workflow. We demand behavioral segments because they isolate users actively experiencing the exact pain point you intend to solve.

**Q: What qualifies as valid purchase intent?**
Money or legally binding ink. Polite compliments and 'I would use this' are false signals that kill startups. We require active commitment: credit cards on file, signed B2B Letters of Intent (LOIs), or cash deposits.

**Q: How should an MVP be scoped?**
As a single-variable experiment. Drop the settings panels, user profiles, and polished UI. The MVP must isolate and test the core value hypothesis. Use manual back-end workarounds to deliver the outcome without building the platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/product-discovery-prover](https://vinkius.com/mcp/product-discovery-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Product Discovery Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `product-discovery-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Product Discovery Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "product-discovery-prover": {
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
