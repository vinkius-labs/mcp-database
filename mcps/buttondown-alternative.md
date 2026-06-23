# Buttondown MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buttondown-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate your newsletter and subscriber management via Buttondown — manage lists, draft emails, and track tags directly from any AI agent.

## Description
Connect your **Buttondown** account to any AI agent to streamline your newsletter operations and audience growth through natural conversation.

### What you can do

- **Subscriber Management** — List, create, update, and delete subscribers. Manage metadata and tags to segment your audience effectively.
- **Email Campaigns** — Draft new emails, schedule them with specific publish dates, and retrieve details of sent or scheduled campaigns.
- **Newsletter Insights** — List and inspect the newsletters associated with your account to maintain a clear overview of your publications.
- **Tagging & Organization** — Create and list tags to keep your subscriber base organized and target your communications precisely.
- **Webhook Integration** — Manage webhooks to connect Buttondown events with your other tools and workflows.

### How it works

1. Subscribe to this server
2. Enter your Buttondown API Key
3. Start managing your newsletter directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — draft and schedule newsletters without leaving your writing environment
- **Marketing Teams** — automate subscriber imports and tag management for better segmentation
- **Developers** — integrate newsletter workflows into your internal tools or IDEs


## Available Tools (14)
- **create_email**: Create a new email
- **create_subscriber**: Create a new subscriber
- **create_tag**: Create a new tag
- **create_webhook**: Create a new webhook
- **delete_subscriber**: Delete a subscriber
- **get_email**: Retrieve a specific email
- **get_newsletter**: Retrieve a specific newsletter
- **get_subscriber**: Retrieve a specific subscriber
- **list_emails**: List all emails
- **list_newsletters**: List all newsletters
- **list_subscribers**: List all subscribers
- **list_tags**: List all tags
- **list_webhooks**: List all webhooks
- **update_subscriber**: Update an existing subscriber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Buttondown** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my most recent subscribers on Buttondown."

**🤖 AI Agent:**
> I've retrieved your subscriber list. You have 150 total subscribers. The most recent additions include 'alice@example.com' and 'bob@work.com'.

---

**👤 You:**
> "Create a new email draft with the subject 'Monthly Newsletter' and a simple greeting in the body."

**🤖 AI Agent:**
> Draft created successfully! The email 'Monthly Newsletter' is now saved in your Buttondown account with the ID 'em_12345'.

---

**👤 You:**
> "Get the details for subscriber ID 'sub_98765'."

**🤖 AI Agent:**
> Subscriber found: 'charlie@provider.net'. They are currently active, have the tags ['premium', 'weekly'], and joined on 2023-10-12.


## ❓ FAQ

**Q: Can I schedule a newsletter for a future date using the AI?**
Yes. When using the `create_email` tool, you can provide an ISO 8601 timestamp in the `publish_date` field to schedule your email for later.

**Q: How do I add tags to a subscriber when creating them?**
You can use the `create_subscriber` tool and pass an array of strings in the `tags` parameter to categorize the new subscriber immediately.

**Q: Is it possible to update the email address of an existing subscriber?**
Yes, use the `update_subscriber` tool with the subscriber's unique ID and provide the new email address in the `email` field.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buttondown-alternative](https://vinkius.com/mcp/buttondown-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Buttondown** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `buttondown-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Buttondown** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "buttondown-alternative": {
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
