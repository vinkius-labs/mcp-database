# KlickTipp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/klicktipp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Grow your German-speaking audience with tag-based email marketing that segments subscribers by behavior and interest.

## Description
Connect your **KlickTipp** account to any AI agent and simplify your email marketing and lead management through natural conversation.

### What you can do

- **Contact Management** — Subscribe new leads, retrieve subscriber profiles, and unsubscribe users programmatically
- **Tagging & Segmentation** — List all tags and apply or remove them from contacts to automate your segmentation
- **Subscription Processes** — Monitor available double opt-in processes and lists in your account
- **Custom Fields** — Query custom data fields to understand the metadata you can store for your leads

### How it works

1. Subscribe to this server
2. Enter your KlickTipp Username and Password
3. Start managing your marketing automation from Claude, Cursor, or any MCP-compatible client


## Available Tools (8)
- **get_contact**: Get details for a specific contact
- **list_fields**: List custom fields
- **list_subscription_processes**: List opt-in processes
- **list_tags**: List KlickTipp tags
- **subscribe_contact**: Subscribe a contact to a list
- **tag_contact**: Apply a tag to a contact
- **unsubscribe_contact**: Unsubscribe a contact
- **untag_contact**: Remove a tag from a contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KlickTipp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my KlickTipp tags."

**🤖 AI Agent:**
> I've retrieved your tags. You have 15 tags, including 'New Lead', 'Webinar Attendee', and 'Customer'.

---

**👤 You:**
> "Tag 'john@example.com' with tag ID '12345'."

**🤖 AI Agent:**
> Done! John Doe has been successfully tagged with 'Webinar Attendee'.

---

**👤 You:**
> "Unsubscribe 'old-user@example.com'."

**🤖 AI Agent:**
> I've processed the request. 'old-user@example.com' has been unsubscribed from your KlickTipp lists.


## ❓ FAQ

**Q: Can I automatically apply a tag to a contact using my AI agent?**
Yes! Use the `tag_contact` tool by providing the subscriber's email and the Tag ID.

**Q: How do I see all my available marketing tags?**
Use the `list_tags` tool. Your agent will retrieve the complete list of tags and their IDs from your account.

**Q: Is it possible to subscribe a new lead via this integration?**
Yes, use the `subscribe_contact` action. You will need to provide the email address and a valid Opt-in Process ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/klicktipp](https://vinkius.com/mcp/klicktipp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **KlickTipp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `klicktipp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **KlickTipp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "klicktipp": {
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
