# MeasureSquare CRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/measuresquare-crm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage flooring and construction project estimates, client relationships, and job tracking for specialty contractors.

## Description
Connect your **MeasureSquare** account to any AI agent and manage flooring estimation workflows.

### What you can do

- **Project Management** — List and inspect flooring projects
- **Cost Estimation** — View detailed material and labor breakdowns
- **Room Details** — Access room dimensions and area calculations
- **Client CRM** — Browse and manage client contacts
- **Templates** — View estimation templates
- **PDF Reports** — Get downloadable project reports


## Available Tools
- **check_measuresquare_status**: Verify API connectivity
- **get_client**: Get client details
- **get_estimation**: Get project estimation
- **get_pdf_link**: Get project PDF
- **get_project_labor**: Get project labor
- **get_project_materials**: Get project materials
- **get_project_rooms**: Get project rooms
- **get_project**: Get project details
- **list_clients**: List clients
- **list_projects**: List all projects
- **list_templates**: List estimation templates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MeasureSquare CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my flooring projects."

**🤖 AI Agent:**
> You have 23 projects. Active: 'Smith Residence' (3 rooms, ,450), 'Office Reno' (12 rooms, ,200).

---

**👤 You:**
> "Show estimation for project prj_001."

**🤖 AI Agent:**
> Project 'Smith Residence': Materials ,200 (hardwood), Labor ,100 (24 hrs), Other ,150. Total: ,450.

---

**👤 You:**
> "Show rooms for project prj_001."

**🤖 AI Agent:**
> 3 rooms: Living Room (15x20ft, 300 sqft), Master Bedroom (12x14ft, 168 sqft), Kitchen (10x12ft, 120 sqft). Total: 588 sqft.


## ❓ FAQ

**Q: Can my AI get cost estimations?**
Yes. `get_estimation` returns a full breakdown of materials, labor, and total cost for any project.

**Q: Can I view room dimensions?**
Yes. `get_project_rooms` lists all rooms with length, width, and area calculations.

**Q: Can I download project PDFs?**
Yes. `get_pdf_link` returns the download URL for the professional project report.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/measuresquare-crm](https://vinkius.com/mcp/measuresquare-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MeasureSquare CRM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `measuresquare-crm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MeasureSquare CRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "measuresquare-crm": {
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
