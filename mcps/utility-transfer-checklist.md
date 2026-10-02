# Utility Transfer Checklist MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/utility-transfer-checklist)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Schedules and tracks utility service transitions during property moves.

## Description
Manage the complexities of moving by coordinating utility service transitions. This MCP provides tools to schedule start and stop dates for services like water, electricity, gas, and internet based on your move date. Use `get_scheduled_tasks` to view your timeline, `get_missing_confirmations` to identify unconfirmed requests, and `get_deposit_summary` to track required financial commitments. You can also use `check_service_readiness` to ensure all service steps are completed before you move.


## Available Tools (4)
- **check_service_readiness**: Evaluates if all necessary steps for a specific service type are completed for the move
- **get_deposit_summary**: Calculates the total financial commitment required for the upcoming utility transfers
- **get_missing_confirmations**: Identifies utility actions that have been requested but have not yet received formal confirmation
- **get_scheduled_tasks**: Provides a chronological list of all utility-related actions that need to be performed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Utility Transfer Checklist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are my scheduled utility tasks for my move on 2025-06-15?"

**🤖 AI Agent:**
> On 2025-06-10, your Electric service will stop at the old location, and on 2025-06-15, your Water service will start at the new location.

---

**👤 You:**
> "Are there any utility confirmations missing for my move on 2025-06-15?"

**🤖 AI Agent:**
> Yes, the Gas service start request is missing confirmation and was required by 2025-06-08.

---

**👤 You:**
> "How much will my utility deposits cost for the move on 2025-06-15?"

**🤖 AI Agent:**
> The total deposit amount is $150.00, consisting of $100.00 for Electric and $50.00 for Water.


## ❓ FAQ

**Q: How do I see my upcoming utility tasks?**
You can use the `get_scheduled_tasks` tool by providing your move date to see a chronological list of all start and stop actions.

**Q: How can I check if my utility services are ready for the move?**
Use the `check_service_readiness` tool for a specific service type to verify if both start and stop tasks have been confirmed.

**Q: How do I track required deposits?**
The `get_deposit_summary` tool provides the total financial commitment and a breakdown of deposits needed for your service starts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/utility-transfer-checklist](https://vinkius.com/en/ai-agent-connect/utility-transfer-checklist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Utility Transfer Checklist** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `utility-transfer-checklist` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Utility Transfer Checklist** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "utility-transfer-checklist": {
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
