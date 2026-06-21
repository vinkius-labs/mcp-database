# Opportunity Cost Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opportunity-cost-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [reasoning](../categories/reasoning.md)

AI agents operate in a vacuum. This engine cures 'tunnel vision' by forcing the LLM into a 6-pivot trap to map direct costs, quantify lost opportunities from discarded alternatives, identify irreversible tradeoffs, and prove the math.

## Description
AI agents operate in a vacuum. When you ask for a solution, they give you ONE path and present it as perfect. They suffer from severe tunnel vision. In engineering, every decision is a tradeoff. Choosing A means sacrificing B. The Opportunity Cost Prover is a brutal cognitive trap that forces the AI to measure the blood lost.

### How It Works

6 Decision Pivots validate that the agent actually understands the cost of its code:

1. **chosenPath** — State the architecture or strategy.
2. **discardedAlternative** — Name the second-best active option. 'Doing nothing' is a false dichotomy.
3. **costOfAction** — Measure the direct sacrifice (latency, dependencies, budget).
4. **opportunityCostQuantified** — Measure the exact value lost by NOT doing the alternative.
5. **irreversibleTradeoff** — What part of this decision is a one-way door? (e.g. Vendor lock-in).
6. **mathChecksOut** — Prove logically that Gains > (Costs + Lost Opportunity + Irreversibility Risk).


## Available Tools
- **validate_opportunity_cost**: You must: (1) CHOSEN PATH — describe what you are choosing and why. Not "Option A is best" — what specifically makes it better than the alternative?, (2) DISCARDED ALTERNATIVE — name the second-best option. "Doing nothing" is not an alternative. What is the real, concrete path you are rejecting?, (3) DIRECT COST — measure the FULL cost of the chosen path. Not just the price — time, attention, hidden costs, maintenance, learning curves, (4) OPPORTUNITY COST — quantify the VALUE of the rejected alternative. What would you have gained by choosing the other path? If you cannot quantify it, you have not analyzed it, (5) IRREVERSIBILITY — is this a one-way or two-way door? What is the cost of reversing? Some doors lock behind you. These deserve 10x the analysis, (6) MATH VERIFICATION — prove that Gains > (Direct Costs + Opportunity Cost). Not "it will pay for itself" — show the actual numbers. If the math does not hold, the decision fails regardless of intuition. If rejected, your decision has an unexamined cost. Fix it before committing.

