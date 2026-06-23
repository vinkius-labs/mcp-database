# Mailsac MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailsac)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage disposable and private email addresses via the Mailsac REST API.

## Description
Connect your **Mailsac** account to any AI agent to automate your email testing and inbox management. This MCP server enables your agent to reserve private email addresses, retrieve and search for messages, and inspect HTML or plain text bodies directly from natural language interfaces.

### What you can do

- **Inbox Oversight** — List and manage your reserved (enhanced) addresses and custom domains
- **Instant Retrieval** — Fetch a list of messages received by any address in your account instantly
- **Content Extraction** — Retrieve sanitized HTML or raw plain text bodies to extract verification codes or links
- **Inbox Maintenance** — Permanently delete individual messages or clear entire inboxes via simple commands
- **Infrastructure Management** — Reserve new private addresses programmatically for isolated testing flows
- **Global Search** — Query messages across all your addresses using advanced search parameters (requires paid tier)

### How it works

1. Subscribe to this server
2. Enter your Mailsac API Key
3. Start managing your disposable inboxes from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — Automate the extraction of email-based verification codes for testing suites
- **Developers** — Quickly inspect incoming test emails and manage temporary addresses directly from your IDE
- **Privacy-Conscious Users** — Manage temporary communication channels via simple natural language commands


## Available Tools (9)
- **list_reserved_addresses**: List all reserved (enhanced) email addresses
- **delete_inbox_message**: Permanently remove a message from an inbox
- **list_custom_domains**: List custom domains linked to the account
- **get_html_message_body**: Get the sanitized HTML body of a specific message
- **get_plain_text_body**: Get the plain text body of a specific message
- **list_inbox_messages**: List messages in a specific inbox
- **release_reserved_address**: Delete/Release a reserved email address
- **reserve_new_address**: Reserve a specific email address
- **search_account_messages**: Requires a paid Mailsac tier. Use query params like to, from, subject.

Search for messages across all addresses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mailsac** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my reserved email addresses in Mailsac."

**🤖 AI Agent:**
> I've retrieved your reserved addresses. You have 3 active inboxes: 'test-user@mailsac.com', 'service-dev@mailsac.com', and 'alert-prod@mailsac.com'.

---

**👤 You:**
> "Fetch the plain text content of the last email sent to 'test-user@mailsac.com'."

**🤖 AI Agent:**
> I've retrieved the text body. The message contains a verification code: '123-456'. Would you like me to extract any other specific information?

---

**👤 You:**
> "Reserve a new private address 'automation-flow@mailsac.com'."

**🤖 AI Agent:**
> Successfully reserved 'automation-flow@mailsac.com'. This inbox is now private and enhanced, allowing you to capture messages exclusively.


## ❓ FAQ

**Q: What is an 'Enhanced' address in Mailsac?**
An enhanced address is a private inbox that only you can access. Use the `reserve_new_address` tool to make an address private/enhanced.

**Q: Can I read the raw SMTP source of an email?**
While this server provides tools for HTML and Plain Text bodies, the Mailsac API supports raw data retrieval. You can use the text body tool to extract key technical metadata.

**Q: Is an API Key required for all addresses?**
Yes, this MCP server requires an API Key to interact with your account and access your reserved resources and private messages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailsac](https://vinkius.com/mcp/mailsac)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mailsac** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mailsac` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mailsac** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mailsac": {
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
