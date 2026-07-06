# AfterLogic Aurora MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/afterlogic-aurora)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Email and webmail management — manage folders, messages, and accounts via AI.

## Description
Connect your **AfterLogic Aurora** account to your AI agent to unlock professional email and webmail orchestration. From managing complex mail folder structures to retrieving message lists and handling administrative account tasks, your agent handles your communication platform through natural conversation.

### What you can do

- **Mail Orchestration** — List and manage email folders and retrieve message lists for any account
- **Administrative Management** — Check if accounts exist and manage domains or users via the REST Admin API
- **Communication Flow** — Send and retrieve technical metadata for emails to support your communication workflows
- **Integration Support** — Access both the Web API for user-level tasks and the REST API for system-wide administration
- **Status Monitoring** — Quickly audit mail server availability and account statuses directly from your chat interface

### How it works

1. Subscribe to this server
2. Enter your AfterLogic Aurora Base URL and Auth Credentials
3. Start managing your emails and mail accounts through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Mail Administrators** — automate user provisioning and domain management effortlessly
- **IT Support Teams** — quickly check account statuses and folder structures to resolve inquiries
- **Developers** — integrate Aurora's mail capabilities into custom applications and workflows
- **Operations Leads** — monitor communication platform health and manage user access using simple commands


## Available Tools (5)
- **list_folders**: Retrieve the internal email folder hierarchy for the authenticated AfterLogic user
- **list_messages**: Requires a folder path from list_folders.

Retrieve recent emails contained within a specified AfterLogic mail folder
- **check_account_exists**: Requires Admin rights.

Verify if an email address is actively provisioned on the AfterLogic server
- **send_email**: Compose and send an outbound email securely via the AfterLogic Web API
- **list_domains**: Requires Admin rights.

Retrieve all active custom domains mapped to the AfterLogic server instance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AfterLogic Aurora** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all mail folders for user 'admin@example.com'."

**🤖 AI Agent:**
> I've retrieved the folder list for admin@example.com. You have 5 standard folders: INBOX, Sent, Drafts, Spam, and Trash, along with 2 custom subfolders. Which folder would you like to open?

---

**👤 You:**
> "Check if the account 'user1@example.com' exists on the server."

**🤖 AI Agent:**
> I've checked the server records. The account 'user1@example.com' exists and is currently active. Would you like to see the quota usage for this account?

---

**👤 You:**
> "Show me the last 10 messages in the INBOX."

**🤖 AI Agent:**
> I've retrieved the latest 10 messages from your INBOX. They include 3 new inquiries, 2 system notifications, and several personal emails. Would you like the technical details for any specific message?


## ❓ FAQ

**Q: Where do I find my AfterLogic API URL?**
The Web API endpoint is typically your Aurora installation URL followed by `/?/Api/`. The REST Admin API endpoint is your URL followed by `/rest.php/`. Consult your system administrator for the specific base path.

**Q: Can I check if an email account exists?**
Yes! Use the `check_account_exists` tool. It uses the REST Admin API to verify if a specific email address is registered on your server.

**Q: Does this support sending emails?**
Yes, you can use the `send_message` tool to compose and send emails via the Web API on behalf of an authenticated user.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/afterlogic-aurora](https://vinkius.com/mcp/afterlogic-aurora)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AfterLogic Aurora** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `afterlogic-aurora` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AfterLogic Aurora** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "afterlogic-aurora": {
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
