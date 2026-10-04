# Net Worth Dashboard MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/net-worth-dashboard)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate net worth, asset allocation, and growth metrics.

## Description
This MCP server provides a suite of financial tools to analyze your wealth. Use `calculate_current_standing` to get a high-level overview of assets and liabilities, `get_asset_allocation` to see how your wealth is distributed, `calculate_growth_metrics` to track changes over time, and `summarize_category_exposure` to identify concentration risks.


## Available Tools (4)
- **summarize_category_exposure**: Identifies potential financial risks by highlighting concentration in specific categories
- **calculate_current_standing**: Provides a high-level overview of the current financial position
- **get_asset_allocation**: Analyzes how wealth is distributed across different asset categories
- **calculate_growth_metrics**: Determines how much the user's net worth has changed compared to a prior point in time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Net Worth Dashboard** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current net worth if I have $50,000 in assets and $20,000 in liabilities?"

**🤖 AI Agent:**
> Your current net worth is $30,000.

---

**👤 You:**
> "How is my wealth distributed if I have $10,000 in Cash and $40,000 in Stocks?"

**🤖 AI Agent:**
> Your asset allocation is 20% Cash and 80% Stocks.

---

**👤 You:**
> "My previous net worth was $100,000. Now it is $120,000. What is my growth?"

**🤖 AI Agent:**
> Your net worth increased by $20,000, which is a 20% growth.


## ❓ FAQ

**Q: How do I calculate my current financial position?**
You can use the `calculate_current_standing` tool by providing your current assets and liabilities.

**Q: Can I track my wealth growth over time?**
Yes, use `calculate_growth_metrics` with your current data and a previous net worth snapshot to see your progress.

**Q: How can I identify if I am too heavily invested in one category?**
The `summarize_category_exposure` tool helps you find categories that exceed a specific percentage threshold of your total assets.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/net-worth-dashboard](https://vinkius.com/en/ai-agent-connect/net-worth-dashboard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Net Worth Dashboard** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `net-worth-dashboard` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Net Worth Dashboard** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "net-worth-dashboard": {
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
