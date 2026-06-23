# SignOnSite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/signonsite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Track who enters and exits your construction sites with digital sign-in, safety inductions, and compliance documentation.

## Description
Connect your **SignOnSite** account to any AI agent and take full control of your construction site safety and attendance orchestration through natural conversation. SignOnSite provides a premier platform for managing worker sign-ons, safety inductions, and site attendance, and this integration allows you to retrieve site metadata, monitor worker enrollments, and track safety briefings directly from your chat interface.

### What you can do

- **Worker & Site Orchestration** — List all active sites and retrieve detailed worker profile metadata, including enrollment status and contact info programmatically.
- **Attendance Lifecycle Management** — Monitor real-time worker sign-ons and sign-offs to ensure your site attendance is always accurate directly from the AI interface.
- **Safety & Permit Control** — Access and monitor site permits and safety briefings to ensure your workplace compliance is always synchronized via natural language.
- **Enrolment & Credential Intelligence** — Access worker credentials and manage enrolment flows to keep your compliance records up to date.
- **Operational Monitoring** — Track site activities and manage company metadata to ensure your safety orchestration is always optimized using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your SignOnSite API Token from your dashboard
3. Start managing your site safety from Claude, Cursor, or any MCP-compatible client

No more manual sign-on sheets or chasing safety certificates. Your AI acts as a dedicated safety officer or site manager.

### Who is this for?

- **Site Managers & Foremen** — quickly retrieve worker attendance and monitor safety induction statuses without switching apps.
- **Safety Officers** — automate the retrieval of site permits and track compliance credentials via natural conversation.
- **Operations Teams** — streamline the retrieval of site-user metadata and monitor multi-site activities directly within the chat.


## Available Tools (12)
- **enrol_worker**: Enrol a new worker
- **get_site_details**: Get details for a specific site
- **get_worker_details**: Get details for a specific worker
- **list_companies**: List all associated companies
- **list_sites**: List all construction sites
- **list_workers**: List all site workers
- **query_site_attendance**: Supports filtering by site and date.

Query worker attendance records
- **query_worker_credentials**: Check worker licenses and inductions
- **query_form_submissions**: Query completed safety forms
- **query_permits**: g., Hot Works, Confined Space) for your projects.

Query safety permits
- **sign_off_worker**: Record a manual sign-off for a worker
- **sign_on_worker**: Record a manual sign-on for a worker


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SignOnSite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all workers currently signed onto the 'Skyline Apartments' site."

**🤖 AI Agent:**
> I've retrieved the attendance list. There are currently 12 workers on site, including 'John Miller' and 'Sarah Chen'. Would you like to see their contact info or induction status?

---

**👤 You:**
> "Show me any active permits for site ID 12345."

**🤖 AI Agent:**
> Checking site permits... I found 3 active permits for site 12345: 'Hot Works', 'Working at Heights', and 'Excavation'. Would you like the full details for any of them?

---

**👤 You:**
> "Check if worker 'Robert Smith' is enrolled for the 'City Hospital' site."

**🤖 AI Agent:**
> Searching worker records... 'Robert Smith' is successfully enrolled for 'City Hospital' and has completed his general induction. Should I check his specific equipment credentials?


## ❓ FAQ

**Q: Can my AI automatically find which workers are currently signed onto a specific construction site?**
Yes! Use the `query_attendance` tool. Provide the Site ID, and your agent will return the list of currently present workers and their sign-on times in seconds.

**Q: How do I check if a specific worker has completed their safety induction for a site?**
Simply ask the agent to run the `get_worker` or `query_credentials` action. It will retrieve the enrollment status and safety credentials for that individual.

**Q: How do I find my SignOnSite API Token?**
Log in to your SignOnSite web dashboard, navigate to the **Settings** > **API** section, and you will find your unique Company API Token there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/signonsite](https://vinkius.com/mcp/signonsite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SignOnSite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `signonsite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SignOnSite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "signonsite": {
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
