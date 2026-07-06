# eCompliance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ecompliance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Equip your AI agent to manage safety incidents, track inspections, and monitor action items via the eCompliance API.

## Description
Integrate **eCompliance**, the leading EHS (Environment, Health, and Safety) management platform, directly into your AI workflow. Manage your safety incidents and investigation statuses, track site inspections and findings, monitor corrective action items and due dates, and oversee employee safety records using natural language.

### What you can do

- **Incident Oversight** — List and retrieve detailed information, severity levels, and investigation status for all your safety incidents.
- **Inspection Intelligence** — Monitor site inspections, resolving individual checklist results, hazard observations, and completion statuses.
- **Action Item Monitoring** — Track corrective action items, descriptions, and due dates across your organization to ensure compliance.
- **Safety Auditing** — Retrieve high-level summaries of incident trends, inspection activity, and organizational safety metadata instantly.

### How it works

1. Connect the eCompliance integration to your AI assistant.
2. Authorize using your eCompliance API Key and Site ID.
3. Orchestrate your safety management and EHS compliance through intuitive conversation.

### Who is this for?

- **Safety Managers** — Quickly check daily incident reports and inspection completion on the go.
- **EHS Coordinators** — Monitor corrective action progress and hazard observations via chat.
- **Operations Leads** — Research specific incident details and organizational safety metadata instantly.


## Available Tools (10)
- **get_ecompliance_metadata**: Retrieve metadata and limits for your eCompliance account
- **list_site_employees**: List all employees registered at the current site
- **list_safety_incidents**: List all safety incidents recorded for the current site
- **get_incident_details**: Get detailed information and investigation status for a specific incident
- **get_inspection_details**: Get detailed results and findings for a specific inspection
- **quick_safety_health_audit**: Retrieve a high-level summary of incident and inspection activity
- **list_corrective_actions**: List all corrective action items and their current progress
- **list_safety_inspections**: List all safety inspections and audits performed at the site
- **list_latest_incidents**: Identify the most recently reported safety incidents
- **search_safety_incidents**: Search for incidents using a title or description keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **eCompliance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all safety incidents reported this week."

**🤖 AI Agent:**
> I've found 3 incidents reported this week, including 'Slip and Fall - Warehouse' and 'Near Miss - Loading Dock'. Would you like to see the investigation status for the Slip and Fall incident?

---

**👤 You:**
> "Show me the details for inspection 'INSP-12345'."

**🤖 AI Agent:**
> Inspection 'INSP-12345' (Title: Monthly Safety Walk) was completed on March 15th with a score of 92%. 2 hazards were observed and associated with new action items. Should I list the action items created from this inspection?

---

**👤 You:**
> "List all outstanding corrective actions."

**🤖 AI Agent:**
> There are 5 outstanding action items, including 'Repair Guardrail' (Due: March 30) and 'Update Safety Signage'. 2 items are currently past their due date. Would you like me to pull the assigned employee names for these items?


## ❓ FAQ

**Q: How do I get an eCompliance API Key?**
Log in to your eCompliance account as an administrator, navigate to **Settings > API**, and you can generate or retrieve your unique API Key from there. You will also need your Site ID.

**Q: Can the agent create new incident reports?**
This integration currently focuses on listing and auditing safety data. Filing new incident reports or performing inspections should be completed via the eCompliance mobile app or web portal to ensure proper capture of media and signatures.

**Q: Does the integration show employee safety training?**
Yes, you can use the list_site_employees tool to retrieve basic employee profile details. Detailed training records may vary based on your specific API permissions and account configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ecompliance](https://vinkius.com/mcp/ecompliance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **eCompliance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ecompliance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **eCompliance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ecompliance": {
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
