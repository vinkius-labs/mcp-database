# Household Maintenance History Book MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/household-maintenance-history-book)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Track and manage all household maintenance jobs, warranties, and upcoming service needs.

## Description
This MCP server provides a centralized system to manage your home's upkeep. It allows AI agents to retrieve a chronological history of all completed maintenance jobs using `get_maintenance_history`, identify upcoming service requirements or expiring warranties with `get_upcoming_actions`, check the health and service status of specific items via `get_asset_health_summary`, and evaluate service providers using `search_contractor_records`.


## Available Tools (4)
- **get_maintenance_history**: Provides a chronological list of all completed household maintenance jobs
- **get_upcoming_actions**: Identifies all scheduled or predicted maintenance tasks and expiring warranties
- **search_contractor_records**: Retrieves all jobs associated with a specific contractor
- **get_asset_health_summary**: Provides a high-level overview of the maintenance status for a specific asset


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Household Maintenance History Book** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What maintenance tasks are coming up in the next month?"

**🤖 AI Agent:**
> You have two immediate actions: the HVAC filter replacement is due on October 15th, and the water heater warranty expires on October 20th.

---

**👤 You:**
> "Show me the maintenance history for the Refrigerator."

**🤖 AI Agent:**
> The Refrigerator had its last service on May 12, 2023, for a compressor check, costing $150.

---

**👤 You:**
> "How reliable is 'Smith Plumbing'?"

**🤖 AI Agent:**
> Smith Plumbing has performed 5 jobs with an average cost of $200 per visit.


## ❓ FAQ

**Q: How can I see what maintenance is due soon?**
You can use the `get_upcoming_actions` tool to identify scheduled maintenance tasks and expiring warranties.

**Q: Can I check the status of a specific appliance?**
Yes, the `get_asset_health_summary` tool provides the last service date, total cost, and warranty status for any registered asset.

**Q: How do I view my past repair history?**
Use the `get_maintenance_history` tool to retrieve a full chronological list of all completed jobs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/household-maintenance-history-book](https://vinkius.com/en/ai-agent-connect/household-maintenance-history-book)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Household Maintenance History Book** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `household-maintenance-history-book` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Household Maintenance History Book** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "household-maintenance-history-book": {
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
