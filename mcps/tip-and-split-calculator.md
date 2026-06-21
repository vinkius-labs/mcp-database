# Tip and Split Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tip-and-split-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate tip amounts, split bills among groups, and round totals for easy payment.

## Description
This MCP server provides specialized tools to manage restaurant billing. Use `calculate_tip_details` to determine the tip amount and final total based on a subtotal and percentage. Use `split_bill_share` to divide a bill among multiple people, ensuring everyone knows their individual share. Finally, use `format_practical_payment` to round amounts to practical increments like nickels, dimes, or dollars for easier physical or digital settlement.


## Available Tools
- **calculate_tip_details**: Calculate tip amount and final total
- **format_practical_payment**: g., nickels, dimes).

Round a calculated amount to a human-friendly value
- **split_bill_share**: Calculate the individual share of a bill


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tip and Split Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a 20% tip on a $50.00 bill."

**🤖 AI Agent:**
> The tip amount is $10.00, and the final total is $60.00.

---

**👤 You:**
> "Split a $120.00 bill among 4 people."

**🤖 AI Agent:**
> Each person's share is $30.00.

---

**👤 You:**
> "Round $14.37 to the nearest nickel."

**🤖 AI Agent:**
> The rounded amount is $14.35.


## ❓ FAQ

**Q: How do I calculate the tip?**
Use the `calculate_tip_details` tool by providing your subtotal and the desired tip percentage.

**Q: Can I split a bill with many people?**
Yes, use `split_bill_share` and specify the total amount and the number of participants.

**Q: What rounding levels are available?**
You can round to cents, nickels, dimes, quarters, or dollars using `format_practical_payment`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tip-and-split-calculator](https://vinkius.com/mcp/tip-and-split-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tip and Split Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `tip-and-split-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tip and Split Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tip-and-split-calculator": {
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
