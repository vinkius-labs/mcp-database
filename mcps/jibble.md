# Jibble MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jibble)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Track time, attendance, and projects via Jibble API.

## Description
Empower your AI agents with Jibble's time tracking and attendance platform. This MCP server allows you to list time entries, retrieve person details, track activities and projects, and view organization information directly through the Jibble API. Ideal for automating workforce management and productivity analysis.


## Available Tools (10)
- **get_organization**: Use to verify account-wide configuration.

Retrieves organization details
- **get_person**: Essential for detailed HR analysis of an individual team member.

Retrieves details for a specific person
- **get_time_entry**: Returns location data, activity notes, and associated device info. Use for auditing or correcting a specific employee time log.

Retrieves details for a specific time entry
- **list_activities**: g., "Meeting", "Development", "Break") that employees can select when clocking in. Useful for identifying high-level task categories.

Lists all configured activities
- **list_clients**: Useful for professional services tracking and billable hours auditing.

Lists all configured clients
- **list_groups**: g., "Sales Team", "Remote Workers") used to organize the workforce. Useful for group-based performance reporting.

Lists all configured groups
- **list_locations**: Useful for auditing site-based workforce distribution.

Lists all configured locations
- **list_people**: Includes names, emails, and internal IDs. Use this to identify personnel before querying their time entries.

Lists all people in the organization
- **list_projects**: Use this when the user asks for a project-based time breakdown.

Lists all configured projects
- **list_time_entries**: Returns employee IDs, entry times, and durations. Use this to monitor workforce activity and total work hours.

Lists all time entries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Jibble** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all people in my Jibble organization."

**🤖 AI Agent:**
> I'll fetch the list of all members in your Jibble organization.

---

**👤 You:**
> "Show me the recent time entries."

**🤖 AI Agent:**
> I'll retrieve the latest time tracking entries from Jibble.

---

**👤 You:**
> "What are the active projects in Jibble?"

**🤖 AI Agent:**
> I'll look up the list of configured projects in your account.


## ❓ FAQ

**Q: How do I get Jibble API credentials?**
Log in to your Jibble account, navigate to Organization Settings > API, and generate a new Client ID and Client Secret.

**Q: Does it support activities and projects?**
Yes, you can list and retrieve data for both activities and projects using this MCP.

**Q: Can I see real-time attendance?**
Yes, the list_time_entries tool provides access to current and historical time tracking data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jibble](https://vinkius.com/mcp/jibble)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Jibble** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jibble` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Jibble** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jibble": {
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
