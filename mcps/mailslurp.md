# MailSlurp MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailslurp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage temporary inboxes and automate email testing via the MailSlurp REST API.

## Description
Connect your **MailSlurp** account to any AI agent to automate your email testing and asynchronous message management. This MCP server enables your agent to create virtual inboxes, send and receive emails, and handle complex automation scenarios using long-polling 'wait-for' methods directly from natural language interfaces.

### What you can do

- **Virtual Inbox Management** — Create random or custom email addresses and list all managed inboxes in your account
- **Email Automation** — Long-poll for the latest incoming email or wait until a specific email count is reached for testing suites
- **Message Retrieval** — List and inspect messages received by any virtual address, including full HTML and text bodies
- **Outbound Capability** — Send emails directly from any of your MailSlurp addresses programmatically
- **Infrastructure Maintenance** — Permanently delete individual messages or entire virtual inboxes via simple commands
- **Metadata Inspection** — Retrieve detailed technical headers and attachment metadata for any received email

### How it works

1. Subscribe to this server
2. Enter your MailSlurp API Key (x-api-key)
3. Start managing your virtual email infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **QA Engineers** — Automate the verification of user registration flows and transactional alerts via natural language
- **Developers** — Quickly inspect incoming test emails and manage temporary addresses directly from your IDE
- **Product Teams** — Monitor and audit automated communication paths and email delivery results effortlessly


## Available Tools (8)
- **list_inbox_emails**: List emails received by an inbox
- **get_email_details**: Get complete content for a specific email
- **list_all_inboxes**: List all MailSlurp inboxes
- **send_email_from_inbox**: Requires recipient and content.

Send an email using a MailSlurp address
- **wait_for_email_count**: Wait until an inbox has a certain number of emails
- **wait_for_latest_email**: Returns the latest one immediately if present.

Long-poll for the next incoming email
- **create_random_inbox**: Create a new random email address
- **delete_specific_inbox**: Delete an inbox and its emails


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MailSlurp** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new random inbox in MailSlurp."

**🤖 AI Agent:**
> I've created a new inbox. The address is 'abc-123@mailslurp.com' and the ID is 'inbox-xyz'. You can now use it to receive emails.

---

**👤 You:**
> "Wait for the next email to arrive in inbox 'inbox-xyz'."

**🤖 AI Agent:**
> I'm monitoring the inbox. [Connection held] ... I've received an email from 'no-reply@service.com' with the subject 'Verify your account'. Would you like the text body?

---

**👤 You:**
> "Send an email to 'user@example.com' from inbox 'inbox-xyz'."

**🤖 AI Agent:**
> I've sent the email to user@example.com from your virtual inbox inbox-xyz. The message has been successfully delivered to the outbound queue.


## ❓ FAQ

**Q: How do I find my Inbox ID?**
Use the `list_all_inboxes` tool to see a comprehensive list of all your MailSlurp addresses along with their unique IDs.

**Q: What is the benefit of the 'wait-for' tools?**
They hold the connection until an email arrives, making it easy to test asynchronous processes (like password resets) without writing complex retry loops.

**Q: Where do I find my API Key?**
Log in to your MailSlurp dashboard and copy the API key from the Home or API Settings section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailslurp](https://vinkius.com/mcp/mailslurp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MailSlurp** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mailslurp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MailSlurp** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mailslurp": {
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
