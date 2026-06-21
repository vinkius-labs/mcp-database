# Jobtoolz MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jobtoolz)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage recruitment, jobs, and candidates via Jobtoolz API.

## Description
Empower your AI agents with Jobtoolz's recruitment management platform. This MCP server allows you to list jobs, track candidates, manage pipeline stages, and view departments and locations directly through the Jobtoolz API. Ideal for automating hiring workflows and candidate engagement.


## Available Tools
- **get_candidate**: Returns contact details, application history, and custom field values. Use this for deep-dive vetting of an applicant.

Retrieves details for a specific candidate
- **get_job**: Returns descriptions, requirements, and internal status. Essential for detailed analysis of a specific role.

Retrieves details for a specific job
- **list_candidates**: Includes candidate names, IDs, and current pipeline status. Use this to monitor applicant flow and identify recent entries.

Lists all candidates
- **list_departments**: Useful for filtering jobs and candidates by business unit (e.g., Sales, R&D).

Lists all departments
- **list_jobs**: Returns job titles, IDs, and departments. Use this to identify open positions and locate job IDs for candidate management.

Lists all active jobs
- **list_locations**: Useful for identifying jobs in specific geographical regions.

Lists all office locations
- **list_sources**: g., "Company Website", "Indeed") configured in Jobtoolz. Useful for auditing the origins of candidate traffic.

Lists all recruitment sources
- **list_stages**: g., "Applied", "Interview", "Offer"). Essential for understanding the company's hiring process.

Lists all configured pipeline stages
- **list_tags**: Useful for identifying valid tags before performing a tagged search.

Lists all configured tags
- **list_users**: Useful for identifying account administrators or hiring managers.

Lists all organization users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jobtoolz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all open jobs in Jobtoolz."

**🤖 AI Agent:**
> I'll fetch the list of active job openings from your Jobtoolz account.

---

**👤 You:**
> "Show me the details for candidate ID '123'."

**🤖 AI Agent:**
> I'll retrieve the full profile and status for that specific candidate from Jobtoolz.

---

**👤 You:**
> "Check the available recruitment sources."

**🤖 AI Agent:**
> I'll look up the list of configured recruitment sources in your Jobtoolz account.


## ❓ FAQ

**Q: How do I get Jobtoolz API credentials?**
Log in to your Jobtoolz account, navigate to Settings > API, and find your API Key.

**Q: Does it support departments and locations?**
Yes, you can list all configured departments and office locations using this MCP.

**Q: Can I see pipeline stages?**
Yes, the list_stages tool provides access to your recruitment pipeline configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jobtoolz](https://vinkius.com/mcp/jobtoolz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jobtoolz** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `jobtoolz` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jobtoolz** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jobtoolz": {
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
