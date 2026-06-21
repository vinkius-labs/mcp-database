# Pinpoint MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pinpoint)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate recruitment and talent acquisition via Pinpoint — manage jobs, applications, candidates, and interviews directly from any AI agent.

## Description
Connect your **Pinpoint** ATS account to any AI agent to streamline your hiring process and manage your talent pipeline through natural conversation.

### What you can do

- **Job Management** — List all active job postings, fetch specific job details, and create or update vacancies across departments and locations.
- **Application Tracking** — Monitor candidate progress, filter applications by stage (applied, review, interview, hired), and retrieve full application metadata.
- **Candidate Insights** — Access candidate profiles, update their information, and manage job seeker records efficiently.
- **Interview Coordination** — List and inspect interview schedules and details to keep the hiring team aligned.
- **Organizational Structure** — Query departments, locations, and divisions to maintain a structured overview of your recruitment needs.

### How it works

1. Subscribe to this server
2. Enter your Pinpoint API Key and Subdomain
3. Start managing your recruitment pipeline from Claude, Cursor, or any MCP-compatible client

No more jumping between browser tabs to check candidate statuses or job requirements. Your AI acts as a dedicated recruitment coordinator.

### Who is this for?

- **Recruiters & Talent Partners** — instantly retrieve application statuses and candidate details without leaving your workflow.
- **Hiring Managers** — review job descriptions and interview schedules directly from your communication tools.
- **HR Operations** — automate the querying of recruitment data for reporting and pipeline analysis.


## Available Tools (41)
- **create_application**: Create a new application
- **create_job_seeker**: Create a new job seeker
- **create_job**: Create a new job
- **create_requisition**: Create a new requisition
- **delete_application**: Delete an application
- **delete_job_seeker**: Delete a job seeker
- **delete_job**: Delete a job
- **delete_requisition**: Delete a requisition
- **delete_user**: Delete a user
- **get_application**: Get details for a specific application
- **get_candidate**: Get details for a specific candidate
- **get_department**: Get details for a specific department
- **get_division**: Get details for a specific division
- **get_interview**: Get details for a specific interview
- **get_job_seeker**: Get details for a specific job seeker
- **get_job**: Get details for a specific job
- **get_location**: Get details for a specific location
- **get_public_postings**: Does not require API key, but requires the subdomain.

Get public job postings for the company
- **get_requisition**: Get details for a specific requisition
- **get_user**: Get details for a specific user
- **list_applications**: List applications in Pinpoint
- **list_candidates**: List candidates in Pinpoint
- **list_custom_attributes**: List custom attributes in Pinpoint
- **list_departments**: List departments in Pinpoint
- **list_divisions**: List divisions in Pinpoint
- **list_interviews**: List interviews in Pinpoint
- **list_job_seekers**: List job seekers in Pinpoint
- **list_jobs**: Supports filtering by status, visibility, department, location, etc.

List jobs in Pinpoint
- **list_locations**: List locations in Pinpoint
- **list_onboarding_applications**: List onboarding applications in Pinpoint
- **list_questions**: List questions in Pinpoint
- **list_requisitions**: List requisitions in Pinpoint
- **list_scorecards**: List scorecards in Pinpoint
- **list_users**: List users in Pinpoint
- **update_application**: Update an existing application
- **update_candidate**: Update an existing candidate
- **update_interview**: Update an existing interview
- **update_job_seeker**: Update an existing job seeker
- **update_job**: Update an existing job
- **update_requisition**: Update an existing requisition
- **update_user**: Update an existing user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pinpoint** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active jobs in the Engineering department."

**🤖 AI Agent:**
> I've found 3 active jobs in Engineering: 'Senior Backend Engineer' (ID: 101), 'DevOps Lead' (ID: 105), and 'Frontend Developer' (ID: 110). Would you like more details on any of these?

---

**👤 You:**
> "Show me the details for application ID 55443."

**🤖 AI Agent:**
> Application 55443 is for the 'Product Manager' role. The candidate is currently in the 'Interview' stage. The last update was 2 days ago. Should I list the scheduled interviews for this candidate?

---

**👤 You:**
> "Get the interview schedule for candidate ID 9988."

**🤖 AI Agent:**
> Candidate 9988 has one upcoming interview: 'Technical Round' scheduled for tomorrow at 10:00 AM with the Engineering team. Would you like to see the scorecard requirements?


## ❓ FAQ

**Q: Can I filter job listings by a specific department or location?**
Yes! Use the `list_jobs` tool and provide the `department_id` or `location_id`. The agent will return only the jobs matching those organizational criteria.

**Q: How do I check the current stage of a specific application?**
You can use the `get_application` tool with the Application ID. It will provide the current stage (e.g., 'interview', 'offer') along with other relevant metadata.

**Q: Is it possible to update job details like requirements or descriptions via the agent?**
Yes, the `update_job` tool allows you to send a JSON:API formatted payload to modify existing job records directly from your conversation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pinpoint](https://vinkius.com/mcp/pinpoint)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pinpoint** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pinpoint` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pinpoint** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pinpoint": {
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
