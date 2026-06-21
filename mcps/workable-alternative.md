# Workable MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/workable-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Streamline recruitment via Workable — list job openings, manage candidate profiles, and track hiring stages directly from your AI agent.

## Description
Connect your **Workable** account to any AI agent to manage your entire recruitment pipeline through natural conversation.

### What you can do

- **Job Management** — List all active job postings and fetch detailed descriptions using job shortcodes
- **Candidate Tracking** — Query candidate lists and retrieve full application details, including contact info and summaries
- **Pipeline Creation** — Create new candidate profiles and applications directly from the chat interface
- **Hiring Stages** — List and understand the different stages of your recruitment process to track progress
- **Team Overview** — Retrieve information about recruiters and team members involved in the hiring process

### How it works

1. Subscribe to this server
2. Enter your Workable API Key and Subdomain
3. Start managing your talent pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters & HR Managers** — quickly check candidate statuses and job details without switching between browser tabs
- **Hiring Managers** — review candidate profiles and job descriptions directly while planning team growth
- **Talent Acquisition Leads** — automate reporting on hiring stages and recruiter workloads


## Available Tools (7)
- **list_candidates**: List candidates in Workable
- **create_candidate**: Create a new candidate in Workable
- **get_candidate**: Get details for a specific candidate
- **get_job**: Get details for a specific job
- **list_jobs**: List job postings in Workable
- **list_recruiters**: List recruiters in Workable
- **list_stages**: List hiring stages in Workable


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Workable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all current job openings in Workable."

**🤖 AI Agent:**
> I've retrieved your active job postings. You have 3 open roles: 'Senior Backend Engineer' (Shortcode: BE-001), 'Product Designer' (Shortcode: PD-042), and 'Sales Lead' (Shortcode: SL-009).

---

**👤 You:**
> "Show me the profile for candidate ID 'cand_123'."

**🤖 AI Agent:**
> Fetching candidate details... This is Jane Doe. She is currently a 'Full Stack Developer' with 5 years of experience. Her application summary mentions expertise in React and Node.js.

---

**👤 You:**
> "Create a candidate profile for John Smith (john@email.com) with the headline 'Senior Developer'."

**🤖 AI Agent:**
> Candidate profile created successfully! John Smith has been added to your Workable account as a 'Senior Developer'.


## ❓ FAQ

**Q: Can I retrieve the full details of a specific job posting?**
Yes! Use the `get_job` tool with the job's shortcode. Your agent will return the full job description, requirements, and metadata associated with that posting.

**Q: Is it possible to add a new candidate directly through the AI?**
Absolutely. Use the `create_candidate` action. You can provide the candidate's name, email, headline, and a summary to instantly create their profile in your Workable account.

**Q: How can I see the different steps in our recruitment process?**
Simply ask the agent to run the `list_stages` tool. It will provide a list of all configured hiring stages, helping you understand where candidates are in the pipeline.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/workable-alternative](https://vinkius.com/mcp/workable-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Workable** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `workable-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Workable** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "workable-alternative": {
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
