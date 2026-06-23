# JobScore MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jobscore)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage jobs, candidates, and hiring teams via JobScore ATS API.

## Description
Empower your AI agents with JobScore's comprehensive applicant tracking system. This MCP server allows you to list and retrieve job postings, track candidates, manage hiring teams and departments, and view hiring sources directly through the JobScore API. Ideal for automating recruitment workflows and talent acquisition.


## Available Tools (10)
- **get_candidate**: Returns contact history, resume highlights (if available), and current application status. Use this before an interview or when evaluating an applicant.

Retrieves details for a specific candidate
- **get_job**: Includes job descriptions, requirements, and hiring team identifiers. Use this to provide detailed information about a specific opening.

Retrieves details for a specific job
- **get_me**: Use this to verify connection status and identity.

Gets current authenticated user info
- **list_candidates**: Includes candidate names, current stage, and IDs. Essential for monitoring the talent pool and identifying new applications.

Lists all candidates
- **list_departments**: g., Engineering, Marketing) used to categorize jobs in JobScore. Useful for filtering hiring data by business unit.

Lists all departments
- **list_hiring_teams**: Useful for identifying recruiters and hiring managers associated with specific jobs.

Lists all hiring teams
- **list_jobs**: Returns job titles, IDs, and departments. Use this to identify active positions or find a job ID for candidate management.

Lists all jobs in JobScore
- **list_locations**: Useful for understanding the geographical scope of hiring efforts.

Lists all office locations
- **list_sources**: g., "LinkedIn", "Referral", "Job Board") from which candidates are originating. Essential for analyzing the effectiveness of hiring channels.

Lists all candidate sources
- **list_users**: Useful for identifying team members and their roles.

Lists all users in the account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JobScore** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open jobs in JobScore."

**🤖 AI Agent:**
> I'll fetch the list of active job postings from your JobScore account.

---

**👤 You:**
> "Show me the details for candidate ID '789'."

**🤖 AI Agent:**
> I'll retrieve the full profile and status for that specific candidate.

---

**👤 You:**
> "Check the hiring team for the 'Software Engineer' job."

**🤖 AI Agent:**
> I'll look up the members of the hiring team assigned to that position.


## ❓ FAQ

**Q: How do I get JobScore API credentials?**
Log in to your JobScore account, navigate to Admin > Integrations, and generate a Personal Access Token.

**Q: Does it support departments and locations?**
Yes, you can list all configured departments and office locations using this MCP.

**Q: Can I see candidate details?**
Yes, the list_candidates and get_candidate tools provide access to your applicant data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jobscore](https://vinkius.com/mcp/jobscore)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JobScore** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jobscore` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JobScore** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jobscore": {
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
