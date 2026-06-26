# kvCORE MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kvcore)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Manage real estate leads — search contacts, track listings, and audit agent tasks.

## Description
Connect your AI agent to **kvCORE**, the primary platform for real estate professionals to manage their entire business.

### Key Features

- **Lead Management** — Search and audit lead profiles, update statuses, and add manual notes through natural language
- **Listing Intelligence** — Access active property listings and detailed metadata including features and pricing
- **Marketing Visibility** — List and monitor smart campaigns and automated marketing sequences
- **Agent Workflow** — Audit pending tasks, reminders, and recent lead activities to stay on top of follow-ups
- **Profile Insights** — Fetch agent profile data and high-level account configuration

### Simple Setup

1. Subscribe to this server
2. Log in to kvCORE, go to **Settings** > **API**, and generate an API Key
3. Enter your key in the configuration panel
4. Start managing your real estate business via chat


## Available Tools (10)
- **list_agent_tasks**: List pending tasks for the agent
- **get_agent_profile**: Get current agent information
- **update_lead_info**: g., status, phone). Provide data as a JSON string.

Update an existing lead
- **list_lead_activity**: List recent activity for a lead
- **create_lead_note**: Add a note to a lead profile
- **search_kvcore_leads**: Returns lead IDs and basic contact info.

Search for leads in kvCORE
- **get_lead_details**: Get details for a specific lead
- **list_property_listings**: List active property listings
- **get_listing_details**: Get metadata for a specific listing
- **list_marketing_campaigns**: List all marketing campaigns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **kvCORE** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for a lead named 'Alice' in my kvCORE"

**🤖 AI Agent:**
> I've found one lead matching 'Alice': Alice Williams (Email: alice@example.com). She is currently in the 'Prospect' status. Would you like to see her recent property views?

---

**👤 You:**
> "Show me details for the property at '123 Maple St'"

**🤖 AI Agent:**
> Retrieved listing details for 123 Maple St. It's a 3-bed, 2-bath home listed at $450,000. It has been on the market for 15 days. Would you like to see the full description?

---

**👤 You:**
> "List my tasks for today"

**🤖 AI Agent:**
> You have 5 follow-up tasks for today, including calling John Doe about the new listing and sending a contract to Jane Smith. Which one would you like to mark as complete?


## ❓ FAQ

**Q: Where do I find my kvCORE API Key?**
Log in to your kvCORE dashboard, navigate to the **Marketplace** or **API** settings section to generate a token.

**Q: Can I update lead status with this server?**
Yes, use the `update_lead_info` tool and provide the fields you want to modify in a JSON string.

**Q: Does this support MLS searches?**
The `list_property_listings` tool retrieves properties available within your kvCORE integrated MLS data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kvcore](https://vinkius.com/mcp/kvcore)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **kvCORE** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kvcore` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **kvCORE** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kvcore": {
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
