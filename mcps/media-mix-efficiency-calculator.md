# Media Mix Efficiency Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/media-mix-efficiency-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate channel efficiency (CPL, CPA, ROAS) and get a data-driven budget reallocation plan to maximize conversions.

## Description
Are you unsure where your marketing spend is providing the best return? In today's complex digital landscape, simply running ads isn't enough; you must know precisely which channels deliver the highest value per dollar. Many businesses struggle with siloed data--they track spend and leads, but they lack a unified view of true profitability.

This tool solves that by providing end-to-end marketing performance analysis. It first uses the `calculate_channel_metrics` function to compute core efficiency ratios (Cost Per Lead, Cost Per Acquisition, ROAS) for every channel you feed it. Next, the `rank_channel_efficiency` tool takes these raw metrics and calculates a weighted composite score, identifying your top-performing channels based on whether your goal is lead volume or revenue maximization. Finally, the powerful `propose_budget_reallocation` function takes this ranking and mathematically recommends exactly how to shift your total budget across all channels to achieve maximum projected conversions while staying within your defined spending limit.

The advantage is clear: you move from guessing where to spend money to executing a proven, optimized plan for measurable growth.


## Available Tools (3)
- **rank_channel_efficiency**: Rank marketing channels by composite efficiency score
- **propose_budget_reallocation**: Propose budget reallocation to maximize conversions within total budget
- **calculate_channel_metrics**: Calculate efficiency metrics (CPL, CPA, ROAS) for a marketing channel


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Media Mix Efficiency Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I spent $10,000 total. Google Ads got me 500 leads for $3k and $20k revenue. Facebook got 800 leads for $4k and $16k revenue. Can you analyze this to tell me where I should spend next?"

**🤖 AI Agent:**
> First, we run `calculate_channel_metrics` on both channels. Then, using `rank_channel_efficiency` with 'Revenue Maximization' as the goal, we get a ranked list. Finally, we pass everything to `propose_budget_reallocation` with $10,000 total budget for the optimized plan.

---

**👤 You:**
> "Please calculate the raw metrics for a new channel: 20 leads, $500 spent, and generated $10,000 in revenue."

**🤖 AI Agent:**
> Calling `calculate_channel_metrics` with the specified parameters. This returns CPL, CPA, and ROAS for this single channel, giving you a baseline score to compare against existing channels.

---

**👤 You:**
> "I want the best possible plan to generate as many leads as possible with my $50,000 budget. My current metrics are: [list of complex JSON array]."

**🤖 AI Agent:**
> The system will use `rank_channel_efficiency` setting the primary goal to 'Lead Generation Volume'. It then feeds that ranking to `propose_budget_reallocation` using $50,000 as the total budget, providing a concrete spending plan.


## ❓ FAQ

**Q: How do I determine if a channel is truly profitable?**
Profitability requires calculating the Return On Ad Spend (ROAS). You must first run `calculate_channel_metrics` to get the ROAS for each channel. Then, use `rank_channel_efficiency` to get a composite score that weights this ROAS against your primary goal.

**Q: What is the final step after analyzing channel metrics?**
The last and most critical step is using `propose_budget_reallocation`. This tool takes your optimal efficiency rankings (from `rank_channel_efficiency`) and mathematically determines the precise amount of budget each channel should receive to maximize total conversions.

**Q: Can this tool handle different optimization goals (e.g., leads vs. revenue)?**
Yes. The `rank_channel_efficiency` tool accepts a `primaryGoal` parameter, allowing you to instruct the system whether the ranking should prioritize 'Lead Generation Volume' or 'Revenue Maximization', ensuring the subsequent budget proposal is tailored to your business objective.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/media-mix-efficiency-calculator](https://vinkius.com/mcp/media-mix-efficiency-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Media Mix Efficiency Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `media-mix-efficiency-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Media Mix Efficiency Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "media-mix-efficiency-calculator": {
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
