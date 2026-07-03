# Itemized Shared Grocery Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/itemized-shared-grocery-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Split grocery receipts by item consumption and distribute tax equally.

## Description
This MCP server provides tools to accurately split a shared grocery receipt where individuals may have consumed different items. Using `get_unique_participants`, you can identify everyone involved in the trip. With `calculate_individual_subtotals`, you can determine exactly how much each person owes for their specific food consumption before tax. Finally, `compute_final_balances` calculates the total amount due by adding an equal share of the total tax to each participant's subtotal. It is perfect for roommates or friends splitting a shopping bill.


## Available Tools (3)
- **calculate_individual_subtotals**: Determine how much each person owes for the food items they specifically consumed, before tax
- **compute_final_balances**: Calculate the final amount each person must pay, including their share of the tax
- **get_unique_participants**: Identify every unique person involved in the shopping trip


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Itemized Shared Grocery Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Who participated in the grocery trip based on these items: [{'name': 'Milk', 'price': 4.50, 'consumedBy': ['Alice', 'Bob']}, {'name': 'Bread', 'price': 2.50, 'consumedBy': ['Bob']}]?"

**🤖 AI Agent:**
> The unique participants are Alice and Bob.

---

**👤 You:**
> "Calculate how much Bob owes for these items: [{'name': 'Milk', 'price': 4.50, 'consumedBy': ['Alice', 'Bob']}, {'name': 'Bread', 'price': 2.50, 'consumedBy': ['Bob']}]"

**🤖 AI Agent:**
> Bob's subtotal is $3.75 (half of the Milk at $2.25 and all of the Bread at $2.50, wait... 4.5/2=2.25 + 2.5 = 4.75). Let me re-calculate: Bob owes $4.75.

---

**👤 You:**
> "Calculate final balances for items: [{'name': 'Chips', 'price': 3.00, 'consumedBy': ['Alice', 'Charlie']}] with a tax of $1.00."

**🤖 AI Agent:**
> The participants are Alice and Charlie. Each pays $0.50 in tax. Alice owes $2.00 (item share) + $0.50 (tax) = $2.50. Charlie owes $2.00 (item share) + $0.50 (tax) = $2.50.


## ❓ FAQ

**Q: How does the tax split work?**
The total tax amount is divided equally among all participants identified in the receipt, regardless of which items they consumed.

**Q: What if someone didn't eat anything?**
If a person is listed in the items array but has no specific food costs, they will still be responsible for their equal share of the total tax.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, you can connect this MCP server to Cursor, VS Code, Claude Desktop, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/itemized-shared-grocery-splitter](https://vinkius.com/mcp/itemized-shared-grocery-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Itemized Shared Grocery Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `itemized-shared-grocery-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Itemized Shared Grocery Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "itemized-shared-grocery-splitter": {
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
