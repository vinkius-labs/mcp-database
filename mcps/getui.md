# GeTui / 个推 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/getui)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Massive notification push and LBS platform in China — manage campaigns, devices, and reports via AI.

## Description
Empower your AI agent to orchestrate your push notification infrastructure with **GeTui** (个推), the dominant CPaaS and developer services provider in China. By connecting GeTui to your agent, you transform complex device targeting, message broadcasting, and delivery auditing into a natural conversation. Your agent can instantly send targeted notifications to specific users, broadcast messages to your entire user base, retrieve real-time delivery and click statistics, and monitor user online status without you ever needing to navigate the comprehensive GeTui Developer Center. Whether you are automating verification flows or coordinating large-scale promotional alerts, your agent acts as a real-time messaging assistant, keeping your communication flow accurate and your user insights up-to-date.

### What you can do

- **Push Orchestration** — Send targeted, list-based, or broadcast notifications with full support for custom payloads.
- **User Status Monitoring** — Retrieve real-time online/offline status and associate custom aliases with Client IDs (CIDs).
- **Tag & Interest Auditing** — Browse user tags to identify audience segments and interest patterns for refined targeting.
- **Delivery Analytics** — Access real-time statistics for push tasks, including delivery counts, display rates, and clicks.
- **Growth Insights** — Monitor application-wide statistics for new and active users across specific dates.

### How it works

1. Subscribe to this server
2. Enter your GeTui App ID, App Key, and Master Secret
3. Start managing your push infrastructure through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Operations** — automate system notifications and monitor delivery health through natural language queries.
- **Marketing Leads** — coordinate time-sensitive promotional pushes and audit user engagement directly from your AI-powered workspace.
- **DevOps Engineers** — monitor system-wide push task performance and user connection health via a unified AI interface.
- **GeTui Power Users** — integrate your existing push workflows into your AI-driven daily routines.


## Available Tools (10)
- **bind_user_alias**: g., username) with a Client ID.

Bind alias to user
- **get_app_user_stats**: Get application user stats
- **get_cid_status**: Check user online status
- **get_daily_push_report**: Get daily push report
- **get_push_status**: Check push task status
- **get_user_tags**: Get user tags
- **push_to_all**: Broadcast push to all users
- **push_to_list**: Send push to multiple users
- **push_to_single**: Send push to single user
- **query_user_alias**: Query user alias


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GeTui / 个推** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a push notification to CID '1a0918c...' with title 'Urgent Update'."

**🤖 AI Agent:**
> I've initiated the targeted push notification for the specified user. The task ID is '8821'. Would you like me to check the delivery status in a few minutes?

---

**👤 You:**
> "Check the online status for user CID '9920a1b...'."

**🤖 AI Agent:**
> I've checked the status for the specified CID. The user is currently 'Online' and connected to the GeTui push server. Should I check their associated tags as well?

---

**👤 You:**
> "Show me the push report for yesterday."

**🤖 AI Agent:**
> I've retrieved the push statistics for yesterday. You had 15 total push tasks reaching 120,000 users with an average display rate of 85%. Would you like a detailed breakdown of the task with the highest click-through rate?


## ❓ FAQ

**Q: How do I find my GeTui App ID and Master Secret?**
Log in to the [GeTui Developer Center](https://dev.getui.com/), select your application from the dashboard, and you will find your AppID, AppKey, and MasterSecret in the application overview section.

**Q: Can I check if a specific user is currently online?**
Yes. Use the `get_cid_status` tool with the user's Client ID (CID) to retrieve their current connection status to the GeTui push server.

**Q: Is it possible to list the tags for a user?**
Yes! Use the `get_user_tags` tool with a Client ID to retrieve all tags associated with that user, helping you understand their segment and interests.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/getui](https://vinkius.com/mcp/getui)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GeTui / 个推** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `getui` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GeTui / 个推** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "getui": {
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
