# Swiftfox MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/swiftfox)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Generate product mockups and marketing visuals instantly with AI that places your designs on real-world backgrounds.

## Description
Connect your **Swiftfox** account to any AI agent and take full control of your member management, engagement strategy, and communication campaigns through natural conversation.

### What you can do

- **Member Management** — List, query, and update individual member profiles and custom data fields.
- **Interaction Tracking** — Log notes, calls, and meetings to maintain a complete history of member engagement.
- **Campaign Insights** — Monitor the performance of your communication campaigns and verify outreach success.
- **Event Monitoring** — List and query interactions to stay on top of your community activity.
- **Operational Status** — Fetch account metadata and check API connectivity directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Swiftfox API Key (found in your account settings)
3. Start managing your CRM ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Member Success Managers** — quickly retrieve profile details and log interactions via simple AI commands.
- **Campaign Coordinators** — monitor communication results and verify member segments directly from the workspace.
- **Non-Profit Leaders** — maintain organized records of community engagement and donor interactions via the AI assistant.


## Available Tools
- **check_swiftfox_status**: Returns a status indicator and account metadata to confirm valid credentials and active connectivity.

Verify Swiftfox API connectivity
- **get_event_fields**: Useful for understanding the data schema before creating or filtering events.

Get custom field definitions for events
- **get_organization**: Get full details of a specific organization in Swiftfox
- **get_person**: Get full details of a specific person in Swiftfox
- **list_circles**: Optionally filter by a search term matching circle names.

List circles (groups/domains/units) in Swiftfox
- **list_events**: Events represent meetings, functions, or activities organized within the CRM.

List events in Swiftfox CRM
- **list_organizations**: Organizations represent companies, associations, or groups that people belong to. Optionally filter by search term.

List organizations in Swiftfox CRM
- **list_people**: Optionally filter by a search term that matches against names or other fields.

List people (members) in Swiftfox CRM
- **list_webhooks**: Webhooks notify external services when specific events occur (e.g., member created, subscription updated).

List configured webhooks in Swiftfox
- **get_me**: Use this to verify connectivity or obtain the current user context.

Get the authenticated Swiftfox user profile
- **list_person_subscriptions**: Subscriptions track membership plans, payment status, and renewal dates.

List subscriptions for a specific person


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swiftfox** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the most recently active members in Swiftfox."

**🤖 AI Agent:**
> I've fetched the latest active members. The list includes: Robert Lewin (Last seen 2h ago), Martha Stewart, and David Beckham. Would you like to check the interaction history for any of them?

---

**👤 You:**
> "Log a new interaction: 'Follow-up call completed' for member ID '10293'."

**🤖 AI Agent:**
> Interaction logged! I've added the note 'Follow-up call completed' to member 10293's profile. The engagement history has been updated in Swiftfox.

---

**👤 You:**
> "Show me the details for member 'Martha Stewart'."

**🤖 AI Agent:**
> I've retrieved Martha Stewart's profile (ID: m_88231). She is a 'VIP Donor' and her last campaign interaction was 'Newsletter Open' yesterday. Shall I list her full contact data?


## ❓ FAQ

**Q: Can I search for a member by their custom ID?**
Yes! Use the `get_member` tool and provide the appropriate ID. Your agent will retrieve the complete profile and custom field data for that member.

**Q: How do I log a new phone call with a member?**
Use the `create_interaction` tool. Provide the Member ID, the interaction type (e.g., 'call'), and your notes. The agent will instantly log it in the member's history.

**Q: Is it possible to see the status of a specific campaign?**
Absolutely. Use the `list_campaigns` query. The agent will retrieve a list of all your outreach efforts along with their current status and engagement metrics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/swiftfox](https://vinkius.com/mcp/swiftfox)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Swiftfox** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `swiftfox` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Swiftfox** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swiftfox": {
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
