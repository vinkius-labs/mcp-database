# Dinner Reservation Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/dinner-reservation-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Fairly distribute restaurant bills, taxes, tips, and fees among diners.

## Description
This MCP server provides a precise calculation engine to split restaurant bills. It handles individual meal costs, proportional distribution of taxes and tips, global or item-specific discounts, and shared items like appetizers. It also manages group-wide costs like cancellation fees and applies credits from pre-paid deposits. Use `calculate_individual_shares` to get a full breakdown for every diner, `analyze_group_disparity` to see who is paying the most relative to the average, `validate_reservation_status` to check for cancellation penalties, or `split_shared_appetizers` to divide a single shared dish among specific participants.


## Available Tools (4)
- **analyze_group_disparity**: Identifies diners paying the highest percentage of the total bill compared to the group average
- **calculate_individual_shares**: Calculates the final amount each person owes, accounting for meals, tax, tip, discounts, and fees
- **split_shared_appetizers**: Splits the cost of a single shared item among a subset of diners
- **validate_reservation_status**: Determines if a cancellation fee should be applied based on reservation status and policy


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dinner Reservation Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the shares for a group where Alice had a $20 meal and Bob had a $30 meal, with an 8% tax, 20% tip, and a $5 cancellation fee."

**🤖 AI Agent:**
> Alice owes $27.00 and Bob owes $33.00.

---

**👤 You:**
> "Check if a cancelled reservation with a $50 flat fee should be charged for a $200 subtotal."

**🤖 AI Agent:**
> Yes, a fee of $50.00 should be charged.

---

**👤 You:**
> "Split a $15 appetizer between Charlie and Dave equally."

**🤖 AI Agent:**
> Each person owes $7.50.


## ❓ FAQ

**Q: How are taxes and tips calculated?**
Taxes and tips are distributed proportionally based on the weight of each person's meal subtotal relative to the group total.

**Q: Can I split a shared appetizer among only some people?**
Yes, you can use `split_shared_appetizers` to assign the cost of a specific item to a subset of diners.

**Q: How are cancellation fees handled?**
Cancellation fees are treated as group-wide costs and are split equally among all participants in the reservation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/dinner-reservation-splitter](https://vinkius.com/en/ai-agent-connect/dinner-reservation-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dinner Reservation Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dinner-reservation-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dinner Reservation Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dinner-reservation-splitter": {
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
