# Listclean MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/listclean)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Verify and validate email addresses in real-time or batch via the Listclean API.

## Description
Connect your **Listclean** account to any AI agent to automate your email hygiene and deliverability workflows. This MCP server enables your agent to verify single email addresses instantly, process batch validations, and monitor your verification credits directly from natural language interfaces.

### What you can do

- **Real-time Verification** — Instantly check if an email address is clean, dirty, or risky before sending
- **Batch Processing** — Validate large lists of email addresses (up to 3,000 per request) efficiently
- **History Oversight** — Retrieve logs of previously performed single verifications to track your activity
- **Credit Management** — Monitor your remaining verification credits to ensure uninterrupted service
- **Data Quality Audit** — Identify catch-all, disposable, and role-based emails to maintain a high-quality contact list

### How it works

1. Subscribe to this server
2. Enter your Listclean API Key (X-Auth-Token)
3. Start validating your emails from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — Maintain high deliverability by cleaning contact lists via simple natural language commands
- **Sales Teams** — Instantly verify lead emails before reaching out to reduce bounce rates
- **Growth Engineers** — Integrate email validation logic and log monitoring directly into your development tools


## Available Tools
- **verify_batch_emails**: Maximum recommended size is 3,000 per request.

Verify multiple email addresses in one batch
- **check_account_credits**: Check remaining verification credits
- **get_verification_logs**: Retrieve logs of previously verified single emails
- **get_account_profile**: Get account profile details
- **verify_single_email**: Requires a single email string.

Verify a single email address in real-time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Listclean** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify the email address 'test@example.com' in Listclean."

**🤖 AI Agent:**
> I've checked the address. 'test@example.com' is marked as 🟢 Clean (valid email). You can safely send to this recipient.

---

**👤 You:**
> "Show my recent email verification logs."

**🤖 AI Agent:**
> I've retrieved your logs. Your last 5 verifications include addresses from 'gmail.com', 'outlook.com', and a disposable domain. Would you like the full details for any of them?

---

**👤 You:**
> "How many verification credits do I have left?"

**🤖 AI Agent:**
> You currently have 12,450 verification credits remaining in your Listclean account.


## ❓ FAQ

**Q: What do the statuses 'clean' and 'dirty' mean?**
'Clean' means the email address is valid and safe to send. 'Dirty' means the email is invalid, non-existent, or highly likely to bounce.

**Q: How many emails can I verify at once?**
The `verify_batch_emails` tool supports JSON arrays. It is recommended to keep batches under 3,000 emails per request for optimal performance.

**Q: Where do I find my API Key?**
Log in to your Listclean dashboard and navigate to Account Settings or Profile to find your unique X-Auth-Token.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/listclean](https://vinkius.com/mcp/listclean)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Listclean** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `listclean` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Listclean** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "listclean": {
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
