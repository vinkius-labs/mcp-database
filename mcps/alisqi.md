# AlisQI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alisqi)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Quality management orchestration — manage analysis sets, results, and QMS data via AI.

## Description
Connect your **AlisQI** instance to your AI agent to unlock professional quality management (QMS) orchestration. From auditing quality results and managing analysis sets to retrieving technical metadata for fields and monitoring workflow webhooks, your agent handles your quality operations through natural conversation.

### What you can do

- **Results Orchestration** — List, retrieve, and store quality results for any of your custom analysis sets
- **Schema Discovery** — List and audit analysis sets and their field definitions to understand your dynamic data model
- **Document Oversight** — Retrieve technical metadata for result attachments and monitor your quality documentation
- **Workflow Monitoring** — List active webhooks to ensure your quality event triggers (like non-conformities) are operational
- **QMS Insights** — Quickly identify quality trends or audit recent analysis entries directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your AlisQI Instance URL and Bearer Token
3. Start managing your quality data and monitoring QMS performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Quality Managers** — automate result audits and monitor non-conformity trends effortlessly
- **Laboratory Technicians** — quickly look up analysis requirements and enter quality data via chat
- **Operations Leads** — verify QMS data integrity and audit metadata definitions on the fly
- **Data Engineers** — trace quality data flows and inspect dynamic API responses using simple commands


## Available Tools (10)
- **list_analysis_sets**: List analysis sets
- **get_analysis_set_details**: Get set metadata
- **list_results**: Supports filtering.

List quality results
- **get_result_details**: Get specific result
- **store_results**: Create or update results
- **list_fields**: List dynamic fields
- **list_choice_lists**: List selection menus
- **get_result_attachments**: List document attachments
- **list_active_webhooks**: List active triggers
- **get_api_info**: Check API status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AlisQI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all analysis sets available in my AlisQI instance."

**🤖 AI Agent:**
> I've retrieved your analysis sets. You have 5 sets configured, including 'Raw Material Inspection', 'Final Product Audit', and 'Environmental Monitoring'. Would you like to see the field definitions for any of them?

---

**👤 You:**
> "Show the last 5 quality results for 'Raw Material Inspection'."

**🤖 AI Agent:**
> I've retrieved the latest 5 entries for Raw Material Inspection. All results were within specification limits, except for entry #98765, which showed a minor deviation in moisture content. Would you like the full details for that entry?

---

**👤 You:**
> "Check if there are any active webhooks for non-conformities."

**🤖 AI Agent:**
> I've checked your integration settings. You have 1 active webhook (ID: wh_123) configured to trigger when a non-conformity is detected. It is currently sending data to your incident management system. There are no reported errors.


## ❓ FAQ

**Q: How do I find my AlisQI Bearer Token?**
Log in to AlisQI, navigate to **Menu** > **Management** > **Integration Hub**. You can generate and manage your API tokens there. Each token inherits the permissions of the associated user account.

**Q: Is the data model the same for everyone?**
No, AlisQI uses a dynamic, user-defined data model. This means field names and analysis sets are specific to your company's configuration. Use the `list_analysis_sets` tool to discover your unique structure.

**Q: Can I attach files to quality results via the agent?**
Currently, the agent can retrieve metadata for existing attachments using the `get_result_attachments` tool. For uploading new files, we recommend using the AlisQI web interface or specific integration endpoints.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alisqi](https://vinkius.com/mcp/alisqi)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AlisQI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `alisqi` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AlisQI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "alisqi": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
