# Worksuite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/worksuite)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Freelancer management and global contractor onboarding via Worksuite directly through AI.

## Description
Connect your **Worksuite** (formerly Shortlist) account to any AI agent to automate your global talent management workflows. Manage your freelancer directory, job openings, projects, and payments through natural conversation.

### What you can do

- **Talent Orchestration** — List and search your talent directory with detailed metadata on freelancers and contractors.
- **Job Management** — Retrieve and monitor current job openings and recruitment stages directly from the AI interface.
- **Project Control** — Track project progress, milestones, and deliverables to ensure your contingent workforce is on schedule.
- **Payment Tracking** — Monitor payment statuses and invoice approvals for your global contractor network.
- **Workforce Intelligence** — Get a comprehensive overview of your external workforce capacity and project assignments using natural language.

### How it works

1. Subscribe to this server
2. Enter your Worksuite Base URL and API Key from your account settings
3. Start managing your talent network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Hiring Managers** — quickly check talent availability and recruitment status without switching tabs.
- **Project Leads** — monitor project milestones and contractor deliverables via natural conversation.
- **Operations Teams** — streamline the onboarding and payment tracking for global contingent workforces.


## Available Tools (9)
- **list_invoices**: List invoices
- **list_jobs**: List job openings
- **list_payments**: List payments
- **list_projects**: List projects in Worksuite
- **list_talents**: List all talents in Worksuite
- **list_tasks**: List tasks in Worksuite
- **get_job**: Get details of a job opening
- **get_project**: Get details of a specific project
- **get_talent**: Get details of a specific talent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Worksuite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active contractors in my Worksuite directory."

**🤖 AI Agent:**
> I've retrieved your directory. You have 25 active contractors. The most recent additions include 'John Doe' (Web Developer) and 'Jane Smith' (Graphic Designer).

---

**👤 You:**
> "Show the status of project 'Mobile App V2'."

**🤖 AI Agent:**
> Project 'Mobile App V2' is currently 'In Progress'. 3 out of 5 milestones have been completed by the assigned contractors. Would you like to see the pending tasks?


## ❓ FAQ

**Q: Where do I find my Worksuite API Key?**
API access is typically available on Enterprise or Plus plans. Navigate to your workspace settings or contact your Worksuite account manager to generate your unique API key.

**Q: What format should the Base URL follow?**
Your Base URL is usually your workspace domain followed by the API path, for example: `https://yourcompany.worksuite.com/api/v1`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/worksuite](https://vinkius.com/mcp/worksuite)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Worksuite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `worksuite` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Worksuite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "worksuite": {
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
