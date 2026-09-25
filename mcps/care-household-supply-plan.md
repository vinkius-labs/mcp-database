# Care Household Supply Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/care-household-supply-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automated replenishment scheduling and purchase management for household supplies.

## Description
This MCP server manages household inventory by connecting AI agents to your supply chain. It uses `get_replenishment_calendar` to predict when items will run out, `generate_purchase_assignments` to assign shopping duties based on budget and helper roles, `get_delivery_instructions` to provide storage guidance, and `get_out_of_stock_fallback` to suggest approved substitutes when items are unavailable.


## Available Tools (4)
- **generate_purchase_assignments**: Answers "Who is responsible for buying what, and how much will it cost?"
- **get_delivery_instructions**: Answers "How should items be received and where should they be stored?"
- **get_out_of_stock_fallback**: Answers "What should I do if an item is unavailable or out of stock?"
- **get_replenishment_calendar**: Answers "When will I run out of items, and when should I buy more?"


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Care Household Supply Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When will I run out of milk and laundry detergent?"

**🤖 AI Agent:**
> You will run out of milk on Tuesday, October 24th, and laundry detergent on Friday, October 27th.

---

**👤 You:**
> "Who is responsible for buying the groceries this week?"

**🤖 AI Agent:**
> John is assigned to buy milk and eggs, and Sarah is assigned to buy cleaning supplies.

---

**👤 You:**
> "What should I do if the brand of coffee I usually buy is unavailable?"

**🤖 AI Agent:**
> You should purchase the medium roast blend instead, as it is your primary preferred substitute.


## ❓ FAQ

**Q: How does the system decide when to reorder items?**
The system uses `get_replenishment_calendar` to monitor inventory levels against usage rates and reorder thresholds to trigger timely purchases.

**Q: Can I limit how much is spent on supplies?**
Yes, `generate_purchase_assignments` respects your defined budget limit and prioritizes urgent items if the budget is tight.

**Q: What happens if a specific item is out of stock?**
The `get_out_of_stock_fallback` tool will suggest a substitute from your pre-defined list of preferred alternatives.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/care-household-supply-plan](https://vinkius.com/en/ai-agent-connect/care-household-supply-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Care Household Supply Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `care-household-supply-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Care Household Supply Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "care-household-supply-plan": {
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
