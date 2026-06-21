# CATS ATS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cats-ats)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage recruitment workflows via CATS ATS — track candidates, job orders, and activities directly from any AI agent.

## Description
Connect your **CATS Applicant Tracking System (ATS)** account to any AI agent and take full control of your recruitment pipeline through natural conversation. Streamline candidate sourcing and job management.

### What you can do

- **Candidate Discovery** — Search and list candidate profiles with detailed contact information and status natively
- **Job Oversight** — List and retrieve details for all active job orders and open positions flawlessly
- **Activity Tracking** — Monitor recent recruitment activities, notes, and interactions securely
- **Organizational Mapping** — List client companies and associated contacts within your ATS flawlessly
- **HAL-native Integration** — Access deep object relationships through the CATS v3 HAL API structure in real-time
- **Pipeline Analysis** — Audit candidate progress across different recruitment stages directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your CATS v3 API Key (obtained from your account Administration)
3. Start managing your recruitment from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Recruiters & Headhunters** — search candidate databases and review application statuses using natural language
- **Hiring Managers** — monitor active job orders and recent candidate activities without opening the dashboard
- **HR Administrators** — manage client company data and staff contacts straight from their chat interface
- **Talent Acquisition Teams** — automate candidate lookups and recruitment reporting workflows


## Available Tools
- **get_candidate_details**: Get detailed information for a specific candidate
- **get_job_details**: Get detailed information for a specific job order
- **list_recruitment_activities**: List recent recruitment activities and notes
- **list_candidates**: List recruitment candidates
- **list_recruitment_companies**: List client companies in the ATS
- **list_recruitment_contacts**: List contacts associated with companies
- **list_job_orders**: List job orders and open positions
- **search_candidates**: Search for candidates using filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CATS ATS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for candidates named 'Sarah' in my CATS ATS."

**🤖 AI Agent:**
> Searching for 'Sarah'... I found 2 candidates: Sarah Miller (Applied for: Senior Developer) and Sarah Jones (Status: Interviewing). Would you like to see the full profile for either of them?

---

**👤 You:**
> "What are the active job orders right now?"

**🤖 AI Agent:**
> Checking active jobs... You currently have 5 open positions, including 'Marketing Manager', 'Product Designer', and 'Sales Executive'.

---

**👤 You:**
> "Show me the last 10 recruitment activities."

**🤖 AI Agent:**
> Retrieving recent activities... I found 10 entries including 3 new notes, 2 status changes, and 5 candidate registrations. Which activity type would you like to review?


## ❓ FAQ

**Q: Can I search for candidates by their name or status?**
Yes! Use the `search_candidates` tool with a filter like `first_name:"John"`. The agent will return matching profiles from your CATS database.

**Q: How do I see the latest notes added to a candidate?**
Use the `list_recruitment_activities` tool. Your agent will fetch the recent activity feed, which includes notes, status changes, and emails for all candidates.

**Q: Where do I find my CATS v3 API Key?**
Log in to your CATS account, go to 'Administration' and look for the 'API' section. You can generate and copy your v3 key from there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cats-ats](https://vinkius.com/mcp/cats-ats)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CATS ATS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cats-ats` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CATS ATS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cats-ats": {
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
