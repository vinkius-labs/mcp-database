# Mail-in-a-Box MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mail-in-a-box)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage mail users, aliases, and system health via the Mail-in-a-Box REST API.

## Description
Connect your **Mail-in-a-Box** instance to any AI agent to automate your private email server management. This MCP server enables your agent to manage mailboxes, configure forwarding aliases, and monitor system health and diagnostics directly from natural language interfaces.

### What you can do

- **User Administration** — List all mail users, create new mailboxes, and update passwords programmatically
- **Alias Management** — Create, update, and remove email forwarding addresses and group aliases
- **System Monitoring** — Retrieve real-time health status, diagnostic checks, and configuration metadata for your server
- **Domain Oversight** — List all hosted mail domains and subdomains configured on your instance
- **Access Control** — Manage administrative privileges and account settings for your email users

### How it works

1. Subscribe to this server
2. Enter your Mail-in-a-Box Host, Admin Email, and Admin Password (or API Key)
3. Start managing your private email infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **System Administrators** — Manage mailboxes and forwarding rules via simple natural language commands
- **DevOps Engineers** — Automate user onboarding and system health monitoring directly from your dev tools
- **Privacy-Conscious Teams** — Maintain your private communication infrastructure effortlessly through an AI-integrated interface


## Available Tools (9)
- **create_mail_user**: Requires a full email address and a password.

Add a new mail user (mailbox)
- **list_mail_aliases**: List all mail aliases and forwarders
- **list_mail_domains**: List all mail domains hosted on the server
- **delete_mail_alias**: Remove a mail alias
- **delete_mail_user**: Remove a mail user
- **update_user_password**: Change the password for a mail user
- **get_system_status**: Check the status of the Mail-in-a-Box system
- **create_or_update_alias**: forwards_to should be a comma-separated list of emails.

Add or update a mail alias
- **list_mail_users**: List all mail users on the server


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mail-in-a-Box** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all mail users on my server."

**🤖 AI Agent:**
> I've retrieved the users. You have 12 mailboxes across 2 domains, including 'admin@example.com', 'user1@example.com', and 'team@otherdomain.io'.

---

**👤 You:**
> "Create a new mail user 'support@example.com' with password 'MySecret123!'."

**🤖 AI Agent:**
> Successfully created the mailbox for support@example.com. The user can now log in via IMAP/SMTP or webmail.

---

**👤 You:**
> "How is the health status of my Mail-in-a-Box server?"

**🤖 AI Agent:**
> I've checked the system status. All core services (DNS, IMAP, SMTP) are running correctly. 2 minor updates are available for your OS.


## ❓ FAQ

**Q: What format is required for the instance host?**
Provide the full hostname without the 'https://' prefix, for example: `box.yourdomain.com`.

**Q: Can I add multiple forwarding targets to an alias?**
Yes, when using the `create_or_update_alias` tool, provide a comma-separated list of emails in the `forwards_to` field.

**Q: Does this work with 2FA enabled accounts?**
The current API implementation uses Basic Auth. If 2FA is enabled on your admin account, you may need to use an API key or a dedicated admin user without 2FA for the integration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mail-in-a-box](https://vinkius.com/mcp/mail-in-a-box)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mail-in-a-Box** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mail-in-a-box` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mail-in-a-Box** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mail-in-a-box": {
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
