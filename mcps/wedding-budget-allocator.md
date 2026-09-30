# Wedding Budget Allocator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wedding-budget-allocator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Manage and distribute wedding expenses across vendors, guests, and contingency funds.

## Description
The Wedding Budget Allocator is a specialized financial engine designed to manage wedding spending. It allows you to distribute a total budget across various vendor categories like `VENUE`, `CATERING`, and `PHOTOGRAPHY` while accounting for priority levels. You can use `allocate_vendor_budget` to assign funds to specific vendors, including tax and deposit calculations. The tool also handles guest-driven costs via `calculate_guest_costs` and ensures financial stability using `validate_budget_health` to keep all spending within your total budget and contingency reserves.


## Available Tools (4)
- **allocate_vendor_budget**: Assigns a specific portion of the budget to a single vendor or category
- **calculate_guest_costs**: Estimates costs that fluctuate based on the number of wedding guests
- **get_budget_summary**: Provides a high-level overview of the current financial standing
- **validate_budget_health**: Performs a comprehensive check to ensure all allocations stay within the total budget


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wedding Budget Allocator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a total budget of $30,000. I want to reserve 10% for emergencies. What is my available budget?"

**🤖 AI Agent:**
> With a $30,000 budget and a 10% contingency reserve ($3,000), you have $27,000 available for allocation.

---

**👤 You:**
> "Allocate $5,000 to the Catering vendor. It is an ESSENTIAL item, has a 7% tax rate, and requires a $500 deposit."

**🤖 AI Agent:**
> The allocation for Catering is complete. The total cost including 7% tax is $5,350, and after the $500 deposit, the remaining balance for this vendor is $4,850.

---

**👤 You:**
> "I have 120 guests and the catering cost is $85 per person with a 5% tax. How much will this cost in total?"

**🤖 AI Agent:**
> The total cost for 120 guests at $85 per person, including a 5% tax, is $10,710.


## ❓ FAQ

**Q: How does the tool handle taxes and deposits?**
When using `allocate_vendor_budget`, you can specify a tax rate and a deposit amount. The tool calculates the total cost including tax and tracks the remaining balance after the deposit is applied.

**Q: Can I set aside money for emergencies?**
Yes, you can use `get_budget_summary` to define a contingency percentage, which reserves a portion of your total budget for unforeseen expenses.

**Q: How are guest-related costs calculated?**
You can use `calculate_guest_costs` by providing the number of guests and the cost per person. The tool will calculate the total cost, including any applicable taxes.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wedding-budget-allocator](https://vinkius.com/en/ai-agent-connect/wedding-budget-allocator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wedding Budget Allocator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wedding-budget-allocator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wedding Budget Allocator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wedding-budget-allocator": {
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
