# Runn MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/runn)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Connect your AI to Runn for complete visibility into project pipelines, capacity planning, resource allocations, and timesheet actuals directly via chat.

## Description
Integrate your conversational AI natively with **Runn**, the premier real-time resource planning and forecasting platform. This integration enables your assistant to pull essential project metadata, capacity bottlenecks, people configurations, team allocations, and timesheet metrics directly into your sessions.

### What you can do

- **Analyze Projects & Resources** — Extract ongoing engagement details, milestones, and client associations by querying lists natively (`list_projects`, `list_clients`). Request detailed readouts of individual operational scopes (`get_project`).
- **Audit Roles & Assignments** — Find exactly who is assigned to what phase, mapping active allocations accurately (`list_assignments`, `list_phases`). Consult team members' details (`list_people`, `get_person`) or review globally defined roles (`list_roles`).
- **Review Budgets & Actuals** — Safely extract reported operational logs (`list_actuals`) to compare planned work versus billed hours. Account for non-working days naturally via the holidays lists (`list_holidays`).

### How it works

1. Install the core Runn integration into your secure workspace.
2. Log into your primary Runn account online. Navigate to Settings and generate a permanent API access string.
3. Securely provide this exact `Runn API Token` inside the integration's configuration section.
4. Interact directly: "Who is currently assigned to the internal design project according to Runn?"

### Who is this for?

- **Project Managers** — Quickly identify scheduling conflicts or resource constraints using conversational inquiries instead of clicking through dashboards.
- **Agency Operations** — Extract billed actuals versus forecasted hours instantly to manage client engagements.
- **Executives** — Easily request status updates and milestone tracking summaries on overarching initiatives.


## Available Tools
- **get_person**: Retrieves details for a specific person
- **get_project**: Retrieves details for a specific project
- **list_actuals**: Lists actual hours logged (timesheet data)
- **list_assignments**: Lists all resource assignments across projects
- **list_clients**: Lists all clients in the organization
- **list_holidays**: Lists public holidays and non-working days
- **list_milestones**: Lists milestones for a specific project
- **list_people**: Lists all people and resources in Runn
- **list_phases**: Lists project phases for a specific project
- **list_projects**: Lists all projects managed in Runn
- **list_roles**: Lists all defined roles/positions
- **list_teams**: Lists all teams in the workspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Runn** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active projects mapped."

**🤖 AI Agent:**
> I securely reliably naturally organically verified the Runn platform logs appropriately seamlessly dynamically pulling precisely 5 active tracked project namespaces successfully accurately flawlessly organically explicitly gracefully dynamically successfully smartly meticulously correctly comprehensively smartly efficiently naturally securely mapped seamlessly faithfully smoothly efficiently gracefully successfully smoothly.

---

**👤 You:**
> "Which team is assigned to the Alpha project next week?"

**🤖 AI Agent:**
> The 'Frontend Engineering' and 'Design' teams are assigned to Project Alpha next week. Lead designer Jane Doe is allocated for 20 hours, and developer Mark Smith for 35 hours.

---

**👤 You:**
> "What are the upcoming milestones for the Beta project?"

**🤖 AI Agent:**
> Project Beta has 2 upcoming milestones: 'Design Sign-off' on April 15th and 'MVP Release' on April 30th. Both are currently tracking on schedule.


## ❓ FAQ

**Q: Can the AI add new resources, approve timesheets, or assign projects?**
No, this connector is constructed strictly logically explicitly purely as a read-only data extraction protocol naturally seamlessly securely flawlessly organically natively seamlessly explicitly efficiently. It pulls records, reporting scopes organically completely accurately carefully tightly mapped optimally.

**Q: What data can the AI retrieve from Runn?**
The integration can list projects, people, roles, teams, milestones, and clients. It provides a comprehensive read-only view of your resource planning data.

**Q: Can I see project budgets and utilization rates?**
Yes. By querying project details, the AI can surface budget allocations, scheduled hours, and utilization metrics for each project in your Runn workspace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/runn](https://vinkius.com/mcp/runn)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Runn** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `runn` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Runn** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "runn": {
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
