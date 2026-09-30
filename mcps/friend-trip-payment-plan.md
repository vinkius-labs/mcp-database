# Friend Trip Payment Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/friend-trip-payment-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage group travel finances, deposits, and peer-to-peer reimbursements.

## Description
This MCP server provides tools to coordinate group travel finances. It allows agents to monitor the total budget, track individual participant balances, and identify upcoming payment deadlines. You can use `get_trip_summary` to check the overall financial health of a trip, `get_participant_ledger` to see what a specific person owes, `calculate_upcoming_deadlines` to prepare for future costs, and `track_reimbursement` to record transfers between travelers to settle debts.


## Available Tools (4)
- **get_trip_summary**: Provides a high-level overview of the trip's financial health
- **track_reimbursement**: Records a transfer between two participants to settle internal debts
- **calculate_upcoming_deadlines**: Identifies all future payment requirements to help the group prepare for upcoming costs
- **get_participant_ledger**: Retrieves a detailed breakdown of a specific person's financial standing within the trip


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Friend Trip Payment Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current financial status of trip 'TRIP-123'?"

**🤖 AI Agent:**
> The trip 'TRIP-123' has a total budget of $1,200, with $800 collected so far and $400 remaining. The current status is 'active'.

---

**👤 You:**
> "How much does Alice still owe for the trip 'TRIP-123'?"

**🤖 AI Agent:**
> Alice has an allocation of $300, has paid $100, and her current balance is $200.

---

**👤 You:**
> "Are there any upcoming payments due in the next 7 days for trip 'TRIP-123'?"

**🤖 AI Agent:**
> Yes, there is a $150 deposit due on October 15th for the accommodation booking, affecting Bob and Charlie.


## ❓ FAQ

**Q: How can I check if a trip is fully paid?**
You can use the `get_trip_summary` tool to check the trip status and see if the remaining total has reached zero.

**Q: Can I record a payment between two friends?**
Yes, use the `track_reimbursement` tool to record transfers between participants to settle internal debts.

**Q: How do I know if someone has missed a payment?**
Use `get_participant_ledger` to check an individual's status; the `isOverdue` field will indicate if they have missed a deadline.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/friend-trip-payment-plan](https://vinkius.com/en/ai-agent-connect/friend-trip-payment-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Friend Trip Payment Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `friend-trip-payment-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Friend Trip Payment Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "friend-trip-payment-plan": {
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
