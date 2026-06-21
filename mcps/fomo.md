# Fomo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fomo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage social proof notifications, push real-time events, and oversee templates via AI agents with Fomo.

## Description
Connect your **Fomo** account to any AI agent to automate your social proof marketing and notification feeds through the Model Context Protocol (MCP). Fomo allows you to programmatically push real-time customer interactions, such as purchases or sign-ups, directly to your website's live feed. This MCP server enables you to manage your notification events, design new templates, and monitor integrations directly through natural conversation.

### Key Features

- **Real-time Events** — Push new customer interactions to your live feed and manage existing events instantly.
- **Template Design** — Programmatically create and list notification templates to define how your social proof looks.
- **Event Monitoring** — Retrieve paginated lists of recent events and fetch detailed metadata for specific notifications.
- **Integration Oversight** — Monitor all active third-party integrations connected to your Fomo account.
- **Application Insights** — Access metadata for your Fomo application to maintain full context of your marketing setup.
- **Clean Feed Management** — Update or delete events from your feed directly through the agent.

### How it works

1. Subscribe to this server
2. Enter your Fomo Auth Token (found in Settings > Site > API Access)
3. Start managing your social proof marketing directly from your AI agent


## Available Tools
- **create_event**: Push a new event to feed
- **create_template**: Create a new template
- **delete_event**: Remove event from feed
- **get_application_info**: Get account attributes
- **get_event**: Get event details
- **get_template**: Get template details
- **list_events**: List recent social proof events
- **list_integrations**: List active integrations
- **list_push_messages**: List sent messages
- **list_templates**: List notification templates
- **update_event**: Modify an existing event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fomo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the last 5 social proof events in my Fomo application."

**🤖 AI Agent:**
> Retrieving events... I found 5 recent notifications, including sign-ups from New York and purchases from London. Your feed is active.

---

**👤 You:**
> "Push a new sign-up event for 'Alex' from 'San Francisco' using template ID '123'."

**🤖 AI Agent:**
> Event created! 'Alex from San Francisco' has been pushed to your live social proof feed using template ID 123.

---

**👤 You:**
> "List all active notification templates in my account."

**🤖 AI Agent:**
> Retrieving templates... I found 3 templates: 'Standard Purchase', 'New Sign-up', and 'Live Visitor Count'. Which one would you like to inspect?


## ❓ FAQ

**Q: How do I get an Auth Token for Fomo?**
You can find your API token in your Fomo dashboard under Settings > Site > API Access.

**Q: Can I use the agent to create new notification designs?**
Yes, you can use the 'create_template' tool to programmatically add new notification shells using the {{ variable }} syntax.

**Q: How do I push a purchase event to my feed via the agent?**
Use the 'create_event' tool and provide the event_type_id along with metadata like first_name, city, and title.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fomo](https://vinkius.com/mcp/fomo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fomo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fomo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fomo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fomo": {
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
