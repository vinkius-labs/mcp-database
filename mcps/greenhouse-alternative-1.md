# Greenhouse MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/greenhouse-alternative-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your recruiting pipeline via Greenhouse — list applications, track candidate activity, and manage job board posts directly from any AI agent.

## Description
Connect your **Greenhouse** account to any AI agent to streamline your hiring process and candidate management through natural conversation.

### What you can do

- **Application Management** — List all applications, retrieve specific details, and update or delete candidate records using the Harvest API.
- **Candidate Insights** — Access the complete activity feed for any candidate to understand their journey and history.
- **Job Board Integration** — List published jobs, offices, and departments, and even submit applications directly to your job boards.
- **Candidate Ingestion** — Add new applications to existing candidates to keep your database up to date.

### How it works

1. Subscribe to this server
2. Enter your Greenhouse API Token
3. Start managing your recruitment workflow from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters & Sourcers** — quickly check candidate statuses and activity feeds without switching tabs.
- **Hiring Managers** — review job posts and application details directly within your workflow.
- **HR Operations** — automate the maintenance of candidate records and application data.


## Available Tools (16)
- **add_application_to_candidate**: Add an application to an existing candidate
- **create_partner_tracking_link**: Create a source-tracked link for a job
- **delete_application**: Delete a candidate application
- **get_application**: Retrieve a specific application
- **get_audit_log_events**: Retrieve audit log events
- **get_board_job**: Retrieve a specific job post and its questions
- **get_candidate_activity_feed**: Retrieve a candidate activity feed
- **get_partner_candidates**: Retrieve candidate status via Partner API
- **list_applications**: List all applications in Greenhouse
- **list_board_departments**: List departments and their associated jobs
- **list_board_jobs**: List all published job posts on a board
- **list_board_offices**: List offices and their associated jobs
- **list_partner_jobs**: List jobs visible to the partner user
- **submit_board_application**: Requires Job Board API Key credential.

Submit a job application to a board
- **submit_partner_candidate**: Submit new candidates or prospects
- **update_application**: Update an application


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Greenhouse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all current applications in Greenhouse."

**🤖 AI Agent:**
> I've retrieved the applications. You have 12 active applications, including 'Software Engineer' for Jane Doe and 'Product Manager' for John Smith. Would you like details on a specific one?

---

**👤 You:**
> "Show me the activity feed for candidate ID 98765."

**🤖 AI Agent:**
> Fetching activity for candidate 98765... The latest activities include a 'Technical Interview' completed yesterday and a status change to 'Offer Pending'.

---

**👤 You:**
> "What are the job posts currently listed on the 'tech-careers' board?"

**🤖 AI Agent:**
> I found 3 active posts on the 'tech-careers' board: Senior Backend Developer, UI/UX Designer, and DevOps Engineer. Do you need the full details for any of these?


## ❓ FAQ

**Q: Can I see the history of interactions with a specific candidate?**
Yes, you can use the `get_candidate_activity_feed` tool with a candidate's ID to retrieve their full activity history, including notes and status changes.

**Q: How do I list all open positions on our job board?**
Use the `list_board_jobs` tool providing your job board token. This will return all active job posts currently published.

**Q: Is it possible to update application details directly through the AI?**
Yes, the `update_application` tool allows you to modify existing application fields by providing the application ID and the data payload.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/greenhouse-alternative-1](https://vinkius.com/mcp/greenhouse-alternative-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Greenhouse** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `greenhouse-alternative-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Greenhouse** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "greenhouse-alternative-1": {
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
