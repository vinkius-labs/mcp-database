# Greenhouse MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/greenhouse)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your recruiting pipeline via Greenhouse — list candidates, track applications, and audit jobs directly via AI.

## Description
Connect your **Greenhouse Recruiting** account to any AI agent and take control of your talent acquisition pipeline through natural conversation.

### What you can do

- **Candidate Oversight** — List all candidates in your system and retrieve specific profile details natively
- **Pipeline Tracking** — Monitor job applications and their current statuses across your active hiring processes flawlessly
- **Job Management** — List and inspect job configurations, including hiring stages and department mappings synchronously
- **Team Coordination** — Retrieve office and department structures to ensure your hiring data is aligned with organizational goals
- **User Auditing** — List and verify user roles and access levels within your Greenhouse workspace natively

### How it works

1. Subscribe to this server
2. Enter your Greenhouse Harvest API Key (v1/v2)
3. Start managing your recruiting operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters & Sources** — quickly search for candidates and verify application statuses without manual dashboard navigation
- **Hiring Managers** — audit job stages and review candidate profiles directly through the chat interface
- **HR Operations** — manage office and department lists and verify user access levels synchronously


## Available Tools (12)
- **create_candidate**: Create a new candidate profile
- **get_application**: Get details for a specific application
- **get_candidate**: Get details for a specific candidate
- **get_job**: Get details for a specific job
- **get_user**: Get details for a specific user
- **list_applications**: Retrieve job applications
- **list_candidates**: List all candidates in Greenhouse
- **list_departments**: List company departments
- **list_job_stages**: List hiring stages for a specific job
- **list_jobs**: List jobs in Greenhouse
- **list_offices**: List company offices
- **list_users**: List Greenhouse users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Greenhouse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active jobs in Greenhouse"

**🤖 AI Agent:**
> Retrieving your active jobs... I found 4 openings: 'Senior Frontend Engineer' (ID: 402), 'Product Designer' (ID: 405), 'Marketing Manager' (ID: 410), and 'Data Scientist' (ID: 412). Would you like to see the applications for any of these?

---

**👤 You:**
> "Show me the profile for candidate ID 93021"

**🤖 AI Agent:**
> Fetching candidate details... Candidate #93021 is John Doe. He is currently in the 'Technical Interview' stage for the Senior Engineer role. His latest resume was uploaded 3 days ago.

---

**👤 You:**
> "What are the hiring stages for the 'Product Designer' job?"

**🤖 AI Agent:**
> Retrieving job stages... For the 'Product Designer' role (ID: 405), the hiring process includes: 1. Application Review, 2. Portfolio Review, 3. Phone Screen, 4. Design Exercise, and 5. Executive Interview.


## ❓ FAQ

**Q: Can my agent list all candidates for a specific job in Greenhouse?**
Yes. Use the 'list_candidates' tool with the 'job_id' parameter. The agent will fetch all candidates associated with that specific opening flawlessly.

**Q: How do I check the current hiring stage of an applicant via chat?**
You can use the 'get_application' tool. Provide the Application ID, and the agent will return the full details, including the candidate's current stage in the hiring process natively.

**Q: Can I search for candidates who were added recently through the agent?**
Absolutely. Use the 'list_candidates' tool with sorting or filtering parameters like 'created_after'. Your agent will retrieve the most recent additions to your Greenhouse database natively.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/greenhouse](https://vinkius.com/mcp/greenhouse)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `greenhouse` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Greenhouse** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "greenhouse": {
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
