# Cryptocurrency Tax Lot Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cryptocurrency-tax-lot-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate cost basis, realized gains, and tax liabilities using FIFO, LIFO, HIFO, and Specific Identification methods.

## Description
This MCP server provides a precision accounting engine for managing cryptocurrency tax lots. By using the `taxLotImpactTool`, you can process transaction histories including buys, sells, transfers, staking rewards, and airdrops. The tool calculates cost basis, distinguishes between short-term and long-term gains, and identifies potential wash sale risks. It supports multiple accounting methodologies: FIFO (First-In, First-Out), LIFO (Last-In, First-Out), HIFO (Highest-In, First-Out), and Specific Identification, allowing for highly accurate tax reporting and strategy optimization.


## Available Tools (1)
- **calculate_tax_lot_impact**: Calculate realized gain/loss for an asset using FIFO accounting


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cryptocurrency Tax Lot Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my realized gain for 0.5 BTC if I sold it at $60,000 with a cost basis of $40,000?"

**🤖 AI Agent:**
> Your realized gain for 0.5 BTC is $10,000.

---

**👤 You:**
> "Calculate the tax impact of selling 1 ETH at $3000 using FIFO."

**🤖 AI Agent:**
> The realized gain for 1 ETH is calculated based on your oldest available lot.

---

**👤 You:**
> "Check for potential wash sale warnings for my SOL transactions."

**🤖 AI Agent:**
> No recent wash sale warnings were detected for your SOL holdings.


## ❓ FAQ

**Q: Which accounting methods are supported?**
The server supports FIFO, LIFO, HIFO, and Specific Identification methods.

**Q: How do I calculate my gains?**
You can use the `taxLotImpactTool` by providing your transaction data in JSON format.

**Q: Does it handle staking rewards?**
Yes, the tool processes staking rewards and airdrops as acquisition events.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cryptocurrency-tax-lot-tracker](https://vinkius.com/mcp/cryptocurrency-tax-lot-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cryptocurrency Tax Lot Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cryptocurrency-tax-lot-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cryptocurrency Tax Lot Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cryptocurrency-tax-lot-tracker": {
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
