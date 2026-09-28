# Service History Record Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/service-history-record-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [asset-management](../categories/asset-management.md)

Manage asset maintenance, service schedules, and digital evidence organization.

## Description
This MCP connects AI agents to a specialized management system for tracking asset lifecycles. It provides tools to retrieve a complete service history using `get_service_history`, generate upcoming maintenance calendars with `get_upcoming_schedule`, construct organized digital evidence folders via `generate_evidence_manifest`, and verify maintenance compliance through `get_ownership_compliance`.


## Available Tools (4)
- **generate_evidence_manifest**: Constructs the logical folder structure and file paths for digital evidence
- **get_ownership_compliance**: Evaluates an asset's status against requirement rules
- **get_service_history**: Retrieves a complete chronological record of all service events for a specific asset
- **get_upcoming_schedule**: Generates a calendar of all future maintenance tasks that are due


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Service History Record Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the service history for asset ID ASSET-123."

**🤖 AI Agent:**
> The service history for ASSET-123 includes a completed oil change on 2023-10-15 by Vendor Alpha and a warranty inspection on 2024-01-10.

---

**👤 You:**
> "What maintenance is due between 2024-06-01 and 2024-12-31?"

**🤖 AI Agent:**
> The upcoming schedule includes a scheduled filter replacement for Generator-01 on 2024-08-15 and a safety check for Pump-05 on 2024-11-20.

---

**👤 You:**
> "Is asset ID ASSET-999 compliant?"

**🤖 AI Agent:**
> Asset ASSET-999 is currently compliant with an assigned vendor and an active warranty.


## ❓ FAQ

**Q: How can I see the maintenance history for a specific piece of equipment?**
You can use the `get_service_history` tool by providing the unique asset ID to retrieve a chronological log of all completed service events.

**Q: How do I know when the next service is due?**
The `get_upcoming_schedule` tool calculates future maintenance tasks based on the last recorded service and defined intervals.

**Q: Can I check if my asset documentation is complete?**
Yes, use `get_ownership_compliance` to evaluate if an asset has an assigned vendor, active warranty, and verified document locations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/service-history-record-plan](https://vinkius.com/en/ai-agent-connect/service-history-record-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Service History Record Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `service-history-record-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Service History Record Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "service-history-record-plan": {
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
