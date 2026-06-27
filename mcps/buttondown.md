# Buttondown MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/buttondown)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage your newsletter via Buttondown — track subscribers, send emails, and monitor analytics directly from any AI agent.

## Description
Connect your **Buttondown** account to any AI agent and orchestrate your newsletter, subscriber management, and email campaigns through natural conversation.

### What you can do

- **Subscriber Oversight** — List all your subscribers and retrieve detailed profiles, including metadata and tags.
- **Email Management** — List all sent emails and drafts, and create new campaigns or drafts directly from your workspace.
- **Analytics Tracking** — Retrieve detailed analytics for specific emails, including open and click rates.
- **Segment Coordination** — Access and list your tags to ensure your audience is properly categorized.
- **Newsletter Access** — List all newsletters managed in your account and access your core profile settings.
- **Subscriber Growth** — Add new subscribers directly from your workspace with custom tags and metadata.

### How it works

1. Subscribe to this server
2. Enter your Buttondown API Key
3. Start managing your newsletter from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Writers & Content Creators** — quickly check subscriber counts or draft new updates without manual dashboard work.
- **Marketers** — retrieve email performance metrics and manage audience tags straight from their workflow tools.
- **Developers** — integrate newsletter subscription and campaign steps into their environment using natural language.


## Available Tools (10)
- **create_subscriber**: Add a new subscriber to the newsletter
- **get_email_analytics**: Get analytics for a specific email
- **get_email**: Get details of a specific email
- **get_subscriber**: Get details of a specific subscriber
- **list_newsletters**: List all newsletters in the account
- **list_tags**: List all subscriber tags
- **create_email**: Create a new email or draft
- **get_account_info**: Retrieve core account/profile settings
- **list_emails**: List all sent emails and drafts
- **list_subscribers**: List all newsletter subscribers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Buttondown** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my newsletter subscribers."

**🤖 AI Agent:**
> I've retrieved your subscribers. You have 150 active subscribers, including 'john.doe@example.com' and 'jane.smith@example.com'. Would you like to see details for a specific subscriber?

---

**👤 You:**
> "Show analytics for my last sent email."

**🤖 AI Agent:**
> Retrieving analytics... Your last email 'Weekly Updates #42' has a 45% open rate and a 12% click rate from 150 recipients.

---

**👤 You:**
> "Create a new draft with subject 'Hello World' and body 'This is a test'."

**🤖 AI Agent:**
> Draft 'Hello World' has been successfully created in your Buttondown account with ID email_99283.


## ❓ FAQ

**Q: Can I check the open rate for a specific email using the agent?**
Yes! Use the `get_email_analytics` tool with the Email ID. Your agent will fetch the detailed statistics, including deliveries, opens, and clicks, directly from Buttondown.

**Q: How do I add a new subscriber with a specific tag?**
Simply ask the agent to `create_subscriber` and provide the email address and a JSON array of tags, for example: `["customer", "api-lead"]`. The subscriber will be added to Buttondown instantly.

**Q: Does the integration allow creating a new draft email?**
Yes. Use the `create_email` action and set the status to `draft`. You can provide the subject and the body in markdown format, and it will appear in your Buttondown account ready for review.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/buttondown](https://vinkius.com/mcp/buttondown)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `buttondown` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Buttondown** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "buttondown": {
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
