# Froged MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/froged)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage customer success, track events, and handle omnichannel support via AI agents with Froged.

## Description
Connect your **Froged** account to any AI agent to automate your customer success and support operations through the Model Context Protocol (MCP). Froged is an omnichannel customer service platform designed to improve retention and engagement. This MCP server enables you to track behavioral events, manage customer profiles, and participate in support conversations directly through natural conversation.

### Key Features

- **Contact Management** — List all customer profiles, fetch detailed metadata, and programmatically create or update contacts to maintain a 360-degree view.
- **Behavioral Event Tracking** — Access recent user events and post custom behavioral data (e.g., 'plan_upgraded') to trigger automated marketing campaigns.
- **Support Conversations** — List active support chats across all channels and post replies to conversations seamlessly.
- **Marketing Campaigns** — Retrieve a list of all active marketing and in-app campaigns to monitor engagement.
- **Knowledge Base Access** — Fetch published help articles from your Knowledge Base to aid in self-service support.
- **Real-time Synchronization** — Keep your customer success data and support inbox perfectly aligned with your internal tools.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Froged API Key (found in your Admin Settings)
3. Start managing your customer operations from Claude, Cursor, or any MCP client

### Who is this for?

- **Customer Success Managers** — quickly check user profiles and recent activity events without navigating the Froged dashboard.
- **Support Agents** — get a real-time overview of active conversations and post quick replies via simple AI commands.
- **Marketing Teams** — automate the logging of custom behavioral events to ensure the right in-app campaigns are triggered.


## Available Tools
- **verify_api_status**: Verify API connection
- **get_contact_details**: Get contact metadata
- **get_chat_details**: Get conversation history
- **list_marketing_campaigns**: List active campaigns
- **list_cs_contacts**: List Froged contacts
- **list_support_conversations**: List support chats
- **list_behavioral_events**: List tracked events
- **list_kb_articles**: List help articles
- **send_chat_message**: Send support reply
- **track_custom_event**: Track user behavior
- **upsert_contact**: Create/Update contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Froged** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 5 most recent active support conversations."

**🤖 AI Agent:**
> Retrieving conversations... I found 5 active chats, including a pricing inquiry from 'jane@example.com' and a bug report from 'john@example.com'.

---

**👤 You:**
> "Track the event 'plan_upgraded' for user 'customer@email.com'."

**🤖 AI Agent:**
> Event tracked! The 'plan_upgraded' event has been successfully logged for customer@email.com. Any associated onboarding campaigns will now trigger.

---

**👤 You:**
> "Show me the contact profile for 'jane@example.com'."

**🤖 AI Agent:**
> Searching contacts... I found Jane Doe (jane@example.com). She signed up 30 days ago and last interacted with support yesterday regarding 'API limits'.


## ❓ FAQ

**Q: How do I get an API Key for Froged?**
Log in to your Froged Admin Panel, navigate to Settings > Integrations > API, and you can generate or copy your active API Key.

**Q: Can I track custom events to trigger campaigns?**
Yes! Use the 'track_custom_event' tool. Provide the event name and the user's email to log the behavior and trigger any associated workflows.

**Q: Is it possible to reply to support chats through the agent?**
Yes, use the 'send_chat_message' tool with the specific Conversation ID to post replies directly to the omnichannel inbox.

**Q: How do I sync a new user to Froged?**
Use the 'upsert_contact' tool. Provide the user's email address, and if they don't exist, a new profile will be created. If they do, their metadata will update.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/froged](https://vinkius.com/mcp/froged)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Froged** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `froged` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Froged** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "froged": {
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
