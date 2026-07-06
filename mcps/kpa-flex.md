# KPA Flex MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kpa-flex)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage EHS compliance — list inspections, audit employees, and search reports.

## Description
Connect your AI agent to **KPA Flex** to maintain a safe and compliant workplace with real-time data access.

### Key Features

- **Inspection Auditing** — List and retrieve detailed safety inspection reports to identify workplace hazards
- **Employee Compliance** — Access individual employee EHS profiles including training and certification status
- **Form Schema Access** — View field definitions for custom audits and reporting forms
- **Asset Inventory** — Audit equipment and company assets managed within the KPA Flex ecosystem
- **Safety Intelligence** — Retrieve high-level site statistics and perform deep searches across all safety reports

### How to setup

1. Subscribe to this server
2. Log in to KPA Flex and generate an **API Key** from your profile or admin settings
3. Enter your key in the configuration panel
4. Start managing your EHS data via natural language


## Available Tools (10)
- **get_form_schema**: Get schema for a specific form
- **list_company_assets**: List equipment and assets
- **list_safety_trainings**: List training records
- **search_ehs_reports**: Search through all EHS reports
- **get_flex_site_stats**: Get high-level safety statistics
- **list_ehs_inspections**: List all safety inspections
- **get_inspection_details**: Get details for an inspection
- **list_flex_employees**: List employees in the system
- **get_employee_ehs_profile**: Get EHS profile for an employee
- **list_custom_forms**: List available custom forms


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KPA Flex** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all safety inspections from the last 7 days"

**🤖 AI Agent:**
> I've found 15 safety inspections conducted this week. 12 were marked as 'Compliant' and 3 have 'Open Issues'. Would you like to review the findings for the open ones?

---

**👤 You:**
> "Check compliance profile for employee 'EMP-555'"

**🤖 AI Agent:**
> Retrieved EHS profile for employee EMP-555 (John Smith). All 5 mandatory safety trainings are 'Completed' and current. No active incident reports found.

---

**👤 You:**
> "Search reports for keywords 'forklift incident'"

**🤖 AI Agent:**
> Searching safety reports… I found 2 reports matching 'forklift incident'. One from last month in Warehouse A and one from 2023. Which one should I open?


## ❓ FAQ

**Q: Where do I find my KPA Flex API Key?**
In KPA Flex, go to your profile settings or the administrative control panel to generate a new API Key for integration.

**Q: Can I see photos attached to inspections?**
The `get_inspection_details` tool returns metadata and links to resources, including photos if available.

**Q: Does this support creating new inspections?**
The current version focuses on data retrieval and auditing. Creation tools are being considered for future releases.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kpa-flex](https://vinkius.com/mcp/kpa-flex)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **KPA Flex** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kpa-flex` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **KPA Flex** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kpa-flex": {
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
