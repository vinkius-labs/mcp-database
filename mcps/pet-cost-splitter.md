# Pet Cost Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pet-cost-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Divide shared pet expenses equally among owners.

## Description
Manage shared pet care costs with precision. This MCP server provides tools to calculate equal splits for expenses, track spending by owner, and validate new entries. Use `get_expense_split` to divide a bill among multiple owners, `get_total_spending_per_owner` to see individual contributions, and `validate_expense_entry` to ensure new costs follow business rules.


## Available Tools (4)
- **get_expense_split**: Calculates how much each owner owes for a specific expense
- **get_total_spending_per_owner**: Aggregates the total amount spent by each owner across all pet expenses
- **list_expenses_by_category**: Retrieves all recorded expenses filtered by a specific type of pet care
- **validate_expense_entry**: Checks if a proposed expense entry is valid according to business rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pet Cost Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Split a $50.00 vet bill between Alice and Bob."

**🤖 AI Agent:**
> Alice owes $25.00 and Bob owes $25.00.

---

**👤 You:**
> "How much has Charlie spent in total?"

**🤖 AI Agent:**
> Charlie has spent a total of $120.50.

---

**👤 You:**
> "Is it valid to enter a pet food expense for $15.00 for owners Dave and Eve?"

**🤖 AI Agent:**
> Yes, the expense entry is valid.


## ❓ FAQ

**Q: How does the split calculation handle rounding?**
To ensure the total matches the original amount exactly, the final owner in the list is assigned any remaining fractional cents.

**Q: Can I see how much a specific person has spent?**
Yes, you can use `get_total_spending_per_owner` to retrieve the total amount spent by a specific owner.

**Q: What categories of expenses are supported?**
Supported categories include Food, Medical, Grooming, Supplies, and Services.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pet-cost-splitter](https://vinkius.com/en/ai-agent-connect/pet-cost-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pet Cost Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pet-cost-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pet Cost Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pet-cost-splitter": {
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
