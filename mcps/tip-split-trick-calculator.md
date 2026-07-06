# Tip Split Trick Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tip-split-trick-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Fast restaurant bill math for even and uneven splits, pre-tax vs. post-tax tipping, and tax breakdowns.

## Description
The Tip Split Trick Calculator is a high-speed utility designed to handle the complexities of restaurant billing. Whether you are splitting an equal bill among friends or calculating individual shares based on different orders, this tool provides instant clarity. Use `even_split_calculator` to determine what each person owes in a group split, including both pre-tax and post-tax tipping scenarios. For groups with varying order totals, `uneven_split_calculator` distributes tax and tip proportionally to each person's contribution. Additionally, use `tax_summary_calculator` to isolate the tax amount and see the total impact of taxes on your bill.


## Available Tools (3)
- **uneven_split_calculator**: Calculate how much each person owes based on individual order values
- **even_split_calculator**: Calculate how much each person owes when splitting a bill equally
- **tax_summary_calculator**: Calculate the specific tax portion and new total


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tip Split Trick Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We have a bill of $100 with 8% tax and we want to tip 20%. There are 4 of us splitting equally. How much does each person owe?"

**🤖 AI Agent:**
> Using the pre-tax method, each person owes $28.00. Using the post-tax method, each person owes $29.60.

---

**👤 You:**
> "I ordered $20 and my friend ordered $30. The total bill is $50 with 10% tax and a 18% tip. How much should each of us pay?"

**🤖 AI Agent:**
> The person who ordered $20 owes $23.60, and the person who ordered $30 owes $35.40.

---

**👤 You:**
> "What is the tax on a $50 meal with an 8% tax rate?"

**🤖 AI Agent:**
> The total tax amount is $4.00, making the post-tax total $54.00.


## ❓ FAQ

**Q: What is the difference between pre-tax and post-tax tipping?**
Pre-tax tipping calculates the tip percentage based only on the cost of food and drinks before tax is added. Post-tax tipping calculates the tip based on the total amount including both the base cost and the tax.

**Q: How does the uneven split calculator work?**
The `uneven_split_calculator` takes an array of individual order amounts. It then calculates each person's proportional share of the total tax and tip based on their contribution to the base amount.

**Q: Can I calculate just the tax amount?**
Yes, you can use the `tax_summary_calculator` to find the exact tax value and the new total after tax is applied.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tip-split-trick-calculator](https://vinkius.com/mcp/tip-split-trick-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tip Split Trick Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tip-split-trick-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tip Split Trick Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tip-split-trick-calculator": {
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
