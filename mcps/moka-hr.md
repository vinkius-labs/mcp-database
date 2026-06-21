# Moka HR MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moka-hr)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Intelligent applicant tracking system (ATS) — manage jobs, candidates, and interviews via AI.

## Description
Empower your AI agent to orchestrate your recruitment lifecycle with **Moka HR**, the premier applicant tracking system for modern high-growth companies. By connecting Moka to your agent, you transform complex candidate tracking, job management, and interview coordination into a natural conversation. Your agent can instantly list open positions, retrieve candidate profiles, monitor interview schedules, and even provide recruitment summaries without you needing to navigate the complex Moka dashboard. Whether you are a hiring manager or a recruiter, your agent acts as a real-time talent assistant, keeping your hiring pipeline organized and your recruitment process efficient.

### What you can do

- **Job Orchestration** — List all active job postings and retrieve detailed requirements for any position.
- **Candidate Management** — Browse recruitment pipelines and manage candidate profiles, including contact details and history.
- **Interview Tracking** — Monitor scheduled interviews and retrieve session details instantly.
- **Application Control** — Manage the relationship between candidates and specific job applications.
- **Hiring Insights** — Retrieve high-level summaries of recruitment activity and pipeline statistics.

### How it works

1. Subscribe to this server
2. Enter your Moka API Key
3. Start managing your recruitment workflow through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters** — track candidate progress and manage job postings through natural language queries.
- **Hiring Managers** — monitor interview schedules and review candidate details directly from your AI-powered workspace.
- **HR Operations** — oversee multiple recruitment pipelines and audit activity summaries across the organization.
- **Moka Power Users** — integrate your existing recruitment workflows into your AI-driven daily routines.


## Available Tools
- **create_candidate**: Add new candidate
- **get_application**: Get application details
- **get_candidate**: Get candidate details
- **get_hiring_summary**: Get recruitment summary
- **get_interview**: Get interview details
- **get_job**: Get job details
- **list_applications**: List job applications
- **list_candidates**: List candidates
- **list_interviews**: List scheduled interviews
- **list_jobs**: List open job positions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moka HR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open job positions in our organization."

**🤖 AI Agent:**
> I've retrieved the active job postings from Moka. You have 8 open positions, including 'Senior Frontend Engineer' and 'Product Marketing Manager'. Would you like to see the details for any of them?

---

**👤 You:**
> "Show me the recruitment pipeline for candidate 'Mario'."

**🤖 AI Agent:**
> I've found candidate Mario in the system. He is currently in the 'Technical Interview' stage for the 'Backend Developer' position. His last interaction was a coding test review yesterday.

---

**👤 You:**
> "Get a summary of our hiring activity for this month."

**🤖 AI Agent:**
> I've compiled the monthly hiring summary. You've received 150 new applications, scheduled 42 interviews, and made 5 offers. The conversion rate from interview to offer is currently 12%. Would you like a breakdown by department?


## ❓ FAQ

**Q: How do I obtain a Moka API Key?**
You must contact your Moka Customer Success Manager (CSM) to enable the API Platform feature and receive your unique API Key.

**Q: Can I see interview schedules for my team?**
Yes. Use the `list_interviews` tool to see upcoming sessions. You can then use `get_interview` with a specific ID to see the full details, including participants and meeting links.

**Q: Is it possible to add a new candidate through the agent?**
Yes! Use the `create_candidate` tool. You will need to provide the candidate's name and email address. You can also optionally include their mobile number.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moka-hr](https://vinkius.com/mcp/moka-hr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moka HR** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `moka-hr` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moka HR** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moka-hr": {
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
