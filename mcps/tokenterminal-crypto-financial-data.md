# TokenTerminal (Crypto Financial Data) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tokenterminal-crypto-financial-data)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Access institutional-grade crypto financial data — query project metrics, track revenue, and analyze market trends directly from your AI agent.

## Description
Connect **Token Terminal** to your AI agent to unlock deep financial insights into the crypto market. Analyze blockchains and dApps using the same data used by institutional investors.

### What you can do

- **Project Discovery** — List all tracked blockchains and decentralized applications to identify market leaders.
- **Detailed Metadata** — Fetch descriptions, categories, and social links for specific projects like Ethereum or Uniswap.
- **Financial Metrics** — Access historical time-series data for revenue, TVL, active users, and more.
- **Market Overview** — Get aggregated market metrics to understand broader sector trends and performance.

### How it works

1. Subscribe to this server
2. Enter your Token Terminal API Key
3. Start analyzing crypto fundamentals from Claude, Cursor, or any MCP client

### Who is this for?

- **Crypto Analysts** — perform fundamental analysis without leaving your research environment.
- **Investors** — track protocol revenue and growth metrics in real-time through natural language.
- **Developers** — integrate financial data into your workflow to build data-driven Web3 applications.


## Available Tools (4)
- **get_market_metrics**: Get aggregated market data metrics
- **get_project_metrics**: g., revenue, tvl, active_users) for a project.

Get historical time series metrics for a project
- **get_project**: Get detailed metadata for a specific project
- **list_projects**: List all projects tracked by Token Terminal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TokenTerminal (Crypto Financial Data)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all crypto projects tracked by Token Terminal."

**🤖 AI Agent:**
> I've retrieved the list of tracked projects. There are over 100 projects including Ethereum, Solana, Uniswap, and Aave. Would you like to see details for a specific one?

---

**👤 You:**
> "Show me the historical revenue and TVL for Ethereum over the last month."

**🤖 AI Agent:**
> Fetching metrics for Ethereum... In the last 30 days, Ethereum generated approximately $250M in revenue with a TVL maintaining around $50B. Would you like the daily breakdown?

---

**👤 You:**
> "What is the current aggregated market data for the crypto sector?"

**🤖 AI Agent:**
> Accessing market metrics... The total crypto market revenue across all tracked protocols is currently trending upwards, led by the L1 and DeFi sectors. I can provide specific sector growth rates if needed.


## ❓ FAQ

**Q: Can I get historical revenue for a specific protocol like Uniswap?**
Yes! Use the `get_project_metrics` tool with 'uniswap' as the project ID and specify 'revenue' in the metrics parameter to see historical financial performance.

**Q: How do I see which blockchains are currently tracked by the platform?**
Simply use the `list_projects` tool. It returns a comprehensive list of all blockchains and decentralized applications currently monitored by Token Terminal.

**Q: Is it possible to get a project's social links and category description?**
Yes, the `get_project` tool provides detailed metadata including the project's description, category, and official social media links.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tokenterminal-crypto-financial-data](https://vinkius.com/mcp/tokenterminal-crypto-financial-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TokenTerminal (Crypto Financial Data)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tokenterminal-crypto-financial-data` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TokenTerminal (Crypto Financial Data)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tokenterminal-crypto-financial-data": {
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
