# Hurma MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hurma)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your HR processes with employee records, leave tracking, and performance reviews designed for growing teams.

## Description
Connect your **Hurma** instance to any AI agent and manage your HR operations through natural conversation.

### What you can do

- **Recruiting Pipeline** — List all candidates, inspect profiles, create new candidate records, and track hiring progress
- **Employee Directory** — Browse all employees with department and position details
- **Time-Off Management** — Monitor out-of-office schedules and leave requests
- **Department Structure** — Browse organizational departments
- **Position Management** — List all job positions
- **Onboarding Tracking** — Monitor new hire checklists and progress

### How it works

1. Subscribe to this server
2. Enter your Hurma domain name and API Key
3. Start managing HR from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Teams** — manage candidates, employees, and leave without switching to the dashboard
- **Hiring Managers** — track recruiting pipeline and review candidate profiles
- **Team Leads** — monitor team availability and time-off schedules


## Available Tools
- **create_candidate**: Create a new candidate
- **create_leave_request**: Create a new leave or absence request
- **export_overtimes**: Export overtime data
- **get_vacation_balance**: Get employee vacation balance
- **get_candidate_details**: Get details for a specific candidate
- **get_employee_details**: Get details for a specific employee
- **list_candidates**: List recruitment candidates
- **list_departments**: List all company departments
- **list_employees**: List all employees
- **list_out_of_office**: List employees currently out of office
- **list_custom_properties**: List custom field definitions
- **list_vacancy_stages**: List recruitment stages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hurma** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all candidates in the pipeline and employees out of office this week."

**🤖 AI Agent:**
> Recruiting pipeline: 18 candidates. Applied (6), Screening (4), Interview (5), Offer (2), Hired (1). Top: 'Maria Silva' (Senior Dev, Interview), 'James Lee' (PM, Offer). Out of office: 3. Ana Costa — Vacation Apr 24-28, Mike Torres — Sick leave Apr 25, Lisa Park — Remote Apr 26.

---

**👤 You:**
> "List all employees in Engineering and create a new candidate for Senior Backend."

**🤖 AI Agent:**
> Engineering: 12 employees. Lead: Sarah Chen (VP). 2 open positions (Senior Backend, DevOps). Candidate created! Carlos Mendes, Senior Backend, Stage: Applied. Pipeline now 19 candidates.

---

**👤 You:**
> "Show onboarding status for new hires and all departments."

**🤖 AI Agent:**
> Onboarding: 3 active. Maria Silva (60%), João Santos (40%), Ana Lima (20%). Departments: 6. Engineering (12), Product (4), Design (3), Marketing (5), Sales (8), HR (3). Total: 35 employees.


## ❓ FAQ

**Q: Can I manage the recruiting pipeline through the AI agent?**
Yes. Use `list_candidates` to see all candidates with status, `get_candidate_details` for full profiles, and `create_candidate` to add new applicants.

**Q: Can I monitor who is out of office today?**
Yes. `list_out_of_office` retrieves all current and upcoming time-off entries. Use `list_leave_requests` for pending approvals and `get_leave_balances` for remaining vacation days.

**Q: Does Hurma require a custom domain in addition to the API Key?**
Yes. Each Hurma account has a unique subdomain. Provide the domain name and API Key. Requests go to `https://{domain}.hurma.work/api/v1` with a Bearer token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hurma](https://vinkius.com/mcp/hurma)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hurma** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hurma` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hurma** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hurma": {
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
