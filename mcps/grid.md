# Grid MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/grid)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/grid-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/grid-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Turn spreadsheet data into interactive dashboards and visual stories that make numbers accessible to every stakeholder.

## Description
Connect your **WorkOnGrid** account to any AI agent and take full control of your field operations and operational data management through natural conversation.

### What you can do

- **Worksheet Orchestration** — List all operational worksheets and retrieve detailed technical metadata and structures programmatically
- **Field Data Capture** — Create, update, and search for records within your worksheets to track inspections, asset status, and team productivity
- **Operational Visibility** — Monitor analytical dashboards and manage team member access to maintain high-fidelity oversight of your workflows
- **Asset Tracking** — List and manage supported asset types to ensure precise inventory management and field record accuracy
- **System Monitoring** — Check API health and manage outbound webhooks directly through your agent for reliable operational automation

### How it works

1. Subscribe to this server
2. Retrieve your **Client ID** and **Secret** from the Grid dashboard (Integrations / API Connectors)
3. Start managing your field data and operations from Claude, Cursor, or any MCP client

No more manual report entry or digging through complex data tables. Your AI acts as your dedicated field operations coordinator.

### Who is this for?

- **Operations Managers** — instantly retrieve field reports and monitor project progress using natural language
- **Field Supervisors** — update worksheet records and track team activities without leaving your workspace
- **Data Analysts** — automate the extraction of operational data for custom reporting and BI integration


## Available Tools
- **check_api_health**: Verify Grid API connectivity
- **create_new_operational_record**: g., a new inspection report) into a specific worksheet.

Add a new record to a worksheet
- **remove_worksheet_record**: Delete a record from a worksheet
- **get_authenticated_user_profile**: Get authenticated user info
- **get_worksheet_details**: Get details for a specific worksheet
- **list_supported_asset_types**: List common asset categories
- **list_grid_dashboards**: List available dashboards
- **list_worksheet_records**: List records from a worksheet
- **list_team_members**: List organization users
- **list_configured_webhooks**: List active webhooks
- **list_grid_worksheets**: List all operational worksheets
- **update_worksheet_record**: Modify an existing operational record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Grid** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active worksheets in my Grid account."

**🤖 AI Agent:**
> I've retrieved your worksheets. You have 3 active structures: 'Site Safety Checks' (ID: ws_123), 'Equipment Maintenance' (ID: ws_456), and 'Asset Inventory' (ID: ws_789). Which one should I inspect or update?

---

**👤 You:**
> "Add a maintenance record to 'ws_456' for 'Excavator EX01'."

**🤖 AI Agent:**
> Record created! I've logged the maintenance entry for Excavator EX01 in the 'Equipment Maintenance' worksheet. The entry is now visible in your Grid dashboard for team review.

---

**👤 You:**
> "Show me the latest dashboard status for field operations."

**🤖 AI Agent:**
> Fetching dashboard metadata... I found your 'Field Operations Overview' dashboard. It indicates 85% completion across active sites with 12 records updated in the last hour. Would you like a detailed breakdown by site?


## Installation & Usage

To install and use the **Grid** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/grid](https://vinkius.com/mcp/grid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*
