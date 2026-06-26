# EnterpriseAlumni MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/enterprisealumni)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage alumni networks, track engagement, and monitor member profiles via the EnterpriseAlumni API.

## Description
Integrate **EnterpriseAlumni**, the strategic alumni engagement platform, directly into your AI workflow. Manage your corporate and academic alumni networks, track member profiles and professional history, monitor upcoming events and job board postings, and oversee your community engagement using natural language.

### What you can do

- **Member Oversight** — Search and retrieve detailed profiles, career history, and contact information for your alumni members.
- **Engagement Intelligence** — Monitor network engagement metrics, resolving activity levels and community participation trends.
- **Event Management** — Access and monitor alumni events and their invitee lists, tracking RSVP statuses.
- **Network Auditing** — Retrieve high-level summaries of member volume and organizational network health instantly.

### How it works

1. Connect the EnterpriseAlumni integration to your AI assistant.
2. Authorize using your **Client ID** and **Client Secret** from the API Access Manager, and select your regional gateway (EU, US, or UK).
3. Orchestrate your alumni relations and corporate community strategy through intuitive conversation.

### Who is this for?

- **Alumni Relations Managers** — Quickly check member professional updates and event registrations on the go.
- **HR & Talent Teams** — Research former employees for boomerang hiring or reference via chat.
- **Operations Teams** — Monitor network growth and organizational engagement metadata instantly.


## Available Tools (7)
- **get_user_by_guid**: Get detailed profile for an alumni by their userResourceGuid
- **search_alumni_users**: Supports filtering by first name, last name, approval status, and join dates.

Search alumni users by name, status, or date criteria
- **get_user_by_external_guid**: Get an alumni profile using an external system identifier
- **get_user_schema**: Retrieve the user data schema from the EnterpriseAlumni platform
- **search_alumni_events**: Search for upcoming and past alumni events
- **list_event_invitees**: List all invitees for a specific alumni event
- **get_alumni_network_summary**: Retrieve a high-level summary of the alumni network size and metadata


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EnterpriseAlumni** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for alumni named 'John'."

**🤖 AI Agent:**
> I found 12 alumni matching 'John', including 'John Miller' (Senior Analyst) and 'John Davis' (Product Manager). Would you like to see the full profile for John Miller?

---

**👤 You:**
> "Show me upcoming alumni events."

**🤖 AI Agent:**
> I retrieved 3 upcoming events: 'Annual Gala 2024' (London, May 15th), 'Tech Networking Night' (Virtual, May 20th), and 'Career Mentorship Workshop' (May 25th). Should I pull the invitee list for the Annual Gala?

---

**👤 You:**
> "How many alumni are in the network?"

**🤖 AI Agent:**
> Your alumni network has 2,847 registered members. The data shows steady growth with 45 new members joining in the last 30 days.


## ❓ FAQ

**Q: How do I get my Client ID and Client Secret?**
Log in to your EnterpriseAlumni Admin Portal, expand the **Site Manager** menu, select **API Access Manager**, and click **Create Key**. You will receive a Client ID and a Client Secret — save the secret immediately, as it is only shown once.

**Q: Which gateway region should I select?**
Select the region where your alumni instance was provisioned: **eu** (Frankfurt), **us** (United States), or **uk** (United Kingdom). Contact your EnterpriseAlumni account manager if you are unsure.

**Q: Does the integration show real-time engagement?**
Yes, you can use the get_alumni_network_summary tool to retrieve high-level statistics on current network activity and member counts across the community.


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
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprisealumni` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
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
