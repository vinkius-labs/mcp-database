# Mosaic (Resource Planning & Workforce Management) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mosaic-resource-planning-workforce-management)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage resource planning via Mosaic — track work plans, audit budget estimates, and monitor team capacity.

## Description
Connect your **Mosaicapp** account to any AI agent and take full control of your enterprise resource management, workforce planning, and project profitability through natural conversation.

### What you can do

- **Resource Orchestration** — List all managed team members and retrieve detailed profiles including roles, availability, and specific project assignments directly from your agent
- **Work Plan Tracking** — Extract complex timeline grids mapping Resource allocations across target operational projects to identify over-allocated or benched team members
- **Financial Profitability** — Audit budget estimates, bill rates, and cost rates for specific projects to track margins and financial boundaries natively within your workspace
- **Capacity Management** — List tracked explicitly mapped temporal calendar events and member check-ins to understand real-time organizational throughput
- **Project Portfolio Audit** — Enumerate high-level projects and initiatives to retrieve the underlying scope mappings where work plans and resources attach securely
- **Organizational Visibility** — Discover hierarchical roles and rate groups to understand how your project contributors are classified and billed across different initiatives
- **Currency & Units** — List team-specific currencies and measurement units used to scale financial logs and timekeeping activity mappings accurately

### How it works

1. Subscribe to this server
2. Enter your Mosaic API Token and X-Origin (Organization ID)
3. Start managing your workforce from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — monitor project work plans and resource assignments through natural conversation without manual grid navigation
- **Resource Leads** — track team capacity and identify potential burnout or under-utilization directly from your workspace
- **Operations Directors** — audit project budgets and billable rates efficiently to maintain high-profitability standards across the organization


## Available Tools (12)
- **list_members**: List all explicit team members mapped within Mosaic
- **get_member**: Get exact details parsing a given Mosaic team member
- **list_work_plans**: List scheduled organizational work plans mapping resources
- **list_calendar_events**: List tracked explicitly mapped temporal calendar events
- **list_check_ins**: List registered physical log check-ins bounded per member
- **list_budgets**: List simulated or structured budget estimates mapping projects
- **list_projects**: List high-level literal projects tracking organizational initiatives
- **list_bill_rates**: List organizational literal configuration tracking external bill rates
- **list_cost_rates**: List explicitly tracked unit limits mapping internal cost rates
- **list_rate_groups**: List defined structured arrays mapping generalized rate groups
- **list_roles**: List explicit categorical domains classifying member project roles
- **list_currencies**: List team literal currencies matching global models


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mosaic (Resource Planning & Workforce Management)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active team members in my Mosaic instance"

**🤖 AI Agent:**
> I've retrieved your list of team members. Highlights include Alex Smith (Senior Architect), Sarah Johnson (Project Manager), and Mark Rivera (Product Designer). Would you like to see the detailed project assignments for any of them?

---

**👤 You:**
> "Show me the work plan for the 'New Mobile App' project"

**🤖 AI Agent:**
> Retrieving work plans… I've identified the timeline for 'New Mobile App'. Sarah is allocated at 100% for the next 4 weeks, while Mark is at 50% capacity. There are 2 weeks where your UI resources are currently over-allocated. Would you like to check for available designers?

---

**👤 You:**
> "What is the budget estimate for project ID 'proj-98765'?"

**🤖 AI Agent:**
> Retrieving budget data for 'proj-98765'… The current estimate is $125,000 based on your resource mappings. This includes $85,000 in billable hours and $40,000 in operational overhead. I can break this down by role if you'd like.


## ❓ FAQ

**Q: Can I see my team's workload across different projects through my agent?**
Yes. Use the `list_work_plans` tool. Your agent will retrieve the hierarchical timeline mapping resources to projects, allowing you to see exactly how many hours are allocated to each member across your entire portfolio.

**Q: How do I check if a specific project is still within its estimated budget?**
The `list_budgets` tool allows your agent to retrieve financial estimates for a given Project ID. You'll see the structured budget models and applied rates, helping you monitor financial health through natural conversation.

**Q: Can my agent list all the roles and bill rates configured in our Mosaic account?**
Absolutely. Use the `list_roles` and `list_bill_rates` tools to identify your organizational allocation vectors. Your agent will report the roles and associated financial constants used to calculate project margins.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mosaic-resource-planning-workforce-management](https://vinkius.com/mcp/mosaic-resource-planning-workforce-management)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mosaic (Resource Planning & Workforce Management)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mosaic-resource-planning-workforce-management` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mosaic (Resource Planning & Workforce Management)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mosaic-resource-planning-workforce-management": {
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
