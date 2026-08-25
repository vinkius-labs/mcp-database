# Accelerator Pro-Rata Rights Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-pro-rata-rights-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Quantify the cost of maintaining ownership and the value of pro-rata rights during funding rounds.

## Description
This MCP server provides essential financial decision-support tools for accelerator investors. It allows users to calculate the exact capital required to prevent ownership dilution using `get_ownership_maintenance_cost`. Investors can also determine the intrinsic value of their participation through `evaluate_pro_rata_rights_value` and receive strategic investment recommendations via the `get_follow_on_decision_framework` tool. It is designed to help quantify the impact of up-rounds and manage follow-on capacity effectively.


## Available Tools (3)
- **evaluate_pro_rata_rights_value**: Calculates the financial value of having pro-rata rights in the current round
- **get_follow_on_decision_framework**: Provides a decision-making recommendation based on the investor's available capital and the cost of maintaining ownership
- **get_ownership_maintenance_cost**: Determines the exact amount of capital required to maintain the current ownership percentage in a new funding round


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Pro-Rata Rights Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will it cost me to maintain 10% ownership if the Series A raises $5,000,000 with a 2.0 up-round multiple?"

**🤖 AI Agent:**
> To maintain your 10% ownership, the required maintenance cost is $1,000,000.

---

**👤 You:**
> "I have $500,000 available for follow-on. If my maintenance cost is $800,000, what should my decision be?"

**🤖 AI Agent:**
> Based on your available capacity, the recommended decision is Partial Participation.

---

**👤 You:**
> "What is the value of my pro-rata rights if I invest $200,000 in a round where I maintain 5% ownership?"

**🤖 AI Agent:**
> The calculated value of your pro-rata rights for this investment is $25,000.


## ❓ FAQ

**Q: How do I calculate the cost to maintain my ownership percentage?**
You can use the `get_ownership_maintenance_cost` tool. Provide your current equity, the up-round multiple, and the total capital being raised in the new round.

**Q: Can this tool help with investment decisions?**
Yes, the `get_follow_on_decision_framework` tool provides specific recommendations like 'Full Participation' or 'Partial Participation' based on your available capacity and the maintenance cost.

**Q: What is the purpose of evaluating pro-rata rights value?**
The `evaluate_pro_rata_rights_value` tool helps you understand the financial benefit of exercising your rights by calculating the resulting ownership and the value of the investment relative to the dilution prevented.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-pro-rata-rights-analyzer](https://vinkius.com/ai-agent-connect/accelerator-pro-rata-rights-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Pro-Rata Rights Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-pro-rata-rights-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Pro-Rata Rights Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-pro-rata-rights-analyzer": {
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
