# Client Profitability Comparator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/client-profitability-comparator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Rank and analyze client profitability using revenue, costs, and operational metrics.

## Description
This MCP server provides tools to evaluate client accounts by calculating net profitability across multiple dimensions. Use `get_client_profitability_ranking` to identify your most and least profitable clients, or `get_client_efficiency_metrics` to analyze the time and effort required for specific accounts. You can also assess cash flow impact with `get_client_financial_health` and compare performance across different service levels using `compare_client_tiers`.


## Available Tools (4)
- **get_client_efficiency_metrics**: Analyzes how "expensive" a client is to serve in terms of time and effort
- **get_client_financial_health**: Evaluates the cash flow impact of a client by looking at payments and acquisition costs
- **get_client_profitability_ranking**: Provides a ranked list of clients based on their net profitability
- **compare_client_tiers**: g., Platinum Tier, Gold Tier).

Allows a user to compare the aggregate performance of different client tiers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Client Profitability Comparator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a list of my most profitable clients in descending order."

**🤖 AI Agent:**
> Here are your most profitable clients: Acme Corp ($50,000), Globex Inc ($42,000), and Stark Industries ($38,500).

---

**👤 You:**
> "How efficient is client 'C123' in terms of revenue per hour?"

**🤖 AI Agent:**
> Client C123 has a revenue per hour of $250, with a total of 40 hours worked and 3 revisions.

---

**👤 You:**
> "Compare the average profit of the Platinum Tier against the Gold Tier."

**🤖 AI Agent:**
> The Platinum Tier has an average profit of $15,000 per client, while the Gold Tier averages $8,500 per client.


## ❓ FAQ

**Q: How is client profitability calculated?**
Profitability is calculated by taking total revenue and subtracting labor costs, direct expenses, acquisition costs, and penalties for revisions or payment delays.

**Q: Can I filter clients by a minimum profit threshold?**
Yes, you can use the `get_client_profitability_ranking` tool with the `minProfitability` parameter to filter results.

**Q: What information is included in efficiency metrics?**
The `get_client_efficiency_metrics` tool provides total hours worked, the number of revisions, and the revenue per hour for a specific client.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/client-profitability-comparator](https://vinkius.com/en/ai-agent-connect/client-profitability-comparator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Client Profitability Comparator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `client-profitability-comparator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Client Profitability Comparator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "client-profitability-comparator": {
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
