# Shared Custody Exchange Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/shared-custody-exchange-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Transforms raw custody data into structured, operational exchange schedules.

## Description
This MCP server acts as a logistics engine for co-parenting. It converts raw input data--such as exchange dates, locations, transport details, and belongings--into a clear, chronological operational schedule. Use `generate_exchange_schedule` to build the timeline, `validate_transition_logistics` to ensure rules are followed, and `filter_operational_view` to provide parents with a clean summary of what, where, and when. It also includes `resolve_belongings_discrepancy` to ensure no essential items are left behind during transitions.


## Available Tools (4)
- **filter_operational_view**: Removes all non-essential data to provide a clean view for the parents
- **generate_exchange_schedule**: Converts raw input data into a chronological sequence of operational steps
- **resolve_belongings_discrepancy**: Identifies if any required items from the belongings list have been omitted from the generated schedule
- **validate_transition_logistics**: Checks if the proposed exchange plan adheres to the agreed-upon transport and contact rules


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shared Custody Exchange Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an exchange schedule for a pickup at the local library on Friday at 5 PM."

**🤖 AI Agent:**
> The exchange is scheduled for Friday at 5:00 PM at the Local Library. Parent B will pick up the child.

---

**👤 You:**
> "Check if the child's school bag and jacket are included in the schedule."

**🤖 AI Agent:**
> The school bag and jacket are both accounted for in the upcoming exchange event.

---

**👤 You:**
> "Show me a summary of the upcoming exchange."

**🤖 AI Agent:**
> Exchange: Saturday, Oct 12th at 10:00 AM at Central Park.


## ❓ FAQ

**Q: How do I create a schedule?**
You can use the `generate_exchange_schedule` tool by providing the exchange dates, transport details, and the list of belongings.

**Q: Can I check if my plan follows the agreed rules?**
Yes, the `validate_transition_logistics` tool checks the proposed schedule against your specific transport and contact constraints.

**Q: How can I see a simplified view for the parents?**
Use the `filter_operational_view` tool with the 'summary' mode to see only the essential dates and locations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/shared-custody-exchange-plan](https://vinkius.com/en/ai-agent-connect/shared-custody-exchange-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shared Custody Exchange Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shared-custody-exchange-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shared Custody Exchange Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shared-custody-exchange-plan": {
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
