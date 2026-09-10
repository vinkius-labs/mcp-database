# Well Economics & Abandonment Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/well-economics-abandonment-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate economic limits, abandonment timing, and remaining reserves for producing wells.

## Description
This MCP server provides essential tools for petroleum engineers and asset managers to optimize well life cycles. By connecting AI agents to production data, you can use `get_economic_limit` to find the profitability threshold, `calculate_abandonment_timing` to predict the end of production, and `estimate_remaining_reserves` to quantify recoverable volumes. Additionally, `analyze_intervention_impact` helps evaluate if workovers or artificial lift installations are financially sound based on current decline curves and operating costs.


## Available Tools (4)
- **calculate_abandonment_timing**: Predicts when the well will reach its economic limit and should be abandoned
- **estimate_remaining_reserves**: Calculates the total volume of oil or gas that can be recovered until abandonment
- **get_economic_limit**: Determines the production rate threshold where the well ceases to be profitable
- **analyze_intervention_impact**: Evaluates if a workover or the installation of artificial lift is economically viable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Well Economics & Abandonment Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the economic limit for a well producing 500 bbl/d with operating costs of $2000/day and oil at $75/bbl?"

**🤖 AI Agent:**
> The economic limit rate for this well is 26.67 bbl/d.

---

**👤 You:**
> "How much oil can we recover from a well currently at 200 bbl/d with a limit rate of 50 bbl/d and a decline exponent of 0.5?"

**🤖 AI Agent:**
> The estimated recoverable volume is 600 bbl.

---

**👤 You:**
> "If I spend $50,000 on a workover to increase my rate by 20%, is it worth it for a well with 10,000 barrels of reserves?"

**🤖 AI Agent:**
> The intervention is not viable as the net value impact is negative.


## ❓ FAQ

**Q: How do I determine when a well should be shut in?**
You can use the `get_economic_limit` tool to find the rate where revenue equals operating costs, and then use `calculate_abandonment_timing` to see how long it will take to reach that threshold.

**Q: Can this tool help evaluate workover decisions?**
Yes, the `analyze_intervention_impact` tool evaluates if the cost of a workover or artificial lift is offset by the resulting increase in production and revenue.

**Q: How are remaining reserves calculated?**
The `estimate_remaining_reserves` tool calculates the integral of the production rate from the current rate down to the economic limit rate based on your decline exponent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/well-economics-abandonment-optimizer](https://vinkius.com/ai-agent-connect/well-economics-abandonment-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Well Economics & Abandonment Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `well-economics-abandonment-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Well Economics & Abandonment Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "well-economics-abandonment-optimizer": {
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