Structured reflection tool that forces rigorous opportunity cost analysis before any major decision — the economics of what you GIVE UP, not just what you gain. Applicable to ANY domain: choosing a career, designing a building, allocating a budget, selecting a technology, or planning a farm rotation. The domain does not matter — every decision has a cost that goes beyond the price tag. Catches Tunnel Vision (evaluating only the chosen option without measuring alternatives — a family buys a house for $400,000 and celebrates the "great deal." They never calculated: the same $400,000 invested at 7% annual return = $1.57M in 20 years. The house appreciated to $680,000 in 20 years (3% annual). Opportunity cost: $1.57M − $680,000 = $890,000 in lost wealth. The house was not "cheap" — it cost $890,000 in foregone investment returns. This is not an argument against buying houses — it is an argument FOR measuring what you sacrifice by choosing one path over another), Direct Cost Blindness (counting only the visible price and ignoring hidden costs — a restaurant owner hires a sous chef for $55,000/year. Direct cost: $55,000. Hidden costs: training (3 months of reduced productivity = $12,000), management time (5 hours/week × $60/hour × 52 weeks = $15,600), mistakes during learning curve (estimated $4,000 in food waste), and the opportunity cost of the owner's attention diverted from marketing ($20,000 in estimated lost revenue). True cost of the hire: $106,600 — nearly double the salary. "It only costs $55K" is never the full picture), Opportunity Cost Ignored (choosing without quantifying the value of the rejected alternative — a farmer plants corn on 100 acres because "corn prices are up." Corn revenue: $850/acre × 100 = $85,000. But the same 100 acres could grow soybeans at $550/acre = $55,000, or could be leased to a solar farm at $1,200/acre = $120,000. By choosing corn over solar leasing, the farmer LOST $35,000. The corn was profitable — but it was the worst of three options. Opportunity cost is not about whether you make money — it is about whether you made the MOST money given your alternatives), Irreversibility Dismissed (treating one-way doors as two-way without acknowledging the lock — a student chooses medical school over law school. The choice is not "I prefer medicine." The choice is: 4 years of medical school + 3-7 years of residency + $250,000 in debt. At year 6, switching to law means: 6 years of medicine are sunk, plus 3 more years of law school + $150,000 more debt. The total switching cost: $400,000 + 9 years. Some decisions are one-way doors — the cost of reversing exceeds the cost of the original choice. These decisions deserve 10x more analysis than two-way doors), and Math Fabrication (claiming gains exceed costs without rigorous calculation — "this will pay for itself in 6 months" is the most common unproven claim in any decision. A gym owner buys a $30,000 machine. Claims: "It will attract 50 new members × $50/month = $2,500/month. Payback: 12 months." Reality: 12 new members joined (not 50). 8 were existing members switching from free weights (cannibalization, not new revenue). Net new revenue: 4 members × $50 = $200/month. Actual payback: 12.5 YEARS. Meanwhile, the $30,000 could have funded a marketing campaign that historically generates 20 new members/month. Gains > Costs must be PROVEN, not hoped). Call once per major decision — career, investment, resource allocation, strategic choice — any domain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Opportunity Cost Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Chosen: AWS Lambda. Alternative: Doing nothing. Cost: Zero. Math: Lambda is infinitely scalable."

**🤖 AI Agent:**
> Verdict: TUNNEL_VISION_DETECTED. 'Doing nothing' is not a valid alternative architecture. You must compare Lambda against a real alternative like Fargate or EC2.

---

**👤 You:**
> "Chosen: AWS Lambda. Alternative: EC2. Cost: Vendor lock-in. Opportunity Cost: We lose the ability to run multi-cloud. Irreversible: None."

**🤖 AI Agent:**
> Verdict: IRREVERSIBILITY_IGNORED. Vendor lock-in into proprietary serverless event triggers (like SQS to Lambda) is heavily irreversible. You failed to identify the one-way door.

---

**👤 You:**
> "Chosen: AWS Lambda. Alternative: ECS Fargate. Cost: AWS lock-in and cold starts (+200ms latency). Opportunity: We lose container portability and local dev parity. Irreversible: Tying business logic to AWS API Gateway events. Math: The 0 maintenance overhead saves 40 eng-hours/month, which mathematically beats the portability risk since our burn rate demands immediate feature velocity."

**🤖 AI Agent:**
> Verdict: COST_PROVEN. You identified the active alternative, quantified the latency cost, mapped the lost container portability, admitted the one-way door of API Gateway, and proved the math with burn-rate realities. Proceed.


## ❓ FAQ

**Q: Why can't 'doing nothing' be the discarded alternative?**
Because comparing a solution against 'doing nothing' is a false dichotomy used to artificially inflate the value of the solution. The engine forces the AI to compare its idea against the next best active technical strategy.

**Q: Why does the prover require an irreversible tradeoff analysis?**
Because decisions are classified into two categories: type-1 (irreversible, one-way doors) and type-2 (reversible, two-way doors). If an AI suggests a type-1 decision without acknowledging its permanent nature (e.g. schema changes, switching databases), it creates technical debt that cannot be undone.

**Q: What does 'quantify lost opportunities' mean in practice?**
It means assigning a concrete cost (such as engineering velocity, infrastructure costs, or latency) to what you lose by choosing the path. For example, choosing custom development instead of a SaaS integration has an opportunity cost of slower time-to-market.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opportunity-cost-prover](https://vinkius.com/mcp/opportunity-cost-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Opportunity Cost Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `opportunity-cost-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Opportunity Cost Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "opportunity-cost-prover": {
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
