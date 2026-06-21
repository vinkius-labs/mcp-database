# GrowthZone MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/growthzone)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate association management via GrowthZone — manage contacts, memberships, events, and organizations directly from any AI agent.

## Description
Connect your **GrowthZone** AMS to any AI agent and take full control of your association management workflows through natural conversation.

### What you can do

- **Member & Contact Management** — List, search, and retrieve detailed profiles for any contact or member in your database.
- **Membership Oversight** — Monitor membership statuses, list types, and verify renewal information seamlessly.
- **Event Coordination** — List all scheduled events and dive into specific event details or registration lists.
- **Organization Insights** — Retrieve metadata and organizational structures for member companies and groups.
- **Automated Reporting** — Use AI to compile lists of expiring memberships or upcoming event participants in seconds.

### How it works

1. Subscribe to this server
2. Enter your GrowthZone API Key and Database Subdomain
3. Start managing your association from Claude, Cursor, or any MCP-compatible client

No more manual exports or jumping between complex CRM tabs. Your AI assistant acts as a dedicated membership coordinator or event manager.

### Who is this for?

- **Membership Directors** — instantly retrieve member statuses and list upcoming renewals without manual data mining.
- **Event Managers** — check registration counts and participant details straight from the communication flow.
- **Executive Assistants** — automate organizational lookups and contact management to keep operations running smoothly.


## Available Tools
- **get_contact**: Get detailed information about a specific contact by ID
- **get_my_profile**: Get information about the current authenticated user/account
- **list_contacts**: List all contacts in the GrowthZone database
- **list_events**: List all events in GrowthZone
- **list_membership_types**: List all available membership types
- **list_memberships**: List all memberships in GrowthZone
- **list_organizations**: List all organizations in GrowthZone
- **search_contacts**: Search for contacts in GrowthZone using a filter query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GrowthZone** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all contacts with 'Growth' in their name."

**🤖 AI Agent:**
> I've searched your database. I found 3 contacts matching 'Growth': John Growth (ID: 101), Growth Corp (ID: 102), and Alice Growthman (ID: 103). Would you like to see the full profile for any of them?

---

**👤 You:**
> "Show me the upcoming events for this month."

**🤖 AI Agent:**
> Fetching events... You have two major events scheduled: 'Annual General Meeting' on April 15th and 'Networking Gala' on April 22nd. Should I list the current registrations for either event?

---

**👤 You:**
> "What are our current membership types?"

**🤖 AI Agent:**
> Accessing membership data... You currently offer: 'Individual', 'Corporate Silver', 'Corporate Gold', and 'Non-Profit Partner'. Would you like to see the count of members for each type?


## ❓ FAQ

**Q: How do I obtain my GrowthZone API key?**
You must request an API key from GrowthZone WebSupport. They will verify your account's API access level and provide the credentials needed to connect your agent.

**Q: Can I search for specific members by their email or name?**
Yes! Use the `search_contacts` tool. You can provide a name or email address as a query, and the agent will return all matching profiles from your database.

**Q: How can I see who is registered for an upcoming event?**
Simply ask the agent to list participants for a specific Event ID. It will fetch the registration list and provide names and details of all attendees.

**Q: Is the integration secure for managing my association's data?**
Absolutely. The connection uses industry-standard API keys and focuses on querying operations. Your credentials are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/growthzone](https://vinkius.com/mcp/growthzone)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GrowthZone** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `growthzone` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GrowthZone** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "growthzone": {
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
