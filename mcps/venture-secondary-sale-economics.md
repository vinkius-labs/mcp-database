# Venture Secondary Sale Economics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-secondary-sale-economics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate secondary sale proceeds, realized returns, and liquidity availability for private equity holdings.

## Description
This MCP server provides specialized financial modeling tools for venture capital professionals to assess the economic impact of secondary market transactions. It allows users to calculate expected cash proceeds using `estimate_sale_proceeds`, evaluate investment performance via `calculate_investment_performance`, and determine market availability with `assess_liquidity_availability`. Additionally, users can model various market conditions using `generate_liquidity_scenario` to prepare for potential exits.


## Available Tools (4)
- **assess_liquidity_availability**: Assess the potential liquidity and ease of selling a position
- **calculate_investment_performance**: Calculate the realized return multiple and total profit/loss for an investment
- **estimate_sale_proceeds**: Calculate the expected cash proceeds from a secondary sale of private shares
- **generate_liquidity_scenario**: Simulate different market scenarios for a potential exit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Secondary Sale Economics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much cash will I receive if I sell 50,000 shares in a company valued at $500,000,000 with 10,000,000 total shares and a 20% secondary discount?"

**🤖 AI Agent:**
> Based on a $500,000,000 valuation and 10,000,000 total shares, the price per share is $50. Applying a 20% discount results in a price of $40 per share. For 50,000 shares, your total sale proceeds will be $2,000,000.

---

**👤 You:**
> "What is my ROI if I sell my position for $1,500,000 that originally cost me $500,000?"

**🤖 AI Agent:**
> Your realized return multiple is 3.0x, and your total profit is $1,000,000.

---

**👤 You:**
> "Assess the liquidity for 10,000 shares with a buyer interest level of 0.8, no transfer restrictions, and 3 years remaining in the fund."

**🤖 AI Agent:**
> The estimated liquidity value is 10,000 shares with an availability score of 80%.


## ❓ FAQ

**Q: How do I calculate my expected cash from a sale?**
You can use the `estimate_sale_proceeds` tool. Provide the number of shares held, the current company valuation, the expected secondary discount, and the total shares outstanding.

**Q: Can I model different market conditions?**
Yes, the `generate_liquidity_scenario` tool allows you to simulate base, pessimistic, and optimistic proceeds based on varying market demand and fund timelines.

**Q: How is my return on investment calculated?**
The `calculate_investment_performance` tool calculates your realized return multiple and total profit or loss by comparing your sale proceeds against your original cost basis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-secondary-sale-economics](https://vinkius.com/en/ai-agent-connect/venture-secondary-sale-economics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Secondary Sale Economics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-secondary-sale-economics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Secondary Sale Economics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-secondary-sale-economics": {
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
