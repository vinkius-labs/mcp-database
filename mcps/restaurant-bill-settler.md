# Restaurant Bill Settler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/restaurant-bill-settler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Precisely split restaurant bills, taxes, tips, and shared dishes among diners.

## Description
This MCP server provides a precise way to partition restaurant expenses. It handles individual ownership of items, proportional distribution of shared dishes, and calculates taxes and tips based on each person's subtotal. It also generates the most efficient reimbursement transfers to settle the bill. Use `calculate_individual_shares` to find itemized costs, `apply_tax_and_tip` for final totals, and `generate_reimbursements` to determine who pays whom.


## Available Tools (4)
- **generate_reimbursements**: Identifies the specific transfers needed to settle the bill
- **apply_tax_and_tip**: Calculates the final amount owed by each person after adding tax and gratuity
- **calculate_individual_shares**: Determines how much each person owes for their specific food and drink items, including their proportional share of shared dishes
- **validate_bill_integrity**: Ensures the provided menu and discount data are mathematically sound before processing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Restaurant Bill Settler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Split a bill where Alice ordered a $20 steak and Bob shared a $10 appetizer with Alice. Tax is 10% and tip is 20%."

**🤖 AI Agent:**
> Alice owes $18.00 for her steak and $5.00 for her share of the appetizer, totaling $23.00 after tax and tip. Bob owes $3.00 for his share of the appetizer, totaling $3.60 after tax and tip.

---

**👤 You:**
> "Calculate the reimbursement transfers if Charlie paid the whole bill and needs to be paid back by Dave and Eve."

**🤖 AI Agent:**
> Dave should pay Charlie $15.50 and Eve should pay Charlie $22.00.

---

**👤 You:**
> "Check if my menu items and discounts are consistent."

**🤖 AI Agent:**
> The bill is consistent. The sum of items minus discounts matches the expected total.


## ❓ FAQ

**Q: How are taxes and tips calculated?**
Taxes and tips are calculated proportionally. Each person pays a percentage of their specific food subtotal, ensuring fairness based on what they actually consumed.

**Q: How do I settle the bill with my friends?**
After calculating final totals, use the `generate_reimbursements` tool. It will provide the minimum number of transfers needed to bring everyone's balance to zero.

**Q: Can I handle shared dishes?**
Yes. By using `calculate_individual_shares`, you can specify which diners shared an item, and the cost will be split among them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/restaurant-bill-settler](https://vinkius.com/en/ai-agent-connect/restaurant-bill-settler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Restaurant Bill Settler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `restaurant-bill-settler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Restaurant Bill Settler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "restaurant-bill-settler": {
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
