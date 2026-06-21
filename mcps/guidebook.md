# Guidebook MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/guidebook)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate mobile app content management via Guidebook — manage guides, sessions, speakers, and custom lists directly from any AI agent.

## Description
Connect your **Guidebook Builder** account to any AI agent and manage your mobile event or organization app content through natural conversation.

### What you can do

- **Guide Oversight** — List all mobile guides in your account and retrieve detailed metadata for each.
- **Schedule Management** — Browse, list, and inspect schedule sessions to keep your event timeline up to date.
- **Speaker Coordination** — Access speaker profiles and presenter details to ensure all bio information is accurate.
- **Custom Lists** — Manage Exhibitors, Sponsors, or any other custom data lists within your app.
- **Venue & Locations** — Retrieve all defined locations and map data for your event.
- **Rate Limit Tracking** — Monitor your API usage to stay within your daily quota.

### How it works

1. Subscribe to this server
2. Enter your Guidebook API Key (JWT token)
3. Start managing your app content from Claude, Cursor, or any MCP-compatible client

No more manual data entry in the Builder interface. Your AI assistant acts as a dedicated content coordinator for your mobile apps.

### Who is this for?

- **Event Organizers** — quickly verify session times and speaker assignments without digging through the CMS.
- **Content Managers** — automate the retrieval and auditing of custom lists like exhibitors or sponsors.
- **App Developers** — integrate Guidebook content flows into your development environment seamlessly.


## Available Tools
- **get_guide**: Get detailed information about a specific guide
- **get_rate_limit**: Check current API usage and rate limits
- **get_session**: Get details for a specific schedule session
- **get_speaker**: Get details for a specific speaker profile
- **list_custom_lists**: List custom list items (e.g., Exhibitors, Sponsors) for a guide
- **list_guides**: List all guides available in the account
- **list_locations**: List all locations/venues defined for a guide
- **list_schedules**: List schedules for a specific guide
- **list_sessions**: List all schedule sessions for a specific guide
- **list_speakers**: List all speakers/presenters for a specific guide


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Guidebook** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active mobile guides in my account."

**🤖 AI Agent:**
> I've retrieved your guides. You have 3 active projects: 'Global Tech Summit 2024' (ID: 8821), 'Internal Sales Kickoff' (ID: 8825), and 'Partner Conference Q2' (ID: 8830). Which guide would you like to inspect?

---

**👤 You:**
> "Show the schedule sessions for guide ID 8821."

**🤖 AI Agent:**
> Fetching sessions for Guide 8821... I found 5 main sessions for today, including 'Opening Keynote' at 09:00 AM, 'Cloud Infrastructure Workshop' at 11:30 AM, and 'Networking Lunch' at 01:00 PM. Should I get more details on any of these?

---

**👤 You:**
> "Who are the speakers for the Global Tech Summit?"

**🤖 AI Agent:**
> Accessing speakers for Guide 8821... I've identified 12 profiles, including Dr. Sarah Chen (AI Research), Marcus Viera (DevOps Lead), and Jane Doe (UX Design). Would you like to see a specific speaker's full bio?


## ❓ FAQ

**Q: How do I generate my Guidebook API Key?**
Log in to Guidebook Builder, click your profile dropdown in the top right, select 'Manage your account', and then navigate to the 'API Key' section to generate your token.

**Q: Can I see the schedules for multiple guides?**
Yes! You can use `list_guides` to find the IDs for all your guides, and then use `list_sessions` or `list_schedules` with the specific guide ID to see its agenda.

**Q: How many requests can I make to the Guidebook API?**
The Guidebook Open API typically has a limit of 10,000 requests per day per account. You can use the `get_rate_limit` tool to check your current usage.

**Q: What format should the API Key be in?**
The API Key should be the raw JWT token provided by the Guidebook Builder. The integration will automatically handle the 'JWT' prefix for authorization.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/guidebook](https://vinkius.com/mcp/guidebook)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Guidebook** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `guidebook` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Guidebook** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "guidebook": {
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
