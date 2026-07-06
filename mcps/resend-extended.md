# Resend MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/resend-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate email delivery via Resend — send emails, manage domains, and track audiences directly from any AI agent.

## Description
Connect your **Resend** account to any AI agent and take full control of your transactional email orchestration through natural conversation. Resend provides a world-class email infrastructure for developers, and this integration allows you to send emails, monitor domain verification, and manage contact audiences directly from your chat interface.

### What you can do

- **Email Orchestration** — Send high-fidelity emails using custom HTML or text programmatically, with support for batch sending and history retrieval.
- **Domain Lifecycle Management** — List all managed domains and trigger verification processes directly from the AI interface to ensure deliverability.
- **Audience & CRM Control** — Create and manage contact audiences and individual subscribers via natural language to maintain your marketing lists.
- **API & Security Oversight** — Access and monitor your API keys to ensure your integration remains secure and synchronized.
- **Operational Monitoring** — Track system responses and manage email delivery logs using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your Resend API Key (re_xxxxxxxxx) from your settings
3. Start managing your email infrastructure from Claude, Cursor, or any MCP-compatible client

No more manual dashboard navigation for checking logs or verifying domains. Your AI acts as a dedicated email operations manager or delivery coordinator.

### Who is this for?

- **Developers & DevOps** — quickly send test emails and verify domain DNS records without switching tools.
- **Marketing Operations** — automate the management of contact audiences and monitor engagement via natural conversation.
- **Startup Founders** — streamline the retrieval of transactional email history directly within the chat.


## Available Tools (11)
- **get_domain_details**: Get details for a specific domain
- **get_email_details**: Get details for a specific email
- **list_api_keys**: List all API keys
- **list_audiences**: List contact audiences
- **list_contacts**: List contacts in an audience
- **list_domains**: List registered domains
- **list_sent_emails**: List sent emails
- **send_email**: Requires from, to, and subject.

Send a single email
- **verify_domain**: Verify a domain
- **create_audience**: Create a new audience
- **add_contact_to_audience**: Requires email.

Add a contact to an audience


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Resend** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a welcome email to test@example.com using HTML."

**🤖 AI Agent:**
> Processing email delivery... Your welcome message has been successfully accepted by Resend for delivery. Should I track the status for you?

---

**👤 You:**
> "Show me the delivery analytics for all emails sent through Resend this week."

**🤖 AI Agent:**
> Email analytics this week. Total sent: 4,567. Delivered: 4,489 (98.3%). Opened: 2,890 (64.4% open rate). Clicked: 1,234 (27.5% click rate). Bounced: 56 (1.2%). Complained: 12 (0.26%). Top performing: "Welcome Email" at 78% open rate. Lowest performer: "Newsletter #42" at 34% open. By domain: gmail.com 42%, outlook.com 23%, corporate domains 35%. Peak send time: Tuesday 10 AM. Average delivery time: 1.2 seconds.

---

**👤 You:**
> "Send a transactional email with the invoice PDF attachment to client@meridian.io."

**🤖 AI Agent:**
> Email sent successfully via Resend. To: client@meridian.io. From: billing@yourcompany.com. Subject: "Invoice #INV-2025-156 - May 2025". Attachment: invoice_2025_156.pdf (234 KB). Message ID: msg_7f2a9b. Delivery confirmed in 0.9 seconds. The email used your verified domain with DKIM and SPF authentication. Open tracking and click tracking enabled. A webhook will fire when the recipient opens the email.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific email just by providing its ID?**
Yes! Use the `get_email` tool with the Email ID. Your agent will respond with complete metadata, including delivery status, timestamps, and recipient info in seconds.

**Q: How do I find my Resend API Key?**
Log in to your Resend dashboard, navigate to the **API Keys** section, and generate a new key (it will start with `re_`). Copy and save it securely.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/resend-extended](https://vinkius.com/mcp/resend-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Resend** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `resend-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Resend** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "resend-extended": {
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
