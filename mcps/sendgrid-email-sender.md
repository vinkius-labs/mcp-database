# SendGrid Email Sender MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sendgrid-email-sender)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

This MCP does exactly one thing: it sends transactional emails using Twilio SendGrid. That's its only function, and nothing else. Incredible for giving your AI agents the ability to dispatch email reports.

## Description
We refused to build a bloated email marketing suite that tries to manage contact lists, suppression groups, and A/B testing campaigns. Instead, this MCP server provides a surgical, zero-trust bridge: **just sending transactional emails.**

Your AI agent gains the immediate, zero-friction ability to drop rich HTML reports, password resets, or executive summaries straight to any inbox via SendGrid's robust delivery network.

### The Superpowers

- **Rich HTML Delivery:** The agent isn't limited to plain text. It can generate complete HTML emails—with tables, inline styles, and images—perfect for executive reporting.
- **Zero-Bloat Integration:** No massive SDKs or complex SMTP setups needed. Just an API Key and a verified 'From' email address.
- **Absolute Containment:** Because this is strictly a sending tool using the `mail/send` endpoint, the agent cannot read your inbox, cannot manage your contacts, and cannot alter your SendGrid domain settings. It is the purest, safest way to give your AI email superpowers.


## Available Tools (1)
- **send_sendgrid_email**: Provide the destination email in the "to" parameter, the subject, and the body content. You can set the "isHtml" boolean parameter to true to send rich HTML emails.

Send an email using the Twilio SendGrid API v3


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SendGrid Email Sender** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an email to john@example.com letting him know the analysis is complete."

**🤖 AI Agent:**
> I've successfully dispatched the email to john@example.com via SendGrid.

---

**👤 You:**
> "Generate a weekly summary report in HTML format and email it to my boss."

**🤖 AI Agent:**
> The HTML formatted weekly report has been generated and emailed successfully.


## ❓ FAQ

**Q: Can the agent read my emails with this?**
No. This MCP utilizes the REST API strictly for creating new messages (`v3/mail/send`). It does not use IMAP or POP3, meaning it acts strictly as a one-way notification megaphone. It cannot see your inbox.

**Q: Why do I need a verified From Email?**
SendGrid requires all senders to verify their identity (via Single Sender Verification or Domain Authentication) to protect against spam and spoofing. You can only send emails from an address you have verified in the SendGrid dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sendgrid-email-sender](https://vinkius.com/mcp/sendgrid-email-sender)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SendGrid Email Sender** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sendgrid-email-sender` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SendGrid Email Sender** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sendgrid-email-sender": {
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
