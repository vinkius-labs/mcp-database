# Marketplace Liquidity Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/marketplace-liquidity-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Analyze marketplace health with real-time liquidity metrics.

## Description
This MCP server provides deep insights into marketplace efficiency. Use `get_liquidity_summary` to evaluate the balance between supply and demand, or `get_fill_rate_metrics` to see how effectively listings convert to sales. You can also use `get_geographic_liquidity` to find regional imbalances and `get_category_efficiency` to monitor throughput across different product segments.


## Available Tools (4)
- **get_fill_rate_metrics**: Analyzes how effectively supply is being converted into completed transactions
- **get_geographic_liquidity**: Breaks down liquidity performance by geographic region to identify local imbalances
- **get_category_efficiency**: Evaluates how liquidity is distributed across different product categories
- **get_liquidity_summary**: Provides a high-level overview of the core liquidity health of the marketplace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marketplace Liquidity Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current liquidity health of my marketplace?"

**🤖 AI Agent:**
> The current supply-demand ratio is 1.2, with a transaction velocity of 0.45 and a composite liquidity score of 78/100.

---

**👤 You:**
> "What is the fill rate for my current listings?"

**🤖 AI Agent:**
> The current fill rate is 65%, meaning 65% of all listings resulted in a successful transaction.

---

**👤 You:**
> "How efficient is the electronics category?"

**🤖 AI Agent:**
> The electronics category has an average order value of $250 based on recent transaction data.


## ❓ FAQ

**Q: What metrics does this server provide?**
It provides supply-demand ratios, transaction velocity, fill rates, and regional or category-specific liquidity scores.

**Q: How is the liquidity score calculated?**
The score is a weighted combination of the supply-demand balance and the transaction velocity.

**Q: Can I analyze specific regions?**
Yes, using `get_geographic_liquidity` you can identify local imbalances by passing regional supply and demand data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/marketplace-liquidity-engine](https://vinkius.com/en/ai-agent-connect/marketplace-liquidity-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Marketplace Liquidity Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `marketplace-liquidity-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Marketplace Liquidity Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marketplace-liquidity-engine": {
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
