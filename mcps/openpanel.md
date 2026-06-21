# OpenPanel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openpanel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Track events, identify users, and manage profile properties directly from your AI agent using OpenPanel analytics.

## Description
Connect your **OpenPanel** account to any AI agent and manage your product analytics and user profiles through natural conversation.

### What you can do

- **Event Tracking** — Record user actions and events with custom properties to understand application usage.
- **User Identification** — Link events to specific individuals and maintain consistent user profiles across sessions.
- **Property Management** — Dynamically increment or decrement numeric properties on user profiles (e.g., credits, points, or login counts).
- **Profile Enrichment** — Set traits and custom metadata on user profiles to segment your audience effectively.

### How it works

1. Subscribe to this server
2. Enter your OpenPanel API Key
3. Start tracking events and managing users from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Product Managers** — track feature adoption and user milestones without writing code.
- **Developers** — integrate analytics tracking into workflows and verify event payloads instantly.
- **Growth Hackers** — update user traits and manage reward points or usage limits via simple commands.


## Available Tools (4)
- **decrement_property**: Decrement a numeric property on a user profile
- **identify_user**: Identify a user in OpenPanel
- **increment_property**: Increment a numeric property on a user profile
- **track_event**: Track an event in OpenPanel


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenPanel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track a 'Sign Up' event for user 'user_99' with property 'source' as 'web'."

**🤖 AI Agent:**
> I've recorded the 'Sign Up' event for user_99. The event has been sent to OpenPanel with the source property set to web.

---

**👤 You:**
> "Identify user 'alex_123' and set their email to 'alex@example.com'."

**🤖 AI Agent:**
> User alex_123 has been identified and their profile has been updated with the email alex@example.com.

---

**👤 You:**
> "Increment the 'credits' property by 50 for profile 'pro_user_01'."

**🤖 AI Agent:**
> Successfully incremented the 'credits' property by 50 for profile pro_user_01.


## ❓ FAQ

**Q: How do I track a specific user action like a button click?**
Use the `track_event` tool. Provide the event name (e.g., 'Button Clicked') and optionally include a `profile_id` and custom `properties` to add context to the action.

**Q: Can I update user profile information or traits?**
Yes! Use the `identify_user` tool with the user's `profile_id`. You can pass a JSON object of `properties` to set or update traits like email, name, or subscription status.

**Q: How do I manage numeric counters like 'points' or 'credits' for a user?**
You can use `increment_property` to increase a value or `decrement_property` to decrease it. Just specify the `profile_id`, the `property` name, and the `value` to change.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openpanel](https://vinkius.com/mcp/openpanel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OpenPanel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `openpanel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OpenPanel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "openpanel": {
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
