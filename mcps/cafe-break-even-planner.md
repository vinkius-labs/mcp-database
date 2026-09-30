# Cafe Break-Even Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cafe-break-even-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate daily revenue and unit targets needed to cover cafe operational costs.

## Description
This MCP server provides specialized financial tools for cafe owners to manage profitability. It calculates the exact daily revenue and unit volume required to reach the break-even point by analyzing fixed costs, variable ingredient costs, and the specific sales mix of products. Use `calculate_daily_break_even` to find your daily targets, `analyze_product_profitability` to identify high-margin items, `simulate_sales_mix_shift` to predict how changing your menu affects revenue needs, and `get_operating_leverage` to understand your business's sensitivity to sales fluctuations.


## Available Tools (4)
- **analyze_product_profitability**: Analyze the profitability of each item in the sales mix
- **calculate_daily_break_even**: Calculate the daily revenue and units needed to break even
- **get_operating_leverage**: Calculate operating leverage and margin of safety
- **simulate_sales_mix_shift**: Simulate how a change in sales mix affects the break-even point


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cafe Break-Even Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much revenue do I need to make daily if my monthly fixed costs are $5000, I'm open 25 days a month, and my sales mix is 60% coffee ($4 price, $1 cost) and 40% pastries ($5 price, $2 cost)?"

**🤖 AI Agent:**
> To cover your $5,000 monthly fixed costs with that sales mix, you need to generate $312.50 in revenue every day.

---

**👤 You:**
> "Which of these items is most profitable: Coffee ($4 price, $1 cost, 70% weight) or Muffin ($5 price, $2 cost, 30% weight)?"

**🤖 AI Agent:**
> The Coffee has a unit margin of $3.00, while the Muffin has a unit margin of $3.00. However, the Coffee contributes $2.10 to your total margin, whereas the Muffin contributes $0.90.

---

**👤 You:**
> "What is my margin of safety if my break-even is $200/day and I currently sell $250/day?"

**🤖 AI Agent:**
> Your margin of safety is 25%. This means your daily sales can drop by 25% before you reach the break-even point.


## ❓ FAQ

**Q: How do I calculate my daily break-even target?**
You can use the `calculate_daily_break_even` tool. Provide your monthly fixed costs, the number of operating days, and a JSON array representing your sales mix (including price, ingredient cost, and revenue weight).

**Q: Can I see which menu items are most profitable?**
Yes, the `analyze_product_profitability` tool provides a detailed breakdown of unit margins and how much each item contributes to your total weighted margin.

**Q: What happens if I change my product mix?**
Use the `simulate_sales_mix_shift` tool to compare your current mix against a new proposed mix. It will show you the percentage change in required revenue and unit volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cafe-break-even-planner](https://vinkius.com/en/ai-agent-connect/cafe-break-even-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cafe Break-Even Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cafe-break-even-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cafe Break-Even Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cafe-break-even-planner": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
