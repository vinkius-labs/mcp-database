# EnterpriseAlumni MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/enterprisealumni)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage alumni networks, track engagement, and monitor member profiles via the EnterpriseAlumni API.

## Description
Integrate **EnterpriseAlumni**, the strategic alumni engagement platform, directly into your AI workflow. Manage your corporate and academic alumni networks, track member profiles and professional history, monitor upcoming events and job board postings, and oversee your community engagement using natural language.

### What you can do

- **Member Oversight** — List and retrieve detailed profiles, career history, and contact information for all your alumni members.
- **Engagement Intelligence** — Monitor network engagement metrics, resolving activity levels and community participation trends.
- **Content Management** — Access and monitor alumni events and job board postings, tracking registration and application statuses.
- **Network Auditing** — Retrieve high-level summaries of member volume, event activity, and organizational network health instantly.

### How it works

1. Connect the EnterpriseAlumni integration to your AI assistant.
2. Authorize using your EnterpriseAlumni REST API Key (found in your admin settings).
3. Orchestrate your alumni relations and corporate community strategy through intuitive conversation.

### Who is this for?

- **Alumni Relations Managers** — Quickly check member professional updates and event registrations on the go.
- **HR & Talent Teams** — Research former employees for boomerang hiring or reference via chat.
- **Operations Teams** — Monitor network growth and organizational engagement metadata instantly.


## Available Tools
- **get_enterprisealumni_metadata**: Retrieve metadata and limits for your EnterpriseAlumni account
- **get_alumni_detailed_profile**: Get detailed profile information for a specific alumni member
- **get_network_engagement_summary**: Retrieve a high-level summary of network engagement metrics
- **quick_alumni_network_audit**: Retrieve a high-level summary of alumni, events, and job postings
- **list_alumni_members**: List all members in your EnterpriseAlumni network
- **list_alumni_engagement_campaigns**: List all outreach and engagement campaigns
- **list_alumni_communities**: List all interest-based communities and groups within the alumni network
- **list_alumni_events**: List all upcoming and past alumni events
- **list_alumni_job_board**: List job opportunities available within the alumni network
- **search_alumni_by_name_or_keyword**: Search for alumni members using a name, skill, or keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EnterpriseAlumni** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all members in the New York community."

**🤖 AI Agent:**
> I've found 45 members in the New York community, including 'John Miller' (Senior Analyst) and 'Alice Connor' (Product Manager). 5 members recently updated their professional status. Would you like to see the details for John Miller?

---

**👤 You:**
> "Show me upcoming alumni events."

**🤖 AI Agent:**
> I've retrieved 3 upcoming events: 'Annual Gala 2024' (London, May 15th), 'Tech Networking Night' (Virtual, May 20th), and 'Career Mentorship Workshop' (May 25th). Should I pull the registration list for the Annual Gala?

---

**👤 You:**
> "Search for alumni with experience in 'Marketing'."

**🤖 AI Agent:**
> I've found 12 alumni with 'Marketing' in their professional background, including 'Sarah Connor' (Marketing Director at Wayne Corp) and 'David Smith' (Brand Lead). Would you like to see Sarah's full career history?


## ❓ FAQ

**Q: How do I get an EnterpriseAlumni API Key?**
Log in to your EnterpriseAlumni administrator dashboard, navigate to **Settings > API Integration**, and you can generate or retrieve your unique REST API Key from there.

**Q: Can the agent invite new members?**
This integration currently focuses on listing and auditing alumni members, events, and jobs. Inviting or onboarding new members should be managed via the EnterpriseAlumni platform dashboard or automated HR integrations.

**Q: Does the integration show real-time engagement?**
Yes, you can use the get_network_engagement_summary tool to retrieve high-level statistics on current network activity and participation rates across the community.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/enterprisealumni](https://vinkius.com/mcp/enterprisealumni)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EnterpriseAlumni** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `enterprisealumni` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EnterpriseAlumni** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprisealumni": {
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
