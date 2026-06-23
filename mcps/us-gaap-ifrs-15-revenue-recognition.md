# US GAAP & IFRS 15 Revenue Recognition MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-gaap-ifrs-15-revenue-recognition)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Automate ASC 606 and IFRS 15 revenue recognition by identifying obligations, allocating prices, and calculating progress.

## Description
This MCP server provides a specialized engine for implementing the five-step model of ASC 606 and IFRS 15. It allows AI agents to automate complex financial calculations required for revenue recognition. Use `identify_performance_obligations` to analyze contract items, `allocate_transaction_price` to distribute total consideration based on relative standalone selling prices, and `calculate_revenue_recognition` to determine earned versus deferred revenue based on completion progress.


## Available Tools (3)
- **allocate_transaction_price**: Distribute total transaction price across performance obligations
- **calculate_revenue_recognition**: Calculate recognized and deferred revenue
- **identify_performance_obligations**: Analyze contract items to determine performance obligations


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US GAAP & IFRS 15 Revenue Recognition** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a contract with two items: 'Software License' and 'Support Services'. How many performance obligations are there?"

**🤖 AI Agent:**
> The `identify_performance_obligations` tool identifies 2 distinct performance obligations: Software License and Support Services.

---

**👤 You:**
> "Allocate a $10,000 total price between 'License' ($8,000 SSP) and 'Support' ($2,000 SSP)."

**🤖 AI Agent:**
> The allocated amounts are: License: $8,000 and Support: $2,000.

---

**👤 You:**
> "If I have an allocated amount of $5,000 and I am 40% complete, how much revenue is recognized?"

**🤖 AI Agent:**
> $2,000 has been recognized as revenue, and $3,000 remains as deferred revenue.


## ❓ FAQ

**Q: How does the tool identify performance obligations?**
The `identify_performance_abilities` tool analyzes a list of contract items to determine which are distinct enough to be treated as separate promises under the ASC 606 framework.

**Q: How is the transaction price allocated?**
Using `allocate_transaction_price`, the total contract value is distributed across all identified obligations proportionally, based on their relative Standalone Selling Price (SSP).

**Q: Can I calculate deferred revenue?**
Yes. The `calculate_revenue_recognition` tool calculates both recognized revenue (earned) and deferred revenue (remaining balance) based on the percentage of completion provided.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-gaap-ifrs-15-revenue-recognition](https://vinkius.com/mcp/us-gaap-ifrs-15-revenue-recognition)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US GAAP & IFRS 15 Revenue Recognition** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-gaap-ifrs-15-revenue-recognition` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US GAAP & IFRS 15 Revenue Recognition** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-gaap-ifrs-15-revenue-recognition": {
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
