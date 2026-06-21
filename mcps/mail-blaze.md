# Mail Blaze MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mail-blaze)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email marketing campaigns and subscriber lists via the Mail Blaze REST API.

## Description
Connect your **Mail Blaze** account to any AI agent to automate your email marketing and audience management. This MCP server enables your agent to manage subscriber lists, create and send campaigns, and track subscriber updates directly from natural language interfaces.

### What you can do

- **Campaign Management** — List all email campaigns and retrieve detailed metadata and status information
- **Instant Sending** — Trigger the delivery of existing campaigns to your targeted lists instantly
- **List Oversight** — Manage subscriber lists and retrieve their unique identifiers for grouping
- **Subscriber Control** — Add, update, and remove subscribers from specific lists while managing custom fields
- **Draft Creation** — Initialize new campaign drafts directly from your conversation to streamline your marketing workflow

### How it works

1. Subscribe to this server
2. Enter your Mail Blaze API Public Key (X-MW-PUBLIC-KEY)
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — Monitor campaign statuses and manage subscriber segments via simple natural language commands
- **Marketing Operations** — Quickly update contact information and trigger campaign sends without opening the dashboard
- **Developers** — Integrate email automation logic and subscriber management into your custom internal tools


## Available Tools
- **add_subscriber_to_list**: Requires a list UID and subscriber data.

Add a new subscriber to a list
- **list_email_campaigns**: List all email marketing campaigns
- **create_new_campaign**: Requires a JSON body with campaign details.

Create a new email marketing campaign
- **delete_list_subscriber**: Remove a subscriber from a list
- **get_campaign_details**: Get details for a specific campaign
- **list_list_subscribers**: List subscribers in a specific list
- **list_subscriber_lists**: List all subscriber lists
- **send_email_campaign**: Trigger the sending of a campaign
- **update_list_subscriber**: Update an existing subscriber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mail Blaze** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active email campaigns in Mail Blaze."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 5 campaigns, including 'Summer Sale 2024 (ID: sb123abc)', 'Welcome Series', and 'Monthly Newsletter'. Which one would you like to see details for?

---

**👤 You:**
> "Add 'user@example.com' to my 'Main Leads' list (UID: 'lz987xyz')."

**🤖 AI Agent:**
> Successfully added user@example.com to the list Main Leads. The subscriber UID is 'sub-abc-123' and their status is currently 'confirmed'.

---

**👤 You:**
> "Send the email campaign with UID 'cp456def'."

**🤖 AI Agent:**
> I've triggered the sending of campaign cp456def. Mail Blaze has queued the delivery to your subscribers.


## ❓ FAQ

**Q: How do I find my List UID or Campaign UID?**
You can retrieve all UIDs by using the `list_subscriber_lists` or `list_email_campaigns` tools. They are also visible in the URL when viewing these resources in the Mail Blaze dashboard.

**Q: Can I add custom fields when subscribing a user?**
Yes, include your custom field values within the `subscriber_json` object when using the `add_subscriber_to_list` tool.

**Q: Is there a limit to the number of subscribers I can retrieve?**
The API uses pagination. The `list_list_subscribers` tool retrieves the first page of results (up to 100 records by default).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mail-blaze](https://vinkius.com/mcp/mail-blaze)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mail Blaze** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mail-blaze` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mail Blaze** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mail-blaze": {
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
