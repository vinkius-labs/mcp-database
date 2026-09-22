# Craft Night Cost Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/craft-night-cost-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage and settle expenses for organized crafting sessions.

## Description
This MCP server provides a specialized engine for managing the financial aspects of organized crafting events. It allows AI agents to record costs, calculate participant balances, and retrieve session summaries. Use `add_expense` to log shared materials, individual supplies, or facility costs. You can use `calculate_participant_balances` to determine exactly how much each person owes or is owed to settle debts, and `get_session_summary` for a high-level overview of total spending.


## Available Tools (4)
- **get_session_summary**: Provides a high-level financial overview of a single crafting session
- **list_session_expenses**: Retrieves a detailed itemized list of all costs incurred during a session
- **add_expense**: Records a new cost associated with a specific crafting session
- **calculate_participant_balances**: Determines exactly how much each person needs to pay or receive to settle the session debts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Craft Night Cost Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add a 25 dollar expense for shared glue to session session_123, paid by Alice."

**🤖 AI Agent:**
> The expense of $25.00 for shared glue has been recorded for session session_123.

---

**👤 You:**
> "What is the total spent in session session_456?"

**🤖 AI Agent:**
> The total spent in session session_456 is $142.50.

---

**👤 You:**
> "Show me all the expenses for session session_789."

**🤖 AI Agent:**
> There are 4 expenses recorded for session session_789: $10.00 (shared_material), $5.00 (facility), $15.00 (individual_supply), and $20.00 (facility).


## ❓ FAQ

**Q: How are shared costs split?**
Shared materials and facility costs are split equally among all participants in the session.

**Q: Can I record costs for a specific person?**
Yes, by using the `add_expense` tool with the 'individual_supply' category and providing a `recipientId`.

**Q: How do I know who needs to pay whom?**
You can use the `calculate_participant_balances` tool to get a list of net balances for every participant.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/craft-night-cost-tracker](https://vinkius.com/en/ai-agent-connect/craft-night-cost-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Craft Night Cost Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `craft-night-cost-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Craft Night Cost Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "craft-night-cost-tracker": {
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
