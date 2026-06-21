# ServiceM8 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/servicem8)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Run your field service business with job scheduling, quoting, invoicing, and GPS tracking from your phone or tablet.

## Description
Connect your **ServiceM8** account to any AI agent and take full control of your field service management workflows through natural conversation. ServiceM8 is the ultimate platform for trade and service businesses, and this integration allows you to orchestrate jobs, coordinate staff, and manage client relations without leaving your chat interface.

### What you can do

- **Job & Task Orchestration** — List all managed jobs and retrieve detailed metadata, including status and scheduled times programmatically.
- **Staff & Team Coordination** — Access and monitor your staff directory to maintain a clear overview of team assignments and availability directly from the AI interface.
- **Client CRM Control** — List and search through your client and contact database to keep your professional records synchronized via natural language.
- **Job Activity Tracking** — Access real-time activity logs for specific jobs to monitor progress and ensuring high-quality service delivery.
- **Operational Monitoring** — Track job categories and manage system metadata to ensure your field service operations are always optimized.

### How it works

1. Subscribe to this server
2. Enter your ServiceM8 API Key from your account settings
3. Start managing your field services from Claude, Cursor, or any MCP-compatible client

No more juggling spreadsheets or multiple browser tabs to see where your team is. Your AI acts as a dedicated dispatcher or operations manager.

### Who is this for?

- **Field Service Managers** — quickly retrieve job details and monitor staff schedules without switching apps.
- **Operations Teams** — automate the management of client records and track job activities via natural conversation.
- **Business Owners** — streamline the retrieval of service metadata and monitor organizational health directly within the chat.


## Available Tools (9)
- **create_job**: Requires description and company_uuid.

Create a new ServiceM8 job
- **get_company**: Get details for a specific company
- **get_job**: Get details for a specific job
- **list_categories**: List job categories
- **list_companies**: List all companies (clients)
- **list_contacts**: List all company contacts
- **list_job_activity**: Get activity history for a job
- **list_jobs**: List all ServiceM8 jobs
- **list_staff**: List ServiceM8 staff members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ServiceM8** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our active jobs on ServiceM8."

**🤖 AI Agent:**
> I've fetched your jobs. You have 5 active projects including 'AC Repair (Job #123)' and 'Kitchen Renovation'. Which one would you like to drill into?

---

**👤 You:**
> "Show me all staff members in the organization."

**🤖 AI Agent:**
> Retrieving staff list... I found 8 staff members including 'John Doe' (Technician) and 'Jane Smith' (Admin). Would you like to check the assignments for any of them?

---

**👤 You:**
> "Fetch the activity history for job UUID 550e8400-e29b-41d4-a716-446655440000."

**🤖 AI Agent:**
> Inspecting job activity... This job has 3 recorded activities: 'Job Created', 'Scheduled for 2PM', and 'Tech En Route'. Would you like the full timestamp details?


## ❓ FAQ

**Q: Can my AI automatically find the details and activity for a specific job just by providing its UUID?**
Yes! Use the `get_job` tool with the Job UUID. Your agent will respond with complete metadata, including status, scheduled times, and specific operational notes in seconds.

**Q: How do I list all staff members to check availability?**
Simply ask the agent to run the `list_staff` action. It will retrieve the full directory of staff members configured in your ServiceM8 account.

**Q: How do I find my ServiceM8 API Key?**
Log in to your ServiceM8 dashboard, navigate to **Settings** > **ServiceM8 Add-ons**, and enable the **API** add-on to find your unique API Key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/servicem8](https://vinkius.com/mcp/servicem8)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ServiceM8** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `servicem8` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ServiceM8** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "servicem8": {
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
