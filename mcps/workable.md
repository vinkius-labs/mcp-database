# Workable MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/workable)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Recruit top talent with an ATS that posts to 200+ job boards, screens candidates with AI, and manages the entire hiring flow.

## Description
Connect your **Workable** recruiting account to any AI agent and simplify how you manage your hiring pipelines, track candidates, and coordinate with your team through natural conversation.

### What you can do

- **Job Management** — List all active and archived job openings and retrieve detailed job descriptions and requirements.
- **Candidate Tracking** — List and inspect candidates across all jobs, and drill down into specific profiles for experience and status.
- **Direct Sourcing** — Programmatically register new candidates to specific job openings to accelerate your hiring process.
- **Team Coordination** — List account members and recruiters to understand your hiring team structure.
- **Ecosystem Overview** — List linked accounts and verify your Workable instance configuration via AI.

### How it works

1. Subscribe to this server
2. Enter your Workable Subdomain and API Key
3. Start managing your recruitment machine from Claude, Cursor, or any MCP client

### Who is this for?

- **Recruiters & HR Managers** — quickly check candidate statuses and job metadata via simple AI queries.
- **Hiring Managers** — monitor the progress of specific pipelines and review new applicants without opening the dashboard.
- **Operations Teams** — automate candidate registration and track team activity levels directly from the workspace.


## Available Tools (7)
- **create_candidate**: Register a new candidate to a job
- **get_candidate_profile**: Get details for a specific candidate
- **get_job_details**: Get details for a specific job
- **list_all_candidates**: List candidates across all jobs
- **list_jobs**: List active job openings
- **list_account_members**: List hiring team members
- **list_linked_accounts**: List connected accounts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Workable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active job openings in our Workable account."

**🤖 AI Agent:**
> I've retrieved your active jobs. You have 4 openings: 'Senior Frontend Engineer', 'Product Designer', 'DevOps Specialist', and 'Marketing Lead'. Which one would you like to see the details for?

---

**👤 You:**
> "Show me the details for the candidate 'John Smith'."

**🤖 AI Agent:**
> I've fetched John Smith's profile. He is currently in the 'Interview' stage for the 'Senior Frontend Engineer' role. He has 8 years of experience and is marked as 'Highly Recommended'.

---

**👤 You:**
> "Add 'Jane Doe' (jane.doe@example.com) as a candidate for the job 'ENG-101'."

**🤖 AI Agent:**
> Success! Jane Doe has been registered as a new candidate for job 'ENG-101' (shortcode: senior-frontend). I've added her email and initiated the application process.


## ❓ FAQ

**Q: How do I find the shortcode for a specific job?**
Use the `list_jobs` tool. It returns a list of all your openings, each with its unique shortcode required for more detailed queries or actions.

**Q: Can I add a new candidate directly to a job via AI?**
Yes! Use the `create_candidate` action. Provide the job shortcode along with the candidate's name and email to register them in your Workable pipeline.

**Q: Is it possible to see the recruiter assigned to an account?**
Absolutely. Run the `list_account_members` query to retrieve the directory of all users and recruiters in your instance, including their roles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/workable](https://vinkius.com/mcp/workable)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `workable` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Workable** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "workable": {
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
