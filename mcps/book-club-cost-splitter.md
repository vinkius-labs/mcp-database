# Book Club Cost Splitter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/book-club-cost-splitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Divide book club expenses equally among members with precise rounding.

## Description
This MCP server provides tools to manage shared costs within book clubs. It handles the mathematical complexity of splitting expenses, ensuring that rounding discrepancies are accounted for so that every cent is tracked. Use `calculate_split_per_member` to find the base share, `generate_payment_instructions` to get a clear list of who owes what, `validate_club_membership` to verify participant counts, and `get_club_expense_history` to review past spending.


## Available Tools (4)
- **calculate_split_per_member**: Determines how much each individual member owes for a single shared expense
- **generate_payment_instructions**: Provides a clear breakdown of who owes what and identifies the rounding discrepancy
- **get_club_expense_history**: Retrieves a summary of previous shared costs to help track club spending
- **validate_club_membership**: Verifies if a proposed split is mathematically sound based on the current member registry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Book Club Cost Splitter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We spent $45.50 on a new book. There are 4 members. How much does each person owe?"

**🤖 AI Agent:**
> Each member owes $11.37, with a $0.02 remainder to be adjusted.

---

**👤 You:**
> "Generate payment instructions for a $30.00 snack expense paid by Alice, split among 3 members."

**🤖 AI Agent:**
> Bob owes $10.00, Charlie owes $10.00, and Alice should receive $10.00 back.

---

**👤 You:**
> "Show me the history of expenses for 'books'."

**🤖 AI Agent:**
> The recorded book expenses are: $25.00 on 2023-10-01 and $45.50 on 2023-11-15.


## ❓ FAQ

**Q: How does the tool handle rounding errors?**
The `generate_payment_instructions` tool calculates a `roundingAdjustment` to ensure the sum of all individual payments exactly matches the total amount spent.

**Q: Can I filter past expenses by type?**
Yes, you can use `get_club_expense_history` with a `filterCategory` to view specific costs like 'books' or 'food'.

**Q: How do I ensure I am splitting with the correct number of people?**
You can use `validate_club_membership` by providing the proposed member count and the list of active member IDs to verify the split is valid.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/book-club-cost-splitter](https://vinkius.com/en/ai-agent-connect/book-club-cost-splitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Book Club Cost Splitter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `book-club-cost-splitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Book Club Cost Splitter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "book-club-cost-splitter": {
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
