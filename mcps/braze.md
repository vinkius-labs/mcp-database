# Braze MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/braze)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Manage customer engagement via Braze — track users, list campaigns, and trigger canvases directly from any AI agent.

## Description
Connect your **Braze** customer engagement platform to any AI agent and orchestrate your marketing automation and user tracking workflows through natural conversation.

### What you can do

- **User Orchestration** — Track new user attributes and events, identify anonymous users, or permanently delete user profiles for compliance.
- **Campaign Management** — List all your marketing campaigns, retrieve detailed metadata, and instantly trigger API-based campaign sends to specific users.
- **Canvas (Journey) Control** — List and inspect multi-step Canvases, and trigger users to enter specific Canvas workflows.
- **Data Export** — Programmatically export user profile data by their external IDs.

### How it works

1. Subscribe to this server
2. Enter your Braze REST API Key and Base URL (e.g., https://rest.iad-01.braze.com)
3. Start managing your customer journeys from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **get_canvas_details**: Get details of a specific Canvas
- **track_user**: Track user attributes or events
- **trigger_campaign**: Trigger an API-triggered campaign
- **trigger_canvas**: Trigger a Canvas journey
- **delete_user**: Delete a user by external ID
- **export_user_ids**: Export profile data for specific users
- **get_campaign_details**: Get details of a specific campaign
- **identify_user**: Identify a user (merge alias to external ID)
- **list_campaigns**: List all campaigns
- **list_canvases**: List all Canvases


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Braze** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active campaigns in Braze."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 3 active campaigns: 'Welcome Series' (ID: camp_1), 'Abandoned Cart' (ID: camp_2), and 'Holiday Promo' (ID: camp_3).

---

**👤 You:**
> "Track user 'usr_992' with attribute {'loyalty_tier':'Gold'}."

**🤖 AI Agent:**
> The user attribute 'loyalty_tier: Gold' has been successfully tracked for user 'usr_992'.

---

**👤 You:**
> "List all Canvases configured in the workspace."

**🤖 AI Agent:**
> Retrieving Canvases... You have 2 active Canvases: 'Onboarding Journey' (ID: can_1) and 'Win-back Flow' (ID: can_2).


## ❓ FAQ

**Q: Can I trigger an API campaign for a specific user?**
Yes! Use the `trigger_campaign` tool with the Campaign ID and a JSON array of recipient objects (e.g., `[{"external_user_id":"123"}]`).

**Q: How do I update a user's custom attribute?**
Simply ask the agent to `track_user` and provide the External ID along with the new attributes in JSON format (e.g., `{"favorite_color":"blue"}`).

**Q: Does the integration allow permanently deleting a user for GDPR compliance?**
Yes. Use the `delete_user` mutation with the user's External ID. This will permanently remove their profile and data from your Braze dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/braze](https://vinkius.com/mcp/braze)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Braze** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `braze` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Braze** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "braze": {
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
