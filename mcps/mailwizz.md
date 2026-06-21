# MailWizz MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailwizz)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage email marketing campaigns and subscriber lists via the MailWizz REST API.

## Description
Connect your **MailWizz** instance to any AI agent to automate your professional email marketing and audience management. This MCP server enables your agent to manage subscriber lists, control campaign lifecycles, and update subscriber data directly from natural language interfaces.

### What you can do

- **Campaign Oversight** — List all email campaigns and retrieve detailed metadata and status information
- **Mailing Control** — Pause or unpause campaigns and manage their delivery lifecycle programmatically
- **Audience Management** — List all subscriber collections (lists) and retrieve their unique identifiers
- **Subscriber Administration** — Add, update, and remove subscribers from specific lists using their UIDs
- **Data Ingestion** — Sync subscriber information and manage custom fields across your email databases
- **Self-Hosted Support** — Works with any self-hosted MailWizz instance using your personal API keys

### How it works

1. Subscribe to this server
2. Enter your MailWizz API URL and Public Key
3. Start managing your marketing audience from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — Monitor campaign results and manage subscriber segments via simple natural language commands
- **CRM Specialists** — Quickly update contact information and audit list health without leaving your productivity tools
- **Developers** — Integrate MailWizz's robust marketing logic into your custom internal tools


## Available Tools
- **add_subscriber_to_list**: Requires a list UID and subscriber data.

Add a new subscriber to a list
- **list_email_campaigns**: List all email marketing campaigns
- **delete_list_subscriber**: Remove a subscriber from a list
- **get_campaign_details**: Get details for a specific campaign
- **get_list_details**: Get details for a specific subscriber list
- **list_list_subscribers**: List subscribers in a specific list
- **list_subscriber_collections**: List all subscriber lists
- **pause_email_campaign**: Pause a running campaign
- **update_list_subscriber**: Update an existing subscriber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MailWizz** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active email campaigns in MailWizz."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 5 campaigns, including 'Product Launch Q4 (UID: sb123abc)', 'Monthly Update', and 'Re-engagement Flow'. Which one would you like to see metadata for?

---

**👤 You:**
> "Add 'user@example.com' to my 'Main Leads' list (UID: 'lz987xyz')."

**🤖 AI Agent:**
> Successfully added user@example.com to the list Main Leads. The subscriber UID is 'sub-abc-123' and they are now ready to receive your mailings.

---

**👤 You:**
> "Pause the email campaign with UID 'cp456def'."

**🤖 AI Agent:**
> I've triggered the pause command for campaign cp456def. MailWizz has updated the status and sending is now suspended.


## ❓ FAQ

**Q: How do I find my List UID or Campaign UID?**
You can retrieve all UIDs by using the `list_subscriber_collections` or `list_email_campaigns` tools. They are also visible in the URL when viewing these resources in your MailWizz dashboard.

**Q: Can I add custom fields when subscribing a user?**
Yes, include your custom field values (like FNAME, LNAME) within the `subscriber_json` object when using the `add_subscriber_to_list` tool.

**Q: What is the API URL?**
This is the full base URL where your MailWizz API is reachable, for example: `https://mail.yourdomain.com/api`. Your token is encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailwizz](https://vinkius.com/mcp/mailwizz)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MailWizz** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mailwizz` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MailWizz** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mailwizz": {
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
