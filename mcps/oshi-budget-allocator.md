# Oshi Budget Allocator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/oshi-budget-allocator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

A deterministic budget tool for Oshi fans to balance fixed costs and discretionary spending.

## Description
Manage your monthly fan spending with precision. This MCP server helps Oshi fans (idol/VTuber enthusiasts) allocate a fixed monthly budget across various categories like merchandise and super chats. By using the `calculate_allocation` tool, you can ensure all mandatory fixed costs are covered first, then distribute the remaining funds based on your specific category priorities. You can also use `get_spending_summary` to see your total committed versus available funds at a glance.


## Available Tools (3)
- **calculate_allocation**: Calculates the exact distribution of funds across all specified spending categories
- **get_spending_summary**: Provides a high-level view of the total committed versus total available funds
- **validate_category_integrity**: Ensures that the provided categories and their specific costs are logically sound


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oshi Budget Allocator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Allocate a 50,000 JPY budget for my Oshi. Categories: merchandise (priority 5, fixed 10,000 JPY), super_chats (priority 3, fixed 5,000 JPY), and streaming_membership (priority 2, fixed 2,000 JPY)."

**🤖 AI Agent:**
> Your allocated amounts are: merchandise: 31,000 JPY, super_chats: 13,000 JPY, and streaming_membership: 6,000 JPY. You have 0 JPY remaining.

---

**👤 You:**
> "Show me a summary for a 20,000 JPY budget with merchandise (priority 4, fixed 15,000 JPY) and event_tickets (priority 1, fixed 10,000 JPY)."

**🤖 AI Agent:**
> Total fixed costs are 25,000 JPY. Since this exceeds your 20,000 JPY budget, you are in a deficit.

---

**👤 You:**
> "Check if my category list is valid: merchandise (priority 5, fixed 5000) and super_chats (priority 3, fixed -100)."

**🤖 AI Agent:**
> The category integrity check failed because a fixed cost cannot be a negative value.


## ❓ FAQ

**Q: How does the budget distribution work?**
The tool first deducts all fixed costs. The remaining budget is then distributed among categories based on their assigned priority (1-5) using a weighted method.

**Q: What happens if my fixed costs exceed my budget?**
The `calculate_allocation` tool will trigger an overspend flag, indicating that your mandatory costs have already exceeded your total monthly budget.

**Q: Can I use this with Cursor or Claude Desktop?**
Yes, you can connect this MCP server to Cursor, Claude Desktop, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/oshi-budget-allocator](https://vinkius.com/ai-agent-connect/oshi-budget-allocator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Oshi Budget Allocator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `oshi-budget-allocator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Oshi Budget Allocator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oshi-budget-allocator": {
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
