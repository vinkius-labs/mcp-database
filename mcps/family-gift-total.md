# Family Gift Total MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-gift-total)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage and aggregate gift costs for family events.

## Description
This MCP server helps you track gift spending for family events. You can use `add_gift_item` to record new purchases, `get_gift_total` to see the total amount spent, and `check_budget_status` to ensure you stay within your allocated budget. It also allows you to `list_gifts_by_recipient` to see exactly what has been planned for specific family members.


## Available Tools (4)
- **add_gift_item**: Requires recipient details, price, name, tier, and event.

Records a new gift purchase in the system
- **check_budget_status**: 
- **get_gift_total**: 
- **list_gifts_by_recipient**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Gift Total** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add a $50 watch for Mom for the Christmas event under Tier 1."

**🤖 AI Agent:**
> The watch for Mom has been recorded. The updated total for the Christmas event is $50.

---

**👤 You:**
> "How much have I spent on gifts for the Christmas event?"

**🤖 AI Agent:**
> You have spent a total of $50 on 1 gift for the Christmas event.

---

**👤 You:**
> "Am I over budget if my limit is $100 and I've spent $120?"

**🤖 AI Agent:**
> Yes, you are over budget by $20.


## ❓ FAQ

**Q: How do I add a new gift to my list?**
Use the `add_gift_item` tool and provide the recipient's name, the gift's price, the gift's name, their tier, and the event name.

**Q: Can I check if I am over my budget?**
Yes, you can use `check_budget_status` by providing your total budget amount to see your remaining balance or overage.

**Q: How can I see the total spent so far?**
You can call `get_gift_total` to get the sum of all recorded gifts, optionally filtered by a specific event name.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-gift-total](https://vinkius.com/en/ai-agent-connect/family-gift-total)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Gift Total** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-gift-total` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Gift Total** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-gift-total": {
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
