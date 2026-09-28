# Family Equipment Sharing Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/family-equipment-sharing-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Coordinate shared gear, maintenance, and reservations within a group.

## Description
This MCP server provides a management system for coordinating the borrowing, maintenance, and storage of shared equipment within a family or group. It allows users to manage reservation precedence, track equipment states, and handle maintenance cycles. Use `get_equipment_calendar` to view usage timelines, `check_reservation_availability` to verify gear availability, `register_checkout_report` to document item condition, `get_maintenance_reminders` to track service needs, and `resolve_usage_conflict` to manage disputes like late returns or damage.


## Available Tools (5)
- **register_checkout_report**: Records the condition of equipment at the moment a user takes possession
- **check_reservation_availability**: Determines if a specific piece of equipment can be borrowed for a requested period
- **get_equipment_calendar**: Provides a chronological view of all equipment usage and maintenance
- **get_maintenance_reminders**: Identifies all equipment that is due for service or has been flagged for issues
- **resolve_usage_conflict**: Provides a guided path to resolve disputes when a return is late or an item is returned damaged


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Family Equipment Sharing Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the equipment schedule for next week."

**🤖 AI Agent:**
> Here is the equipment calendar for next week: Monday: Lawn Mower (User: Alice), Wednesday: Power Drill (Maintenance), Friday: Bicycle (User: Bob).

---

**👤 You:**
> "Is the camping tent available from June 1st to June 5th?"

**🤖 AI Agent:**
> Yes, the camping tent is available for those dates.

---

**👤 You:**
> "I just picked up the pressure washer. What is the status?"

**🤖 AI Agent:**
> The checkout report for the pressure washer has been successfully registered with ID R-12345.


## ❓ FAQ

**Q: How can I see when a piece of equipment is available?**
You can use the `check_reservation_availability` tool to see if a specific item is free for your requested dates.

**Q: What happens if an item is returned damaged?**
You should use `resolve_usage_conflict` to follow the guided steps for handling damage discrepancies.

**Q: How do I know if something needs servicing?**
Run `get_maintenance_reminders` to see a list of all equipment due for service or flagged for issues.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/family-equipment-sharing-plan](https://vinkius.com/en/ai-agent-connect/family-equipment-sharing-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Family Equipment Sharing Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `family-equipment-sharing-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Family Equipment Sharing Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "family-equipment-sharing-plan": {
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
