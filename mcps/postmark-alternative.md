# Postmark MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/postmark-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate transactional email via Postmark — send emails, retrieve templates, inspect bounces, and manage your delivery analytics directly from any AI agent.

## Description
Connect your **Postmark** server to any AI agent to fully orchestrate and analyze your transactional email pipeline.

### What you can do

- **Send Emails & Templates** — Send transactional emails directly from the agent using pre-configured Postmark Templates or Raw HTML.
- **Investigate Bounces** — Read the server bounce log to find out why specific recipients failed delivery (Hard Bounces, Blocks).
- **Template Management** — Fetch and review the raw body of your templates to ensure dynamic variables align flawlessly with code.
- **Outbound Analytics** — Review message stream stats, open rates, and general health metrics directly via chat.

### How it works

1. Subscribe to this server
2. Enter your Postmark Server Token
3. Gain complete control of your application's email notifications from Claude, Cursor, or any MCP-compatible environment

### Who is this for?

- **Software Engineers** — Trigger template dispatches from the terminal and review server logs to debug application email flows seamlessly.
- **Product Teams** — Monitor bounce rates and verify the visual layout of critical system emails without accessing the Postmark UI.
- **System Admins** — Quickly query delivery analytics and trace email endpoints for quick operational overviews.


## Available Tools
- **get_bounces_overview**: Get bounce overview analytics
- **get_server**: Get Postmark server details
- **get_template**: Get a specific Postmark template details
- **list_templates**: List templates in the server
- **get_outbound_overview**: Get outbound overview analytics
- **search_bounces**: You can filter by type, email, or message ID.

Search email bounces
- **search_outbound_messages**: You can filter by recipient, from email, or status.

Search outbound messages history
- **send_email**: Requires From, To, and either Subject/HtmlBody or Subject/TextBody.

Send a transactional email
- **send_email_with_template**: Send an email using a Postmark Template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Postmark** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the bouncing metrics for our transactional emails."

**🤖 AI Agent:**
> I've analyzed your bounce metrics. The server currently has 14 Hard Bounces and 3 Soft Bounces within the query scope. Overall health looks good! Want me to list the specific emails?

---

**👤 You:**
> "Can you fetch the HTML body layout of our 'Welcome' template?"

**🤖 AI Agent:**
> I found your 'Welcome' template (ID: 809214). It expects three variables: `first_name`, `action_url`, and `support_email`. The HTML renders a classic logo-centric email layout.

---

**👤 You:**
> "Send a standard test email to alice@example.com using our current Postmark setup."

**🤖 AI Agent:**
> The email has been processed! Postmark returned success mapping with a Message ID `f8a847a9-2169-45e0-...` indicating instantaneous dispatch.


## ❓ FAQ

**Q: Can I use this server to actually send operational emails from my account?**
Yes! The `send_email` and `send_email_with_template` tools will dispatch active live emails using your Postmark server configuration.

**Q: How can I debug a specific user reporting that they didn't receive an email?**
You can ask the agent to execute `search_outbound_messages` or `search_bounces` using their exact email address. The agent will fetch the delivery log and status codes.

**Q: Do I need the Account Token or the Server Token to use this?**
You only need the **Server Token**. Postmark divides workflows by servers (environments). Supplying the server token isolates this specific operational environment perfectly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/postmark-alternative](https://vinkius.com/mcp/postmark-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Postmark** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `postmark-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Postmark** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "postmark-alternative": {
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
