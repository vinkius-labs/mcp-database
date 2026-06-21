# US Depreciation Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-depreciation-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate US asset depreciation using MACRS, Section 179, and Bonus Depreciation rules.

## Description
This MCP server provides AI agents with specialized tools to calculate complex US tax depreciation. Using `get_asset_class_info`, agents can retrieve recovery periods for different asset classes like vehicles or buildings. The `calculate_depreciation_schedule` tool generates a full year-by-year breakdown of expenses, accounting for Section 179 expensing and Bonus Depreciation. Additionally, `calculate_expensing_impact` allows agents to compare the immediate tax benefits of accelerated expensing methods against standard MACRS depreciation.


## Available Tools
- **calculate_depreciation_schedule**: Generate a year-by-year depreciation schedule
- **calculate_expensing_impact**: Compare the impact of Section 179 and Bonus Depreciation against standard MACRS
- **get_asset_class_info**: g., car, residential, commercial).

Get information about a specific asset class


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Depreciation Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the recovery period for a commercial building?"

**🤖 AI Agent:**
> You can find this by calling `get_asset_class_info` with 'commercial' as the asset class name.

---

**👤 You:**
> "Calculate a depreciation schedule for a car costing $30,000 with $5,000 Section 179 expensing."

**🤖 AI Agent:**
> The agent would use `calculate_depreciation_schedule` with 'car', an initial cost of 30000, and a section179Amount of 5000.

---

**👤 You:**
> "Show me the tax benefit impact for a $50,000 asset with 80% bonus depreciation."

**🤖 AI Agent:**
> The agent would use `calculate_expensing_impact` providing the cost, a bonusPercentage of 0.8, and any applicable Section 179 amount.


## ❓ FAQ

**Q: How can I find the recovery period for a specific asset?**
You can use the `get_asset_class_info` tool by providing the asset class name, such as 'car', 'residential', or 'commercial'.

**Q: Does the calculator support Section 179 expensing?**
Yes. The `calculate_depreciation_schedule` tool allows you to input a Section 179 amount to reduce the initial cost basis before calculating MACRS and Bonus Depreciation.

**Q: Can I compare different depreciation strategies?**
Yes. Use the `calculate_expensing_impact` tool to see the net benefit of using Section 179 and Bonus Depreciation compared to standard MACRS.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-depreciation-calculator](https://vinkius.com/mcp/us-depreciation-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Depreciation Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `us-depreciation-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Depreciation Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-depreciation-calculator": {
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
