# Namely MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/namely)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage HRIS data via Namely — track employee profiles, job info, and organization groups directly from your AI agent.

## Description
Connect your **Namely** HRIS account to your AI agent and take full control of your organization's employee data and structures through natural conversation.

### What you can do

- **Employee Directory** — List all employee profiles and get detailed information including contact info and roles.
- **Job & Salary Info** — Access a complete list of job titles and salary structures defined in your organization.
- **Org Structure** — View all groups, departments, and teams to understand your organizational hierarchy.
- **HR Timeline** — Monitor organization events like birthdays and work anniversaries.
- **Custom Fields & Reports** — List available reports and custom data fields defined for your profiles.
- **Company Feed** — Access recent company-wide announcements from the Namely home feed.

### How it works

1. Subscribe to this server
2. Enter your Namely Company Slug and API Token
3. Start managing your HR data from Claude, Cursor, or any MCP client

### Who is this for?

- **HR Managers** — quickly check employee details or organization structures without opening the Namely portal.
- **IT & Operations** — automate the retrieval of employee lists for provisioning or reporting.
- **Team Leads** — verify team members and job titles through natural language commands.


## Available Tools (10)
- **get_profile**: Get specific employee details
- **get_team**: Get team details
- **list_announcements**: List company announcements
- **list_events**: g., birthdays, work anniversaries) from the organization timeline.

List HR events
- **list_fields**: List custom employee fields
- **list_groups**: g., departments, offices) in your organization.

List organization groups
- **list_jobs**: List job titles and info
- **list_profiles**: List employee profiles
- **list_reports**: List HR reports
- **list_teams**: List organization teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Namely** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all employees in the 'Engineering' department."

**🤖 AI Agent:**
> I've retrieved the profiles for the Engineering department. You have 15 members, including 'David Smith' (Lead Developer), 'Elena Rodriguez' (Senior QA), and 13 others. Shall I show you the contact info for David?

---

**👤 You:**
> "What company announcements were posted recently?"

**🤖 AI Agent:**
> I've checked the company feed. There are 3 recent announcements: 'New Office Safety Guidelines', 'Q3 Performance Review Kickoff', and 'Welcome Our New Hires!'. Would you like the full text for the safety guidelines?

---

**👤 You:**
> "Show me upcoming birthdays in the organization."

**🤖 AI Agent:**
> Retrieving upcoming events... We have 4 birthdays this week: Sarah Jenkins (Tomorrow), Michael Chen (Thursday), and two others on Saturday. Shall I get their Slack handles for you?


## ❓ FAQ

**Q: How do I get a Namely API Token?**
You can generate a Personal Access Token in your Namely account under API > Personal Access Tokens. Ensure your user has the appropriate permissions to view the data you want to retrieve.

**Q: Can I see salary information through this server?**
This depends on the permissions of the user who generated the API token. If your Namely user can see salary data, the `get_profile` and `list_jobs` tools will return that information.

**Q: What is the Company Slug?**
The slug is the unique part of your Namely URL. For example, if you log in at 'acme.namely.com', your slug is 'acme'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/namely](https://vinkius.com/mcp/namely)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Namely** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `namely` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Namely** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "namely": {
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
