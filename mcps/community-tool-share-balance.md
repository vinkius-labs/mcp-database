# Community Tool Share Balance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/community-tool-share-balance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate member balances, booking costs, and pending payments for tool-sharing cooperatives.

## Description
This MCP server provides a financial reconciliation engine for community tool-sharing cooperatives. It connects AI agents to the cooperative's financial data, allowing for precise tracking of member accounts. Use `get_member_balance` to check if a member owes money or has credit, `calculate_booking_cost` to determine the total price of a rental including late fees, `get_member_activity_summary` for historical financial overviews, and `list_pending_payments` to identify debtors. It handles usage fees, late penalties, repair charges, and deposits.


## Available Tools (4)
- **get_member_balance**: To determine the current outstanding amount or credit for a specific member
- **calculate_booking_cost**: To calculate the total cost of a specific tool rental, including penalties
- **get_member_activity_summary**: To provide a high-level view of a member's financial interactions with the cooperative
- **list_pending_payments**: To identify members who currently owe money to the cooperative


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Community Tool Share Balance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current balance for member M123?"

**🤖 AI Agent:**
> Member M123 currently has a balance of $15.00, meaning they owe the cooperative fifteen dollars.

---

**👤 You:**
> "How much does booking B987 cost in total?"

**🤖 AI Agent:**
> The total cost for booking B987 is $25.00, which includes a $20.00 base fee and a $5.00 late fee.

---

**👤 You:**
> "List all members who owe more than $50."

**🤖 AI Agent:**
> The following members owe more than $50: Alice (Member ID: A01, Amount: $65.00) and Bob (Member ID: B02, Amount: $120.00).


## ❓ FAQ

**Q: How is a member's balance calculated?**
The balance is the sum of all usage fees, late penalties, and repair charges, minus any deposits and previous payments made by the member. You can use `get_member_balance` to retrieve this value.

**Q: Can I see a summary of a member's history?**
Yes, the `get_member_activity_summary` tool provides a high-level view of total fees charged, penalties incurred, and payments made over a specific period.

**Q: How do I find members who owe money?**
You can use the `list_pending_payments` tool to get a list of all members with a positive balance (debtors).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/community-tool-share-balance](https://vinkius.com/en/ai-agent-connect/community-tool-share-balance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Community Tool Share Balance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `community-tool-share-balance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Community Tool Share Balance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "community-tool-share-balance": {
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
