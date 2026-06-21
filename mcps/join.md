# Join MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/join)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage recruiting, jobs, and candidates via JOIN API.

## Description
Empower your AI agents with JOIN's modern recruiting platform. This MCP server allows you to list job openings, retrieve candidate details, manage applications, and view organization departments directly through the JOIN API. Ideal for automating hiring workflows and talent acquisition.


## Available Tools
- **get_application**: Returns answers to form questions, internal notes, and application status. Use when evaluating a specific applicant or moving them through the pipeline.

Retrieves details for a specific application
- **get_candidate**: Use this for detailed candidate vetting and interview preparation.

Retrieves details for a specific candidate
- **get_job**: Returns descriptions, requirements, and internal metadata. Use this when the user needs to analyze the specifics of a particular role or prepare content related to it.

Retrieves details for a specific job
- **get_me**: Use this to verify identity and check connection health.

Gets details about your own authenticated user
- **list_applications**: Includes candidate summaries and basic application info. Essential for monitoring recent applicant flow and identifying new leads in the recruitment process.

Lists all job applications
- **list_candidates**: Returns candidate profiles, contact info, and their association with jobs. Use this when the user wants to search for specific people or perform bulk talent management tasks.

Lists all candidates in the system
- **list_departments**: g., Engineering, Sales, HR). Useful for filtering jobs or organizing the recruiting workspace by functional areas.

Lists all organization departments
- **list_jobs**: Returns job titles, IDs, and current status. Use this as the primary entry point to identify specific jobs or to provide an overview of the current hiring pipeline.

Lists all job postings in JOIN
- **list_locations**: Use this when the user asks for jobs in specific regions or needs to audit location-based recruiting data.

Lists all job locations
- **list_users**: Useful for identifying hiring managers or checking account access permissions.

Lists all users in your JOIN account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Join** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active job postings in JOIN."

**🤖 AI Agent:**
> I'll fetch the list of open job postings from your JOIN account.

---

**👤 You:**
> "Show me the latest candidate applications."

**🤖 AI Agent:**
> I'll retrieve the most recent applications across all your jobs.

---

**👤 You:**
> "Get details for candidate ID '123'."

**🤖 AI Agent:**
> I'll retrieve the full profile and status for that specific candidate from JOIN.


## ❓ FAQ

**Q: How do I get JOIN API credentials?**
Log in to your JOIN account, navigate to User Settings > API Credentials, and generate a new token.

**Q: Can I see candidates for specific jobs?**
Yes, you can retrieve applications and candidates associated with your job postings using this MCP.

**Q: Does it support departments and locations?**
Yes, you can list all configured departments and office locations using the corresponding tools.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/join](https://vinkius.com/mcp/join)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Join** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `join` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Join** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "join": {
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
